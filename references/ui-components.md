# Composants génériques

Les composants sont les briques qui construisent une interface. Leur qualité détermine la qualité du produit.

⸻

Objectif

Construire une bibliothèque de composants cohérente, réutilisable et évolutive.

Un Design System n’est pas une collection d’écrans.

C’est une collection de composants.

Chaque composant doit :

* résoudre un problème précis ;
* être réutilisable ;
* être accessible ;
* être cohérent ;
* être documenté.

⸻

Qu’est-ce qu’un composant ?

Un composant est un élément autonome possédant :

* une fonction ;
* une apparence ;
* un comportement ;
* plusieurs états.

Exemples :

* Bouton
* Champ de saisie
* Carte
* Badge
* Modal
* Tooltip
* Tableau
* Dropdown

⸻

Les principes fondamentaux

Un bon composant est :

Simple

Une seule fonction.

Exemple :

Un bouton sert à déclencher une action.

Il ne sert pas à ouvrir un menu, afficher une notification et modifier des données simultanément.

⸻

Prévisible

Le même composant se comporte toujours de la même manière.

Un bouton primaire doit agir comme tous les autres boutons primaires.

⸻

Réutilisable

Le composant ne dépend pas d’un écran particulier.

Il peut être utilisé partout.

⸻

Accessible

Il fonctionne :

* au clavier ;
* avec un lecteur d’écran ;
* sur mobile ;
* avec différents contrastes.

⸻

Anatomie d’un composant

Chaque composant possède :

Nom
Description
Utilisation
Variantes
États
Accessibilité
Bonnes pratiques
Erreurs fréquentes
Exemples

Cette documentation doit accompagner tous les composants du Design System.

⸻

Les états

Chaque composant interactif possède au minimum les états suivants :

État	Description
Default	État normal
Hover	Survol
Focus	Navigation clavier
Active	Pendant le clic
Disabled	Désactivé
Loading	Chargement
Success	Succès (si applicable)
Error	Erreur (si applicable)

Tous ces états doivent être conçus dès le départ.

⸻

Les variantes

Un composant peut avoir plusieurs variantes.

Prenons l’exemple du bouton.

Bouton primaire

Action principale.

Un seul par écran dans la majorité des cas.

⸻

Bouton secondaire

Action moins importante.

Visuellement plus discret.

⸻

Bouton tertiaire

Action peu importante.

Souvent sous forme de lien.

⸻

Bouton destructif

Actions irréversibles.

Exemple :

Supprimer un compte.

Il utilise la couleur d’erreur.

⸻

Les tailles

Chaque composant possède généralement plusieurs tailles.

Exemple :

Taille	Utilisation
Small	Tableaux
Medium	Taille standard
Large	Landing pages

Évite les tailles arbitraires.

⸻

Les icônes

Les icônes servent à renforcer la compréhension.

Elles ne remplacent pas le texte.

✔️

📥 Télécharger

❌

📥

Sans texte, le sens devient ambigu.

⸻

Le bouton

Objectif

Déclencher une action.

⸻

Bonnes pratiques

✔ Une seule action principale.

✔ Texte court.

✔ Verbe d’action.

Exemples :

Créer

Enregistrer

Supprimer

Payer

Continuer

⸻

Mauvais exemples

Clique ici

OK

Continuer

Valider

Ces intitulés manquent souvent de contexte.

⸻

États

* Normal
* Hover
* Focus
* Disabled
* Loading

⸻

Checklist

☐ Taille suffisante

☐ Contraste élevé

☐ Verbe d’action

☐ Accessible au clavier

☐ Zone de clic confortable

⸻

Le champ de saisie

Objectif

Permettre la saisie d’informations.

⸻

Anatomie

Label
Champ
Texte d'aide
Erreur éventuelle

⸻

Bonnes pratiques

Toujours afficher le label.

Ne jamais utiliser le placeholder comme unique indication.

⸻

États

* Vide
* Rempli
* Focus
* Désactivé
* Erreur
* Succès

⸻

Mauvais exemple

Nom

Placeholder uniquement.

Lorsque l’utilisateur commence à écrire, il oublie ce qu’il devait saisir.

⸻

Les cartes (Cards)

Les cartes regroupent plusieurs informations.

Une carte contient généralement :

Image
Titre
Description
Métadonnées
CTA

⸻

Règles

Les espacements restent constants.

Le contenu suit une hiérarchie claire.

Les cartes similaires possèdent les mêmes dimensions.

⸻

Les badges

Les badges servent à afficher :

* un statut ;
* une catégorie ;
* une priorité.

Ils ne doivent jamais être utilisés comme bouton.

⸻

Les alertes

Une alerte communique une information importante.

Types :

* Succès
* Erreur
* Avertissement
* Information

Chaque type possède :

* une couleur dédiée ;
* une icône cohérente ;
* un titre clair ;
* un message concis.

⸻

Les modales

Une modale interrompt l’utilisateur.

Elle doit être utilisée avec modération.

⸻

Une modale contient :

Titre

Description

Action principale

Action secondaire

Fermeture

⸻

Mauvais usages

❌ Publicité

❌ Confirmation inutile

❌ Tutoriel obligatoire

⸻

Les tooltips

Le tooltip explique.

Il ne remplace jamais un texte important.

Il disparaît lorsque l’utilisateur n’en a plus besoin.

⸻

Les dropdowns

Un menu déroulant est utile lorsque :

* la liste est relativement courte ;
* un seul choix est possible.

Évite les listes de plusieurs centaines d’éléments.

⸻

Les accordéons

Ils servent à réduire la quantité d’informations visibles.

Ils ne doivent pas masquer des informations essentielles.

⸻

Les tableaux

Un tableau doit :

* être lisible ;
* permettre le tri si nécessaire ;
* proposer une recherche lorsque le volume augmente ;
* rester responsive.

⸻

Les onglets (Tabs)

Les onglets permettent de changer de contexte sans quitter la page.

Ils doivent être :

* peu nombreux ;
* clairement nommés ;
* visuellement distincts.

⸻

Les menus

Un menu présente les actions disponibles.

Les actions les plus fréquentes apparaissent en premier.

Les actions destructives sont isolées.

⸻

Les composants vides (Empty States)

Une interface vide doit expliquer :

Pourquoi elle est vide.

Que faire ensuite.

Exemple :

Aucun projet
Créez votre premier projet pour commencer.
[Créer un projet]

⸻

Les chargements (Loading)

Pendant une attente :

Afficher un indicateur.

Mieux encore :

Afficher un squelette (Skeleton).

Le Skeleton réduit la perception du temps d’attente.

⸻

Les erreurs fréquentes

❌ Un même composant possède plusieurs styles.

❌ Les boutons changent selon les pages.

❌ Les formulaires utilisent des labels différents.

❌ Les cartes changent de taille.

❌ Les modales sont utilisées partout.

❌ Les états Hover ou Focus sont oubliés.

❌ Les composants ne sont pas documentés.

⸻

Cas pratique

Imaginons un bouton « Enregistrer ».

Une mauvaise implémentation changerait sa couleur, sa taille ou son comportement selon les écrans.

Une bonne implémentation définirait un composant unique :

* hauteur fixe ;
* paddings constants ;
* mêmes couleurs ;
* mêmes états ;
* même comportement.

Tous les écrans utiliseraient cette version.

Le résultat est une interface plus cohérente, plus simple à maintenir et plus facile à utiliser.

⸻

Checklist du chapitre

Avant de valider un composant :

* ☐ Sa fonction est clairement définie.
* ☐ Il possède un nom unique dans le Design System.
* ☐ Toutes ses variantes sont documentées.
* ☐ Tous ses états sont conçus.
* ☐ Il est accessible au clavier.
* ☐ Son contraste respecte les règles d’accessibilité.
* ☐ Les espacements sont cohérents.
* ☐ Il est réutilisable sur plusieurs écrans.
* ☐ Les icônes complètent le texte sans le remplacer.
* ☐ Son comportement est identique dans toute l’application.

⸻

Ce qu’il faut retenir

Les utilisateurs ne perçoivent pas une interface comme un assemblage de pages.

Ils interagissent avec des composants.

Lorsque ces composants sont cohérents, prévisibles et bien documentés, l’expérience utilisateur devient plus fluide et le développement plus rapide.

Un excellent Design System n’est pas seulement une bibliothèque graphique : c’est un langage commun entre designers, développeurs et équipes produit.

⸻

Notes d’application

À partir du prochain chapitre, nous entrerons dans une approche beaucoup plus détaillée : un chapitre complet sera consacré à chaque famille de composants (boutons, formulaires, navigation, tableaux, modales, cartes, etc.), avec des dizaines de règles, des cas d’usage, des variantes et des exemples. L’objectif est que ce guide puisse servir de documentation de référence pour concevoir ou auditer une interface professionnelle.
