# Accessibilité

## Sommaire

- [Références normatives vérifiées](#section-1)

<a id="section-1"></a>
## Références normatives vérifiées

Les seuils ci-dessous viennent de WCAG 2.2 (vérifié le 2026-07-10) : contraste minimal de 4,5:1 pour le texte courant et 3:1 pour le grand texte ; contraste de 3:1 pour les composants d’interface et les graphiques nécessaires. Le critère Target Size (AA) demande 24 × 24 CSS px, avec exceptions ; 44 × 44 CSS px correspond au niveau AAA, pas à une règle AA universelle. Voir [WCAG 2.2](https://www.w3.org/WAI/WCAG22/understanding/) et [Target Size](https://www.w3.org/WAI/WCAG22/Understanding/target-size-minimum).

Pour les applications natives, les recommandations de plateforme sont distinctes : Apple recommande généralement 44 × 44 pt ([HIG Accessibilité](https://developer.apple.com/design/human-interface-guidelines/accessibility)) et Android 48 × 48 dp ([Android Accessibility](https://developer.android.com/guide/topics/ui/accessibility/apps)). Elles ne remplacent pas les critères WCAG d’un produit web.

Vérifier aussi le focus non masqué, l’identification et la suggestion des erreurs, les messages d’état et l’authentification accessible selon les critères WCAG 2.2 ; utiliser des noms accessibles cohérents selon l’[ARIA Authoring Practices Guide](https://www.w3.org/WAI/ARIA/apg/practices/names-and-descriptions/).

Une bonne interface fonctionne pour tout le monde, pas seulement pour les utilisateurs sans limitation.

⸻

Objectif

L’accessibilité consiste à concevoir des interfaces utilisables par le plus grand nombre, quelles que soient les capacités de l’utilisateur.

Cela inclut notamment les personnes ayant :

* une déficience visuelle ;
* une déficience auditive ;
* une limitation motrice ;
* une limitation cognitive ;
* un handicap temporaire ;
* un contexte d’utilisation particulier (forte luminosité, écran de mauvaise qualité, utilisation d’une seule main, etc.).

L’accessibilité améliore également l’expérience de tous les utilisateurs.

⸻

Pourquoi l’accessibilité est importante ?

Une interface inaccessible peut empêcher un utilisateur de :

* acheter ;
* réserver ;
* travailler ;
* communiquer ;
* apprendre.

L’accessibilité n’est donc pas une fonctionnalité optionnelle.

C’est une exigence de qualité.

⸻

Les quatre principes fondamentaux

Les recommandations internationales (WCAG) reposent sur quatre grands principes.

Une interface doit être :

* Perceptible
* Utilisable
* Compréhensible
* Robuste

Ces quatre principes servent de base à toutes les décisions de conception.

⸻

1. Perceptible

L’information doit pouvoir être perçue.

Exemples :

✔ Texte suffisamment contrasté.

✔ Images avec texte alternatif.

✔ Sous-titres pour les vidéos.

✔ Icônes accompagnées d’un texte lorsque nécessaire.

⸻

2. Utilisable

L’interface doit fonctionner avec différents modes d’interaction.

Par exemple :

* souris ;
* clavier ;
* écran tactile ;
* lecteur d’écran.

Une fonctionnalité utilisable uniquement à la souris n’est pas pleinement accessible.

⸻

3. Compréhensible

L’utilisateur doit comprendre :

* le contenu ;
* les actions ;
* les erreurs ;
* les conséquences.

Les interfaces ambiguës sont difficiles à utiliser pour tous.

⸻

4. Robuste

Le code doit être suffisamment standard pour fonctionner avec :

* différents navigateurs ;
* technologies d’assistance ;
* futures évolutions des logiciels.

⸻

Les contrastes

Le contraste est l’un des points les plus importants.

Un texte gris clair sur fond blanc peut sembler élégant, mais il devient illisible pour de nombreux utilisateurs.

Règles :

* privilégier un contraste élevé pour le texte principal ;
* vérifier systématiquement les contrastes lors de la conception.

Ne fais jamais confiance uniquement à ton œil.

⸻

La couleur ne suffit jamais

Ne transmets jamais une information uniquement par la couleur.

❌ Mauvais exemple

Rouge = erreur
Vert = succès

Si un utilisateur ne distingue pas ces couleurs, il perd l’information.

✔ Bon exemple

❌ Erreur
✔ Succès

Ajoute toujours :

* une icône ;
* un texte ;
* ou une forme.

⸻

La taille des zones interactives

Les éléments cliquables doivent être suffisamment grands.

Une cible trop petite est difficile à utiliser sur mobile ou pour une personne ayant une motricité réduite.

Privilégie une zone d’interaction d’environ 44 × 44 px minimum.

⸻

Le focus clavier

Tous les éléments interactifs doivent être accessibles au clavier.

Le focus doit être clairement visible.

Évite de supprimer le contour de focus sans le remplacer par une indication équivalente.

⸻

L’ordre de navigation

Lorsque l’utilisateur appuie sur la touche Tab, le focus doit suivre un ordre logique.

Exemple :

Logo
↓
Navigation
↓
Recherche
↓
Contenu
↓
Pied de page

Un ordre incohérent désoriente les utilisateurs.

⸻

Les formulaires accessibles

Chaque champ possède :

* un label visible ;
* un texte d’aide si nécessaire ;
* un message d’erreur explicite.

Les lecteurs d’écran doivent pouvoir associer correctement ces éléments.

⸻

Les messages d’erreur

Les erreurs doivent être :

* visibles ;
* compréhensibles ;
* localisées.

Exemple :

✔

« L’adresse e-mail est invalide. »

plutôt que :

« Erreur 125 ».

⸻

Les images

Une image informative doit posséder un texte alternatif décrivant son rôle.

Une image purement décorative n’a pas besoin d’une description destinée aux technologies d’assistance.

Le texte alternatif doit décrire l’information utile, pas simplement l’apparence.

⸻

Les icônes

Une icône seule est souvent ambiguë.

Associe-la à un texte lorsque son sens n’est pas évident.

Exemple :

✔

🗑️ Supprimer

plutôt que :

🗑️

⸻

Les animations

Certaines animations peuvent provoquer une gêne.

Évite :

* les clignotements rapides ;
* les animations permanentes ;
* les mouvements excessifs.

Lorsque cela est possible, respecte la préférence système de réduction des animations.

⸻

Les vidéos

Une vidéo doit proposer :

* des sous-titres ;
* une transcription lorsque cela est pertinent ;
* des commandes accessibles.

⸻

Les tableaux

Les tableaux doivent conserver :

* des en-têtes clairement identifiés ;
* une structure logique ;
* des intitulés compréhensibles.

Évite les tableaux utilisés uniquement pour faire de la mise en page.

⸻

Les liens

Le texte d’un lien doit être compréhensible hors contexte.

✔

Télécharger le rapport annuel

❌

Cliquez ici

⸻

Les boutons

Chaque bouton doit posséder un nom explicite.

✔

Créer un projet

❌

OK

⸻

Les notifications

Les notifications importantes doivent rester visibles suffisamment longtemps.

Ne fais pas disparaître automatiquement un message avant que l’utilisateur ait pu le lire.

⸻

Les documents

Les PDF, exports et documents générés doivent eux aussi respecter des règles d’accessibilité :

* titres structurés ;
* texte sélectionnable ;
* ordre logique de lecture.

⸻

Les erreurs fréquentes

❌ Contraste insuffisant.

❌ Focus clavier invisible.

❌ Navigation impossible sans souris.

❌ Images sans texte alternatif.

❌ Icônes sans libellé.

❌ Texte trop petit.

❌ Formulaires sans labels.

❌ Couleur utilisée comme seul indicateur.

❌ Animations excessives.

⸻

Cas pratique

Imaginons un formulaire de paiement.

Mauvaise conception

* labels remplacés par des placeholders ;
* erreurs uniquement signalées en rouge ;
* impossible d’utiliser le clavier ;
* bouton de paiement très petit.

Une partie des utilisateurs rencontre des difficultés importantes.

Bonne conception

* labels visibles ;
* erreurs accompagnées d’un texte explicatif et d’une icône ;
* navigation clavier complète ;
* bouton principal suffisamment grand ;
* contraste élevé.

Le formulaire devient utilisable par un public beaucoup plus large.

⸻

Checklist du chapitre

Avant de publier une interface :

* ☐ Les contrastes sont suffisants.
* ☐ Toutes les actions sont réalisables au clavier.
* ☐ Le focus est clairement visible.
* ☐ Les formulaires possèdent des labels.
* ☐ Les messages d’erreur expliquent la solution.
* ☐ Les images informatives possèdent un texte alternatif.
* ☐ Les liens décrivent leur destination.
* ☐ Les zones interactives sont suffisamment grandes.
* ☐ Les animations restent discrètes et peuvent être réduites.
* ☐ Les informations ne reposent jamais uniquement sur la couleur.

⸻

Ce qu’il faut retenir

L’accessibilité ne consiste pas à créer une version spéciale d’un produit.

Elle consiste à créer un meilleur produit pour tous.

Une interface accessible est généralement :

* plus claire ;
* plus simple ;
* plus robuste ;
* plus agréable à utiliser.

C’est pourquoi l’accessibilité doit être prise en compte dès les premières étapes de la conception, et non ajoutée à la fin du projet.

⸻

Notes d’application
