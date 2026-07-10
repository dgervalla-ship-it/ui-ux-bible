# Layout, grille et espacement

## Sommaire

- [Objectif](#section-1)
- [Cas pratique](#section-2)
- [Checklist du chapitre](#section-3)
- [Ce qu’il faut retenir](#section-4)

<a id="section-1"></a>
## Objectif
Construire une interface équilibrée grâce à une grille cohérente, des alignements précis et un système d’espacement réutilisable.

Le layout est le squelette de l’interface.

Si le squelette est mauvais, même les meilleurs composants paraîtront désordonnés.

Pourquoi le layout est-il si important ?

Les utilisateurs ne voient pas consciemment la grille.

En revanche, ils ressentent immédiatement lorsqu’elle est absente.

Une interface mal alignée donne une impression de désordre, même si chaque composant est bien conçu.

Les quatre piliers d’un bon layout

Un layout professionnel repose sur quatre éléments :
1. La grille.
2. Les alignements.
3. Les espacements.
4. Les proportions.

Ces éléments créent un rythme visuel qui rend l’interface agréable à parcourir.

La grille (Grid)

Une grille est un ensemble de colonnes invisibles qui servent de guide pour positionner les éléments.

Elle permet de :

* maintenir des alignements cohérents ;
* faciliter le responsive ;
* accélérer la conception ;
* garantir une interface harmonieuse.

Une grille n’est pas une contrainte, mais un outil d’organisation.

Les colonnes

Sur desktop, les interfaces utilisent souvent une grille de 12 colonnes.

Pourquoi 12 ?

Parce qu’elle se divise facilement :

* 2 colonnes de 6 ;
* 3 colonnes de 4 ;
* 4 colonnes de 3 ;
* 6 colonnes de 2.

Cela offre une grande flexibilité.

Les marges

Une interface ne doit jamais toucher les bords de l’écran.

Prévois des marges généreuses.

Exemple :

┌──────────────────────────────┐
     Contenu principal
└──────────────────────────────┘

Les marges améliorent immédiatement la lisibilité.

Les gouttières (Gutters)

Les gouttières sont les espaces entre les colonnes.

Elles empêchent les éléments de se coller.

Une gouttière constante renforce la cohérence visuelle.

Le rythme des espacements

L’espacement est un langage.

Au lieu de choisir des valeurs au hasard, utilise une échelle.

Exemple :

Niveau	Valeur
XS	4 px
S	8 px
M	16 px
L	24 px
XL	32 px
XXL	48 px
XXXL	64 px

Toute l’interface doit utiliser cette même échelle.

La règle de proximité

Deux éléments proches sont perçus comme liés.

Exemple :

Nom
Prénom
Adresse

Ces champs forment naturellement un groupe.

À l’inverse :

Nom
           Prénom
Adresse

Le groupe est brisé.

La règle de répétition

Les espacements doivent être constants.

Exemple :

Tous les champs d’un formulaire utilisent le même espace vertical.

Tous les titres utilisent le même espace avant et après.

Cette répétition crée une sensation d’ordre.

Les alignements

Les éléments doivent partager des lignes invisibles.

Exemple :

Nom          Email
Téléphone    Ville

Tous les champs commencent au même endroit.

L’œil balaie plus facilement l’interface.

Les tailles

Les composants similaires doivent avoir des dimensions cohérentes.

Par exemple :

Tous les boutons principaux possèdent :

* la même hauteur ;
* les mêmes coins ;
* le même padding.

Même principe pour :

* les cartes ;
* les champs ;
* les badges ;
* les tableaux.

Les proportions

Une interface agréable repose sur des proportions équilibrées.

Un titre énorme au-dessus d’un bouton minuscule crée un déséquilibre.

Les éléments doivent conserver une relation logique entre eux.

Le principe du “contenu avant tout”

L’espace disponible ne doit pas être rempli à tout prix.

L’espace vide est un élément de design.

Il permet :

* d’isoler les groupes ;
* d’améliorer la lecture ;
* de guider le regard.

Une interface dense n’est pas forcément riche.

Elle est souvent simplement plus difficile à utiliser.

Les cartes (Cards)

Chaque carte possède généralement :

* un padding interne constant ;
* un espace régulier entre les éléments ;
* une largeur cohérente ;
* une hauteur adaptée au contenu.

Évite les cartes où chaque élément semble placé au hasard.

Les sections

Une page est découpée en sections.

Chaque section doit être clairement séparée des autres.

Utilise davantage d’espace entre deux sections qu’entre les éléments d’une même section.

Exemple :

Titre
Paragraphe
Bouton
Nouvelle section
Titre
Paragraphe

Le cerveau identifie naturellement les groupes.

Le responsive

Le layout doit s’adapter à toutes les tailles d’écran.

Un bon système responsive :

* conserve la hiérarchie ;
* simplifie la mise en page ;
* évite les défilements horizontaux.

L’objectif n’est pas de reproduire exactement la version desktop, mais d’offrir une expérience équivalente.

Les breakpoints

Au lieu de multiplier les versions, définis quelques points de rupture cohérents.

Exemple :

Format	Largeur indicative
Mobile	≤ 640 px
Tablette	641–1024 px
Desktop	1025–1440 px
Grand écran	> 1440 px

Les valeurs exactes peuvent varier selon le projet.

Les conteneurs

Le contenu principal ne doit pas s’étendre sur toute la largeur d’un très grand écran.

Des lignes trop longues réduisent la lisibilité.

Utilise un conteneur avec une largeur maximale.

Les tableaux

Les colonnes doivent être alignées.

Les espacements doivent être réguliers.

Les lignes doivent rester aérées.

Une table compacte n’est pas forcément plus efficace.

Les dashboards

Un tableau de bord est constitué de blocs.

Chaque bloc possède :

* une largeur cohérente ;
* un alignement précis ;
* un espacement identique aux autres.

Le rythme visuel est essentiel.

Les formulaires

Les formulaires suivent une grille.

Les labels sont alignés.

Les champs possèdent la même largeur lorsque leur fonction est identique.

Les boutons sont alignés avec les champs.

Les erreurs fréquentes

❌ Espacements choisis au hasard.

❌ Colonnes non alignées.

❌ Cartes de tailles incohérentes.

❌ Marges insuffisantes.

❌ Trop d’éléments sur une même ligne.

❌ Contenu collé aux bords.

❌ Utilisation excessive de séparateurs au lieu d’espaces.
<a id="section-2"></a>
## Cas pratique
Imaginons une page de tableau de bord.

Une mauvaise mise en page présenterait :

* des cartes de largeurs différentes sans raison ;
* des marges variables ;
* des boutons non alignés ;
* des espaces irréguliers entre les sections.

Une meilleure mise en page utiliserait :

* une grille de 12 colonnes ;
* un système d’espacement constant ;
* des cartes alignées ;
* des marges généreuses ;
* un rythme vertical régulier.

L’interface paraît immédiatement plus professionnelle, sans avoir modifié le contenu.
<a id="section-3"></a>
## Checklist du chapitre
Avant de valider un layout :

* ☐ Une grille cohérente structure la page.
* ☐ Les colonnes sont correctement alignées.
* ☐ Les marges sont suffisantes.
* ☐ Les espacements suivent une échelle définie.
* ☐ Les composants similaires ont les mêmes dimensions.
* ☐ Les sections sont clairement séparées.
* ☐ Les lignes de texte restent confortables à lire.
* ☐ Le responsive conserve la hiérarchie de l’information.
* ☐ Les conteneurs limitent la largeur sur les grands écrans.
* ☐ L’espace vide est utilisé comme un élément de design.

<a id="section-4"></a>
## Ce qu’il faut retenir
Un bon layout est presque invisible.

Les utilisateurs ne remarquent pas la grille, les alignements ou les espacements. Ils ressentent simplement une impression d’ordre, de clarté et de professionnalisme.

Le layout est la structure qui permet à tous les autres éléments — couleurs, typographie, composants et contenus — de fonctionner ensemble de manière harmonieuse.
