---
name: ui-ux-bible
description: Use when a task involves designing, prototyping, implementing, auditing, or improving a web or mobile interface, user flow, landing page, dashboard, form, component, design system, SaaS product, conversational AI experience, accessibility, visual hierarchy, color, typography, navigation, conversion, UX writing, user testing, product metrics, acquisition, SEO, SEA or digital advertising, email marketing, social media, funnels, or analytics.
---

# UI/UX Bible

Appliquer ce routeur pour produire une interface compréhensible, cohérente, accessible et vérifiable. Charger uniquement les références utiles à la tâche.

## Ordre de travail

1. Reformuler l’objectif utilisateur, le public, le contexte, la plateforme et le résultat attendu.
2. Inspecter l’existant : produit, contenu, contraintes techniques, design system et données disponibles.
3. Classer chaque règle mobilisée comme exigence, convention, heuristique ou préférence.
4. Pour une question étroite, lire seulement la référence ciblée. Pour une tâche large, lire `references/core-principles.md`, puis commencer par une à trois références ciblées et élargir seulement si nécessaire.
5. Concevoir ou auditer le parcours avant de polir l’apparence. Couvrir contenu, structure, interactions, états et responsive.
6. Implémenter selon les conventions du projet. Réutiliser les composants et tokens existants lorsqu’ils satisfont les exigences.
7. Vérifier le résultat dans son contexte réel, puis appliquer la checklist finale.

## Invariants

- Faire primer les exigences explicites, l’accessibilité et l’intégrité du parcours sur les préférences esthétiques.
- Donner à chaque écran un objectif principal et une hiérarchie immédiatement perceptible.
- Réduire la mémorisation, les choix inutiles et les ambiguïtés ; employer des libellés explicites.
- Concevoir les états initial, survol, focus, actif, désactivé, chargement, vide, erreur et succès selon le composant.
- Préserver la navigation clavier, le focus visible, la lecture par technologies d’assistance et un contraste suffisant.
- Adapter la hiérarchie, le contenu et les cibles tactiles aux petits comme aux grands écrans.
- Prévenir les erreurs, expliquer leur correction et fournir un retour après chaque action.
- Refuser les dark patterns et ne jamais inventer une preuve, une norme, un benchmark ou une valeur « exacte ».

## Nature des décisions

| Nature | Traitement |
|---|---|
| Exigence | Appliquer l’obligation issue de la demande, du produit, d’une norme ou d’une contrainte validée. Signaler tout conflit. |
| Convention | Suivre le design system, la plateforme ou le code existant sauf conflit avec une exigence. |
| Heuristique | Utiliser comme point de départ testable, jamais comme vérité universelle. Indiquer l’hypothèse. |
| Préférence | Proposer comme choix subjectif et laisser une alternative lorsque l’impact est significatif. |

Respecter l’ordre `exigence > convention > heuristique > préférence`.

## Routeur des références

| Sujet | Lire |
|---|---|
| Principes transversaux | `references/core-principles.md` |
| Fondations UX | `references/ux-foundations.md` |
| Compréhension des utilisateurs | `references/understanding-users.md` |
| Architecture de l’information | `references/information-architecture.md` |
| Hiérarchie visuelle | `references/visual-hierarchy.md` |
| Couleur | `references/color.md` |
| Typographie | `references/typography.md` |
| Layout, grille, espacement | `references/layout-grid-spacing.md` |
| Composants génériques | `references/ui-components.md` |
| Boutons et CTA | `references/buttons.md` |
| Formulaires et validation | `references/forms.md` |
| Navigation | `references/navigation.md` |
| Cartes | `references/cards.md` |
| Tableaux de données | `references/data-tables.md` |
| Dashboards et visualisation | `references/dashboards.md` |
| Landing pages et conversion | `references/landing-pages-conversion.md` |
| UX writing et copywriting | `references/ux-writing-copywriting.md` |
| Accessibilité | `references/accessibility.md` |
| Design system et tokens | `references/design-system.md` |
| Audit UX/UI | `references/ux-audit.md` |
| Psychologie cognitive | `references/cognitive-psychology.md` |
| Lois UX | `references/ux-laws.md` |
| Micro-interactions et motion | `references/microinteractions-motion.md` |
| Produit SaaS | `references/saas.md` |
| Mobile | `references/mobile.md` |
| IA conversationnelle | `references/conversational-ai.md` |
| Métriques produit | `references/product-metrics.md` |
| Anti-patterns | `references/anti-patterns.md` |
| Vérification avant livraison | `references/release-checklist.md` |
| Tests utilisateurs et expérimentation | `references/user-testing-experimentation.md` |

## Sources volumineuses et marketing

- Commencer par `references/`. Ne pas charger plusieurs sources longues par défaut.
- Rechercher dans `sources/` avec des termes précis, puis lire seulement les passages entourant les résultats utiles.
- Résumer les principes nécessaires ; ne pas reproduire de longs extraits ni redistribuer les sources privées.
- Utiliser `sources/marketing-index.md` pour toute demande d’acquisition, SEO, SEA/publicité, emailing, réseaux sociaux, funnel ou analytics. Traiter ce corpus historique privé comme contexte exigeant une vérification actuelle.
- Vérifier en ligne, auprès de sources primaires récentes, tout fait marketing instable : prix, politiques de plateforme, formats, options de ciblage, algorithmes, benchmarks, réglementation et disponibilité régionale.
- Dater et sourcer les faits vérifiés. Présenter les chiffres non vérifiables comme hypothèses ou fourchettes, jamais comme normes.

## Checklist finale

- [ ] Confirmer l’objectif, le public et l’action principale.
- [ ] Charger seulement les références pertinentes et distinguer les quatre natures de décision.
- [ ] Vérifier hiérarchie, contenu, navigation, composants et cohérence avec l’existant.
- [ ] Couvrir responsive, clavier, focus, contraste, technologies d’assistance et cibles tactiles.
- [ ] Couvrir tous les états utiles, erreurs, cas vides, chargements et retours d’action.
- [ ] Tester le parcours principal et les cas d’échec dans le produit réel lorsque possible.
- [ ] Vérifier en ligne les faits instables et signaler clairement les hypothèses restantes.
- [ ] Supprimer les éléments sans fonction, les valeurs arbitraires et les dark patterns.
