---
name: ui-ux-bible
description: >-
  Manuel de référence UI/UX & marketing digital (le "Bible" de l'utilisateur) qui impose des règles
  précises de design d'interface — hiérarchie visuelle, couleurs, typographie, layout/grille,
  composants (boutons, formulaires, navigation, cartes, modales, tableaux), accessibilité, dashboards,
  landing pages, conversion, UX writing, design system, micro-interactions, mobile, SaaS, produits IA,
  anti-patterns et audit. Utilise systématiquement ce skill dès que la tâche touche à la conception,
  la construction, la revue ou l'amélioration d'une interface — même si l'utilisateur ne dit pas
  explicitement "UI" ou "UX". Déclencheurs typiques : "crée/designe/build une page / un écran / un
  composant / un formulaire / un bouton / une landing / un dashboard / une app", "améliore le design",
  "revois cette interface", "quelle couleur / typo / espacement", "audit UX", "design system",
  "page de login/signup/checkout/pricing", "onboarding", "chat IA", "accessibilité". Vaut aussi bien
  pour du HTML/CSS, React/Vue/Tailwind, une maquette, ou une simple recommandation de design.
  Couvre aussi le marketing digital complet (SEO, publicité/SEA, emailing, réseaux sociaux, tunnel de
  conversion, acquisition, analytics) — déclenche sur "stratégie marketing", "campagne", "SEO",
  "pub Facebook/Google", "newsletter", "funnel", "landing de vente". Inclut en plus les ouvrages de
  référence complets (Refactoring UI, Don't Make Me Think, The Design of Everyday Things, Color
  Palettes, Font Recommendations, Component Gallery, Le grand livre du marketing digital) pour donner
  une valeur concrète : palette avec codes hex exacts, police recommandée, variante de composant.
---

# UI/UX Bible — Guide de référence

Ce skill contient le manuel complet de l'utilisateur (28 chapitres) sur la conception d'interfaces et le marketing digital. C'est **la source de vérité** : quand tu conçois, construis, revois ou améliores une interface, applique ces règles.

**Directive centrale : l'utilisateur ne doit jamais avoir à réfléchir.** Une bonne interface disparaît — elle laisse la personne accomplir sa tâche vite, facilement, sans confusion. Tout ce qui suit sert ce but.

## Comment utiliser ce skill

Le manuel est trop grand pour être lu en entier à chaque fois. Fonctionne en deux temps :

1. **Le socle ci-dessous** (les 25 règles + principes transversaux) s'applique à *toute* interface. Garde-le en tête à chaque tâche.
2. **Avant tout travail détaillé sur un élément précis** (un formulaire, une palette, un dashboard…), **lis d'abord le chapitre de référence correspondant** dans `references/` via l'index plus bas. Chaque chapitre contient les règles fines, des exemples, des contre-exemples, une checklist et des cas réels. Ne devine pas — la réponse exacte y est.

Le but n'est pas de citer le livre à l'utilisateur, mais de produire un résultat qui **respecte** ces règles. Explique tes choix de design en une phrase quand c'est utile (« bouton primaire unique pour éviter l'hésitation »), sans noyer la personne sous la théorie.

## Le socle — les 25 règles fondamentales

Toujours valables, quel que soit l'écran (chapitre 01 pour le détail) :

1. L'utilisateur ne doit jamais réfléchir — actions et intitulés évidents, pas d'icône ambiguë seule.
2. Une page = un seul objectif principal.
3. La hiérarchie (taille, position, contraste, espace) prime sur la couleur.
4. Les éléments identiques se ressemblent toujours (même bouton, même état, même comportement).
5. Les espaces créent la structure — le vide est un outil, pas un manque.
6. Les gens *scannent*, ils ne lisent pas : titres courts, listes, forte hiérarchie.
7. Tout élément a une raison d'exister — sinon on le supprime.
8. L'action principale (CTA) est identifiable en moins d'une seconde.
9. Rendre les erreurs impossibles ou faciles à corriger (validation temps réel, annulation, confirmation des actions destructrices).
10. Donner un retour à chaque action (hover, chargement, succès, erreur).
11. La simplicité est le résultat d'un travail — supprimer est plus dur qu'ajouter.
12. Réduire le nombre de décisions (choix, menus, options).
13. Reconnaître plutôt que mémoriser (menus visibles, suggestions, historique, recherche).
14. Respecter les conventions du web (logo, menu, panier, recherche, profil, retour).
15. Chaque couleur porte une information — jamais « juste pour faire joli ».
16. Le contraste compte plus que la saturation.
17. L'information la plus importante apparaît en premier (titre → valeur → bénéfice → preuve → action).
18. Une bonne interface guide le regard — parcours visuel intentionnel.
19. Les composants sont réutilisables (créer un bouton/carte/champ une seule fois).
20. Les états comptent autant que les composants (normal, hover, focus, actif, désactivé, chargement, succès, erreur).
21. Le contenu fait partie du design — un bon design avec un mauvais texte reste une mauvaise expérience.
22. L'interface inspire confiance — pas de dark patterns, faux comptes à rebours, CTA trompeurs.
23. La performance fait partie de l'UX — une interface lente est une mauvaise interface.
24. L'accessibilité n'est pas optionnelle (clavier, lecteur d'écran, contraste, déficiences visuelles/motrices).
25. Concevoir pour l'utilisateur, jamais pour le designer.

## Principes transversaux (les systèmes)

Ne choisis jamais une valeur au hasard. Ces systèmes se retrouvent partout :

- **Échelle typographique** : une seule police (deux max, rôles distincts). Texte courant 16 px, interligne 1,4–1,7, lignes de 50–80 caractères, aligné à gauche. Détail → `references/07-la-typographie.md`.
- **Échelle d'espacement** : 4 · 8 · 12 · 16 · 24 · 32 · 48 · 64 px, réutilisée partout. Proximité = groupe. Détail → `references/08-le-layout-les-grilles-et-les-espacements.md`.
- **Système de couleur** : 1 primaire, 1 secondaire (option), 8–12 gris, + états succès/erreur/avertissement/info. Une couleur = une signification stable. Détail → `references/06-les-couleurs.md`.
- **Hiérarchie visuelle** : taille, contraste, poids, espacement, position, couleur, mouvement — un seul point focal par écran. Détail → `references/05-la-hierarchie-visuelle.md`.
- **Composants** : chaque composant a une fonction unique, des variantes et **tous ses états** dès le départ. Détail → `references/09-les-composants-ui-design-system.md`.

## Index des chapitres — lis la référence avant le travail détaillé

| Tu travailles sur… | Lis d'abord |
|---|---|
| Poser les bases, comprendre l'utilisateur | `references/02-les-fondations-de-lux.md`, `references/03-comprendre-les-utilisateurs.md` |
| Organiser le contenu, menus, catégories, recherche | `references/04-larchitecture-de-linformation.md` |
| Décider où va le regard, point focal, priorités | `references/05-la-hierarchie-visuelle.md` |
| Choisir/valider une palette, couleurs d'état | `references/06-les-couleurs.md` |
| Polices, tailles, interlignes, lisibilité du texte | `references/07-la-typographie.md` |
| Grille, marges, espacements, responsive, breakpoints | `references/08-le-layout-les-grilles-et-les-espacements.md` |
| Construire/auditer un composant générique | `references/09-les-composants-ui-design-system.md` |
| Boutons (texte, types, tailles, états, CTA) | `references/10-les-boutons-buttons.md` |
| Formulaires (champs, labels, validation, erreurs) | `references/11-les-formulaires.md` |
| Navigation (menus, barres, mobile, fil d'Ariane) | `references/12-la-navigation.md` |
| Dashboards, tableaux de bord, KPI, graphiques | `references/13-les-dashboards.md` |
| Landing page, conversion, taux de clic | `references/14-les-landing-pages-et-la-conversion.md` |
| Rédiger textes d'interface, microcopy, ton | `references/15-ux-writing-copywriting.md` |
| Accessibilité (WCAG, clavier, lecteur d'écran) | `references/16-laccessibilite-accessibility.md` |
| Construire un design system complet, tokens | `references/17-construire-un-design-system-professionnel.md` |
| Auditer / critiquer une interface existante | `references/18-audit-ux-ui-professionnel.md` |
| Comprendre le « pourquoi » cognitif d'une règle | `references/19-la-psychologie-cognitive-appliquee-a-lux.md` |
| Lois UX (Hick, Fitts, Miller, Jakob…) | `references/20-les-lois-fondamentales-de-lux.md` |
| Micro-interactions, animation, motion design | `references/21-les-micro-interactions-et-le-motion-design.md` |
| Concevoir une app SaaS (onboarding, settings…) | `references/22-concevoir-une-application-saas-moderne.md` |
| App mobile iOS / Android (patterns natifs) | `references/23-concevoir-une-application-mobile-ios-android.md` |
| Interface conversationnelle / produit IA / chat | `references/24-concevoir-des-interfaces-conversationnelles-et-des.md` |
| Métriques UX & produit (à mesurer, KPI) | `references/26-les-metriques-ux-produit.md` |
| Repérer/éviter les anti-patterns et dark patterns | `references/27-les-anti-patterns-ux-ui.md` |
| Vérification finale complète avant livraison | `references/28-la-checklist-professionnelle-ultime-ux-ui.md` |

`references/00-introduction.md` et `references/01-les-25-regles-fondamentales-dune-bonne-interface.md` donnent la vision d'ensemble et le format du manuel.

Quand une tâche croise plusieurs sujets (ex. une page de checkout = formulaire + boutons + hiérarchie + conversion + accessibilité), lis les chapitres concernés avant de produire, pas après.

## Sources primaires — les livres complets

`references/` est la **synthèse**. Pour une valeur **concrète et exacte** (un code couleur, une police précise, une variante de composant), ou pour un sujet que la synthèse ne couvre pas (surtout le marketing détaillé), va lire l'ouvrage d'origine dans `sources/`. Ils sont volumineux : lis par tranches autour de la partie utile. Voir `sources/INDEX.md` pour le détail.

| Besoin concret | Source à lire |
|---|---|
| Prendre une **palette réelle** + ses codes HSL/hex exacts (13 palettes prêtes) | `sources/color-palettes.md` |
| **Choisir une police** concrète (appairages, poids, licence) | `sources/font-recommendations.md` |
| **Lister les variantes** d'un composant avant de le concevoir | `sources/component-gallery.md` |
| Tactiques visuelles détaillées (Refactoring UI, source des chap. 4–8) | `sources/refactoring-ui-v1.0.2.md` (+ `-wathan-schoger` en second) |
| Fondations d'utilisabilité / tests / conventions (Krug) | `sources/dont-make-me-think.md` |
| Le « pourquoi » cognitif (affordances, feedback, erreurs — Norman) | `sources/design-of-everyday-things.md` |
| **Marketing digital** : SEO, SEA/pub, emailing, réseaux sociaux, funnel, acquisition, analytics | `sources/marketing-digital.md` |

Règle : ne recopie jamais un code couleur ou un nom de police de mémoire — ouvre la source et prends la valeur exacte.

## Checklist rapide avant de livrer

Vérifie systématiquement, et lis `references/28-la-checklist-professionnelle-ultime-ux-ui.md` pour l'audit complet :

- [ ] Un seul objectif clair et une seule action principale visible en < 1 s.
- [ ] Hiérarchie lisible sans couleur (taille/contraste/espace suffisent).
- [ ] Échelles cohérentes : typo, espacement, couleurs, rayons — aucune valeur au hasard.
- [ ] Tous les états des éléments interactifs sont conçus (hover, focus, actif, désactivé, chargement, erreur, succès, vide).
- [ ] Chaque action donne un retour ; les erreurs sont prévenues ou faciles à corriger.
- [ ] Textes explicites (verbes d'action sur les boutons, labels visibles, pas de jargon).
- [ ] Contraste et navigation clavier suffisants (accessibilité).
- [ ] Responsive : la hiérarchie tient sur mobile, pas de débordement horizontal.
- [ ] Aucun dark pattern ; l'interface inspire confiance.
- [ ] Chaque élément présent a une raison d'exister — le reste est supprimé.
