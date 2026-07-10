# UI/UX Bible Refactor Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Convertir `ui-ux-bible` en un skill Codex valide, actuel, navigable et vérifié, puis publier la refonte sur `origin/master`.

**Architecture:** Garder un unique skill dont `SKILL.md` sert de routeur compact vers des références sémantiques à profondeur unique. Conserver les ouvrages privés comme sources brutes, mais ajouter des index de recherche et distinguer clairement exigences normatives, heuristiques, conventions de plateforme et contenu historique.

**Tech Stack:** Markdown, YAML, Git, scripts de validation Codex, recherches ciblées avec `rg`, sources officielles W3C/WAI et guides de plateforme.

---

## Structure cible

Fichiers principaux :

- `SKILL.md` : déclenchement, workflow, invariants, routeur et contrôle final.
- `agents/openai.yaml` : métadonnées d'interface Codex.
- `README.md` : présentation privée du dépôt et installation Codex.
- `references/*.md` : références opérationnelles structurées, une responsabilité par fichier.
- `sources/INDEX.md` : politique d'usage et routes de recherche vers les OCR privés.
- `sources/marketing-index.md` : index thématique du livre marketing historique.

Références canoniques :

```text
references/core-principles.md
references/ux-foundations.md
references/understanding-users.md
references/information-architecture.md
references/visual-hierarchy.md
references/color.md
references/typography.md
references/layout-grid-spacing.md
references/ui-components.md
references/buttons.md
references/forms.md
references/navigation.md
references/cards.md
references/data-tables.md
references/dashboards.md
references/landing-pages-conversion.md
references/ux-writing-copywriting.md
references/accessibility.md
references/design-system.md
references/ux-audit.md
references/cognitive-psychology.md
references/ux-laws.md
references/microinteractions-motion.md
references/saas.md
references/mobile.md
references/conversational-ai.md
references/user-testing-experimentation.md
references/product-metrics.md
references/anti-patterns.md
references/release-checklist.md
```

### Task 1: Capturer les échecs de référence

**Files:**
- Inspect: `SKILL.md`
- Inspect: `references/*.md`
- Inspect: `sources/*.md`

- [ ] **Step 1: Vérifier que le frontmatter actuel échoue sur la longueur**

Run:

```bash
ruby -ryaml -e 's=File.read("SKILL.md"); y=s.split(/^---\s*$\n/)[1]; d=YAML.safe_load(y).fetch("description"); puts d.length; abort "expected current description to exceed 1024" unless d.length > 1024'
```

Expected: affiche une valeur supérieure à `1024` et retourne `0`.

- [ ] **Step 2: Vérifier que les références ne sont pas structurées**

Run:

```bash
for f in references/*.md; do rg -q '^# ' "$f" || echo "$f"; done
```

Expected: les 28 fichiers actuels sont listés.

- [ ] **Step 3: Exécuter quatre scénarios sans le skill**

Utiliser des agents frais sans lecture du dépôt pour : inscription SaaS, audit d'interface, exigence WCAG précise, tactique marketing dépendante du temps. Conserver dans le fil principal les fichiers consultés, les omissions et les affirmations non vérifiées.

- [ ] **Step 4: Exécuter les mêmes scénarios avec la version actuelle**

Demander explicitement l'usage de `/Users/doti/.codex/skills/ui-ux-bible`. Mesurer le nombre de fichiers ouverts, la précision des routes et les recours à des sources externes.

### Task 2: Corriger le routeur et les métadonnées Codex

**Files:**
- Modify: `SKILL.md`
- Create: `agents/openai.yaml`
- Modify: `README.md`

- [ ] **Step 1: Remplacer le frontmatter par un déclencheur inférieur à 1 024 caractères**

Le texte doit commencer par `Use when` et couvrir les situations, pas le workflow :

```yaml
---
name: ui-ux-bible
description: Use when conceiving, building, reviewing, auditing, or improving a web or mobile interface, design system, SaaS product, dashboard, form, navigation, landing page, onboarding, checkout, pricing page, conversational AI experience, accessibility behavior, visual hierarchy, typography, color, spacing, UX writing, or conversion flow. Also use for UI implementation guidance in HTML/CSS, React, Vue, or Tailwind, and for digital-marketing requests that need the user's private reference corpus.
---
```

- [ ] **Step 2: Réécrire le corps comme routeur compact**

Conserver uniquement : ordre de travail, invariants transversaux, table sujet → fichier canonique, politique de recherche dans `sources/`, distinctions normatif/heuristique/historique et checklist de livraison. Viser moins de 1 000 mots.

- [ ] **Step 3: Générer `agents/openai.yaml` avec l'outil officiel**

Run:

```bash
python3 /Users/doti/.codex/skills/.system/skill-creator/scripts/generate_openai_yaml.py . \
  --interface 'display_name=UI/UX Bible' \
  --interface 'short_description=Concevoir et auditer des interfaces fiables et accessibles' \
  --interface 'default_prompt=Utilise $ui-ux-bible pour concevoir ou auditer cette interface en appliquant les références pertinentes.'
```

Expected: `agents/openai.yaml` existe et son prompt contient `$ui-ux-bible`.

- [ ] **Step 4: Actualiser le README**

Décrire un skill Codex privé, l'installation sous `~/.codex/skills/ui-ux-bible`, la séparation `references/`/`sources/`, et l'interdiction de republier les ouvrages privés.

- [ ] **Step 5: Vérifier et committer**

Run:

```bash
git diff --check
git add SKILL.md agents/openai.yaml README.md
git commit -m "refactor: streamline skill routing"
```

Expected: commit créé sans avertissement de whitespace.

### Task 3: Normaliser l'arborescence des références

**Files:**
- Rename: `references/01-*.md` à `references/28-*.md`
- Delete: `references/00-introduction.md`
- Create: `references/cards.md`
- Create: `references/data-tables.md`

- [ ] **Step 1: Extraire Navigation, Cartes et Data Tables**

Séparer `references/12-la-navigation.md` aux marqueurs `Chapitre 12 — Les Cartes` et `Chapitre 13 — Les Tableaux`. Supprimer les phrases de transition qui précèdent ces marqueurs et préserver intégralement les trois contenus utiles.

- [ ] **Step 2: Renommer chaque fichier selon la liste canonique**

Utiliser `git mv` afin que Git conserve l'historique. Supprimer `00-introduction.md`, qui ne contient qu'un résidu conversationnel.

- [ ] **Step 3: Corriger le premier titre de chaque fichier**

Remplacer la numérotation contradictoire par un unique `# Titre sémantique`. Aucun nom de référence ne doit dépendre d'un numéro de chapitre.

- [ ] **Step 4: Vérifier le découpage**

Run:

```bash
test "$(find references -maxdepth 1 -name '*.md' | wc -l | tr -d ' ')" = 29
rg -n 'Chapitre 12|Chapitre 13' references/navigation.md && exit 1 || true
test -s references/cards.md
test -s references/data-tables.md
```

Expected: 29 références avant l'ajout du chapitre de tests, et aucun chapitre Cartes/Tableaux dans `navigation.md`.

### Task 4: Structurer et nettoyer toutes les références existantes

**Files:**
- Modify: `references/*.md`

- [ ] **Step 1: Ajouter une structure Markdown cohérente**

Chaque fichier doit avoir exactement un H1, plusieurs H2 descriptifs, des listes Markdown valides et un `## Sommaire` pour les fichiers de plus de 100 lignes. Retirer les séparateurs `⸻` devenus inutiles.

- [ ] **Step 2: Supprimer le bruit éditorial**

Retirer les phrases adressées à l'utilisateur, les annonces du « prochain chapitre », les projets de volumes futurs et les réserves du modèle. Préserver les règles, exemples, contre-exemples et checklists utiles.

- [ ] **Step 3: Corriger les promesses et contradictions mesurables**

Supprimer les annonces « plus de 200 erreurs », « plus de 500 critères », « plus de 1 000 points » et « 300 composants » lorsqu'elles ne correspondent pas au contenu. Aligner l'échelle d'espacement du routeur avec la référence ou présenter `12 px` comme pas intermédiaire optionnel.

- [ ] **Step 4: Clarifier le statut des règles**

Employer les libellés `Exigence`, `Convention`, `Heuristique` ou `Préférence du manuel` lorsqu'une formulation pourrait être prise pour une norme universelle. Nuancer notamment « une page = un objectif », « une couleur = une information » et « ne jamais faire réfléchir ».

- [ ] **Step 5: Vérifier et committer**

Run:

```bash
for f in references/*.md; do rg -q '^# ' "$f" || exit 1; rg -q '^## ' "$f" || exit 1; done
! rg -n -i 'Parfait\. On va|Souhaites-tu|Je te propose|le prochain chapitre|plus de 1 000|plus de 500|plus de 200' references
git diff --check
git add references
git commit -m "refactor: organize ui ux references"
```

Expected: toutes les références passent les contrôles et le commit est créé.

### Task 5: Ajouter et actualiser les références normatives

**Files:**
- Create: `references/user-testing-experimentation.md`
- Modify: `references/accessibility.md`
- Modify: `references/forms.md`
- Modify: `references/buttons.md`
- Modify: `references/mobile.md`
- Modify: `references/release-checklist.md`

- [ ] **Step 1: Vérifier les normes actuelles dans les sources officielles**

Consulter au minimum WCAG 2.2, les Understanding Documents W3C/WAI pertinents, ARIA Authoring Practices et les guides officiels des plateformes pour les cibles tactiles. Ne reprendre que des seuils soutenus par les pages consultées.

- [ ] **Step 2: Mettre à jour l'accessibilité**

Documenter : contraste texte AA, contraste non textuel, focus visible et non masqué, taille de cible WCAG 2.2, authentification accessible, clavier, noms accessibles, erreurs et annonces dynamiques. Ajouter les liens officiels et la date de vérification.

- [ ] **Step 3: Créer la référence tests utilisateurs et expérimentation**

Inclure : question de recherche, recrutement, scénario non orienté, protocole, consentement, observation, prise de notes, sévérité, synthèse, priorisation, test modéré/non modéré, A/B test, hypothèse, métrique primaire, garde-fous, taille d'échantillon, durée, biais, arrêt anticipé et limites éthiques.

- [ ] **Step 4: Propager les règles applicables**

Aligner formulaires, boutons, mobile et checklist finale sur les exigences vérifiées. Ne pas confondre minimum WCAG, recommandation Apple et recommandation Android.

- [ ] **Step 5: Vérifier et committer**

Run:

```bash
rg -n 'WCAG 2\.2|w3\.org/WAI|Date de vérification' references/accessibility.md
rg -n '^# Tests utilisateurs et expérimentation|A/B|hypothèse|garde-fou' references/user-testing-experimentation.md
git diff --check
git add references
git commit -m "docs: update accessibility and user testing guidance"
```

Expected: les références contiennent les preuves attendues et le commit est créé.

### Task 6: Corriger les index des sources privées

**Files:**
- Modify: `sources/INDEX.md`
- Create: `sources/marketing-index.md`
- Inspect only: `sources/marketing-digital.md`
- Inspect only: `sources/color-palettes.md`
- Inspect only: `sources/component-gallery.md`
- Inspect only: `sources/font-recommendations.md`

- [ ] **Step 1: Corriger les faits de l'index principal**

Indiquer 24 palettes, expliquer que HSL et hex sont groupés par séries, qualifier Component Gallery et Font Recommendations d'OCR textuels privés ayant perdu leurs visuels, et corriger les chemins relatifs.

- [ ] **Step 2: Ajouter des commandes de recherche ciblées**

Pour chaque source de plus de 10 000 mots, fournir des exemples `rg -n -i 'motif' sources/fichier.md` et interdire le chargement intégral par défaut.

- [ ] **Step 3: Créer l'index marketing historique**

Cartographier les thèmes stratégie, SEO, SEA, emailing, réseaux sociaux, funnel, acquisition et analytics vers des motifs de recherche. Marquer le livre comme source de 2018 et exiger une vérification actuelle des plateformes, formats, politiques et benchmarks.

- [ ] **Step 4: Vérifier et committer**

Run:

```bash
rg -n '24 palettes|OCR textuel|2018|vérification actuelle|rg -n' sources/INDEX.md sources/marketing-index.md
git diff --check
git add sources/INDEX.md sources/marketing-index.md
git commit -m "docs: make private sources searchable"
```

Expected: les index signalent correctement la provenance et le caractère historique.

### Task 7: Retester le skill révisé

**Files:**
- Inspect: `SKILL.md`
- Inspect: `agents/openai.yaml`
- Inspect: `references/*.md`
- Inspect: `sources/*.md`

- [ ] **Step 1: Exécuter le validateur officiel**

Run:

```bash
python3 /Users/doti/.codex/skills/.system/skill-creator/scripts/quick_validate.py .
```

Expected: `Skill is valid!`. Si le Python système ne contient pas PyYAML, utiliser le runtime Python groupé par Codex sans modifier les dépendances du dépôt.

- [ ] **Step 2: Exécuter les contrôles d'intégrité**

Run:

```bash
ruby -ryaml -e 's=File.read("SKILL.md"); y=s.split(/^---\s*$\n/)[1]; d=YAML.safe_load(y).fetch("description"); abort if d.length > 1024'
for f in references/*.md; do test "$(rg -c '^# ' "$f")" = 1 || exit 1; rg -q '^## ' "$f" || exit 1; done
for p in $(rg -o 'references/[a-z0-9-]+\.md|sources/[A-Za-z0-9._/-]+\.md' SKILL.md | sort -u); do test -f "$p" || exit 1; done
git diff --check
```

Expected: aucune sortie d'erreur.

- [ ] **Step 3: Rejouer les quatre scénarios avec des agents frais**

Vérifier : bonnes routes, moins de lectures inutiles, seuils normatifs exacts, distinction entre faits actuels et source marketing historique, aucune source brute chargée intégralement.

- [ ] **Step 4: Corriger les nouvelles lacunes et rejouer les contrôles**

Limiter les changements aux échecs observés. Tous les contrôles des étapes 1 à 3 doivent repasser.

### Task 8: Nettoyer les artefacts de processus et préparer la livraison

**Files:**
- Delete: `docs/superpowers/specs/2026-07-10-ui-ux-bible-refactor-design.md`
- Delete: `docs/superpowers/plans/2026-07-10-ui-ux-bible-refactor.md`
- Modify if needed: `README.md`

- [ ] **Step 1: Retirer les documents de processus du package final**

Le dépôt final ne conserve ni spécification ni plan d'agent, conformément aux règles de packaging des skills.

- [ ] **Step 2: Vérifier l'inventaire final**

Run:

```bash
test ! -d docs/superpowers
find . -maxdepth 2 -type f -not -path './.git/*' | sort
git diff --check
```

Expected: uniquement `SKILL.md`, `README.md`, `agents/`, `references/` et `sources/` avec leurs fichiers utiles.

- [ ] **Step 3: Committer le nettoyage**

Run:

```bash
git add -A
git commit -m "chore: finalize ui ux bible package"
```

Expected: commit créé et arbre de travail propre.

### Task 9: Publier sur GitHub

**Files:**
- Inspect: dépôt Git complet

- [ ] **Step 1: Relire la portée du diff et l'historique**

Run:

```bash
git status --short --branch
git diff --stat origin/master...HEAD
git log --oneline origin/master..HEAD
```

Expected: branche `master` en avance, aucun fichier non committé, uniquement la refonte prévue.

- [ ] **Step 2: Pousser vers le dépôt demandé**

Run:

```bash
git push origin master
```

Expected: mise à jour réussie de `origin/master`.

- [ ] **Step 3: Vérifier la correspondance locale/distante**

Run:

```bash
test "$(git rev-parse HEAD)" = "$(git ls-remote origin refs/heads/master | cut -f1)"
git status --short --branch
```

Expected: hashes identiques et `master...origin/master` sans avance ni retard.
