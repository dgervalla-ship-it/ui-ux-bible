# Cartes

Les cartes permettent d’organiser l’information en unités simples, lisibles et réutilisables.

## Sommaire

- [Objectif](#section-1)
- [Pourquoi utiliser des cartes ?](#section-2)
- [Les principes fondamentaux](#section-3)
- [Une carte = une information principale](#section-4)
- [Anatomie d’une carte](#section-5)
- [Le titre](#section-6)
- [L’image](#section-7)
- [La description](#section-8)
- [Les métadonnées](#section-9)
- [Les actions](#section-10)
- [Les espacements](#section-11)
- [Les dimensions](#section-12)
- [Les bordures](#section-13)
- [Les ombres](#section-14)
- [Les coins](#section-15)
- [Les états](#section-16)
- [Les cartes cliquables](#section-17)
- [Les cartes de statistiques](#section-18)
- [Les cartes de profil](#section-19)
- [Les cartes produit](#section-20)
- [Les cartes d’article](#section-21)
- [Les cartes de tableau de bord](#section-22)
- [Les cartes vides](#section-23)
- [Les erreurs fréquentes](#section-24)
- [Cas pratique](#section-25)
- [Checklist du chapitre](#section-26)
- [Ce qu’il faut retenir](#section-27)

<a id="section-1"></a>
## Objectif

Les cartes sont aujourd’hui l’un des composants les plus utilisés dans les interfaces modernes.

On les retrouve dans :

* les dashboards ;
* les e-commerces ;
* les CRM ;
* les applications SaaS ;
* les blogs ;
* les réseaux sociaux ;
* les applications mobiles.

Une carte bien conçue permet à l’utilisateur de comprendre rapidement une information et d’agir dessus.

<a id="section-2"></a>
## Pourquoi utiliser des cartes ?

Une carte représente une seule entité.

Par exemple :

* un produit ;
* un utilisateur ;
* un projet ;
* une facture ;
* un article ;
* une tâche.

Une carte ne doit jamais représenter plusieurs objets différents.

<a id="section-3"></a>
## Les principes fondamentaux

Une bonne carte est :

* autonome ;
* cohérente ;
* lisible ;
* réutilisable ;
* facilement comparable aux autres cartes.

<a id="section-4"></a>
## Une carte = une information principale

Chaque carte possède une information dominante.

Exemple :

Carte Produit

→ Nom du produit

Carte Employé

→ Nom de l’employé

Carte Projet

→ Nom du projet

Tout le reste est secondaire.

<a id="section-5"></a>
## Anatomie d’une carte

Une carte est généralement composée de :

┌─────────────────────────────┐
│ Image / Illustration         │
│                              │
│ Titre                        │
│ Description                  │
│                              │
│ Informations secondaires     │
│                              │
│ Action principale            │
└─────────────────────────────┘

Toutes les cartes d’une même famille doivent partager cette structure.

<a id="section-6"></a>
## Le titre

Le titre est toujours l’information la plus visible.

Il doit être :

* court ;
* clair ;
* unique.

Exemple :

✔ MacBook Air M3

✔ Projet Apollo

✔ Jean Dupont

Évite les titres trop longs qui cassent la grille.

<a id="section-7"></a>
## L’image

Toutes les cartes n’ont pas besoin d’image.

Ajoute une image uniquement lorsqu’elle apporte une information.

Exemples :

✔ Produit

✔ Profil

✔ Immobilier

En revanche, une facture ou une notification n’ont généralement pas besoin d’image.

<a id="section-8"></a>
## La description

La description complète le titre.

Elle répond à la question :

Pourquoi cette carte est-elle importante ?

Elle doit rester courte.

Deux ou trois lignes suffisent dans la majorité des cas.

<a id="section-9"></a>
## Les métadonnées

Les métadonnées apportent du contexte.

Exemple :

Projet

Créé le 12 juin
12 tâches
3 collaborateurs

Produit

En stock
Livraison gratuite
★★★★★

Les métadonnées doivent être discrètes.

<a id="section-10"></a>
## Les actions

Une carte contient généralement :

* une action principale ;
* éventuellement des actions secondaires.

Exemple :

Modifier

Les autres actions :

Partager
Dupliquer
Archiver

peuvent être regroupées dans un menu.

<a id="section-11"></a>
## Les espacements

Toutes les cartes utilisent les mêmes marges internes.

Exemple :

24 px
Titre
16 px
Description
24 px
Bouton

Le rythme vertical doit être constant.

<a id="section-12"></a>
## Les dimensions

Les cartes similaires doivent avoir :

* la même largeur ;
* la même hauteur lorsque cela facilite la comparaison.

Dans une grille de produits, des cartes de hauteurs très différentes rendent la lecture plus difficile.

<a id="section-13"></a>
## Les bordures

Les bordures servent à séparer les cartes.

Elles doivent rester discrètes.

Évite les contours épais qui attirent inutilement l’attention.

<a id="section-14"></a>
## Les ombres

Les ombres créent une impression de profondeur.

Utilise-les avec modération.

Une légère ombre suffit généralement.

Les ombres très marquées donnent rapidement une impression datée.

<a id="section-15"></a>
## Les coins

Le rayon des coins doit être identique dans tout le Design System.

Exemple :

Toutes les cartes utilisent :

* 8 px

ou

* 12 px

Pas un mélange de plusieurs valeurs.

<a id="section-16"></a>
## Les états

Une carte interactive possède plusieurs états.

### Normal

État par défaut.

### Hover

La carte indique qu’elle est interactive.

Exemple :

* légère élévation ;
* légère ombre ;
* contour accentué.

### Focus

Visible lors de la navigation clavier.

Le focus doit rester clairement identifiable.

### Active

La carte fournit un état visible après le clic.

### Selected

Une carte sélectionnée doit être identifiable.

Exemple :

* contour coloré ;
* fond légèrement différent ;
* coche de validation.

<a id="section-17"></a>
## Les cartes cliquables

Deux approches sont possibles :

### Toute la carte est cliquable

Approche adaptée :

* catalogue ;
* galerie ;
* tableau de bord.

### Seul un bouton est cliquable

Approche adaptée :

* formulaires ;
* tableaux ;
* interfaces complexes.

Évite de mélanger les deux sans distinction.

<a id="section-18"></a>
## Les cartes de statistiques

Exemple :

Chiffre d'affaires
125 000 €
+12 %

La valeur principale domine.

L’évolution est secondaire.

Les explications sont discrètes.

<a id="section-19"></a>
## Les cartes de profil

Structure classique :

Photo
Nom
Fonction
Entreprise
Actions

Le nom est toujours l’information principale.

<a id="section-20"></a>
## Les cartes produit

Structure recommandée :

Image
Nom
Prix
Description courte
Évaluation
Ajouter au panier

Le prix doit être immédiatement visible.

<a id="section-21"></a>
## Les cartes d’article

Structure :

Image
Titre
Résumé
Auteur
Date
Temps de lecture

Le titre attire d’abord le regard.

<a id="section-22"></a>
## Les cartes de tableau de bord

Une carte de KPI contient généralement :

Titre
Valeur
Variation
Période

La valeur est l’élément dominant.

<a id="section-23"></a>
## Les cartes vides

Lorsqu’aucune donnée n’est disponible :

Aucun projet
Créez votre premier projet.
[Créer]

Une carte vide doit toujours guider l’utilisateur.

<a id="section-24"></a>
## Les erreurs fréquentes

❌ Trop d’informations.

❌ Plusieurs CTA principaux.

❌ Images inutiles.

❌ Espacements différents selon les cartes.

❌ Titres trop longs.

❌ Cartes de hauteurs incohérentes.

❌ Métadonnées plus visibles que le contenu principal.

❌ Ombres excessives.

<a id="section-25"></a>
## Cas pratique

Imaginons une grille de projets.

### Mauvaise conception

* certaines cartes mesurent 200 px de haut, d’autres 450 px ;
* les boutons changent de position ;
* les titres s’étalent sur cinq lignes ;
* les actions principales ne sont pas alignées.

Le balayage visuel devient difficile.

### Bonne conception

Toutes les cartes :

* utilisent la même grille ;
* possèdent les mêmes marges internes ;
* présentent les informations dans le même ordre ;
* alignent leurs boutons au même niveau.

L’utilisateur doit pouvoir comparer les projets rapidement.

<a id="section-26"></a>
## Checklist du chapitre

Avant de publier une carte :

* ☐ La carte représente une seule entité.
* ☐ Le titre est immédiatement identifiable.
* ☐ Les informations suivent une hiérarchie claire.
* ☐ Les espacements sont constants.
* ☐ Les actions principales sont faciles à trouver.
* ☐ Les métadonnées restent secondaires.
* ☐ Les états Hover, Focus et Selected sont définis.
* ☐ Les cartes similaires possèdent les mêmes dimensions.
* ☐ Les images apportent une véritable valeur.
* ☐ Les cartes restent lisibles sur mobile.

<a id="section-27"></a>
## Ce qu’il faut retenir

Une carte est une unité d’information.

Elle doit permettre à l’utilisateur de comprendre rapidement :

* de quoi il s’agit ;
* pourquoi c’est important ;
* ce qu’il peut faire ensuite.

Un Design System qui définit clairement les règles des cartes favorise la cohérence, la lisibilité et l’évolution des interfaces.
