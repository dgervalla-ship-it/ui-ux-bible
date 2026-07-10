# Tableaux de données

Un tableau n’est pas seulement une liste de données. C’est un outil d’analyse et de décision.

## Sommaire

- [Objectif](#section-1)
- [Le rôle d’un tableau](#section-2)
- [Quand utiliser un tableau ?](#section-3)
- [Évite les tableaux pour :](#section-4)
- [Anatomie d’un tableau](#section-5)
- [Les colonnes](#section-6)
- [L’ordre des colonnes](#section-7)
- [Les largeurs](#section-8)
- [Les alignements](#section-9)
- [Les en-têtes](#section-10)
- [Les lignes](#section-11)
- [Les actions](#section-12)
- [Les sélections](#section-13)
- [Les tris](#section-14)
- [Les filtres](#section-15)
- [La recherche](#section-16)
- [La pagination](#section-17)
- [Le défilement](#section-18)
- [Les états](#section-19)
- [Les couleurs](#section-20)
- [Les lignes sélectionnées](#section-21)
- [Les tableaux responsives](#section-22)
- [Les performances](#section-23)
- [Les erreurs fréquentes](#section-24)
- [Cas pratique](#section-25)
- [Checklist du chapitre](#section-26)
- [Ce qu’il faut retenir](#section-27)

<a id="section-1"></a>
## Objectif

Les tableaux sont omniprésents dans les applications professionnelles :

* CRM
* ERP
* SaaS
* Comptabilité
* Gestion de projet
* RH
* Finance
* Administration

Un bon tableau permet de :

* retrouver une information rapidement ;
* comparer plusieurs éléments ;
* filtrer ;
* trier ;
* agir sur plusieurs lignes.

<a id="section-2"></a>
## Le rôle d’un tableau

Un tableau répond principalement à trois besoins :

* consulter ;
* comparer ;
* agir.

Si le tableau ne remplit pas ces trois fonctions, il doit être repensé.

<a id="section-3"></a>
## Quand utiliser un tableau ?

Utilise un tableau lorsque :

* plusieurs objets possèdent les mêmes attributs ;
* l’utilisateur doit comparer des données ;
* des actions sont réalisées sur plusieurs éléments.

Exemples :

✔ Liste des clients

✔ Commandes

✔ Factures

✔ Utilisateurs

✔ Produits

<a id="section-4"></a>
## Évite les tableaux pour :

* raconter une histoire ;
* afficher un seul objet ;
* présenter du contenu éditorial.

Une carte est souvent plus adaptée dans ces cas.

<a id="section-5"></a>
## Anatomie d’un tableau

Un tableau est composé de :

┌───────────────────────────────────────────────┐
│ Barre d'outils                                │
│                                               │
│ Recherche                                     │
│ Filtres                                       │
│ Actions                                       │
├───────────────────────────────────────────────┤
│ En-têtes                                      │
├───────────────────────────────────────────────┤
│ Lignes                                        │
│                                               │
│                                               │
├───────────────────────────────────────────────┤
│ Pagination                                    │
└───────────────────────────────────────────────┘

Chaque partie possède un rôle précis.

<a id="section-6"></a>
## Les colonnes

Une colonne représente toujours un attribut.

Exemple :

| Nom | Email | Société | Statut | Dernière connexion |

Ne mélange jamais plusieurs informations dans une même colonne sans raison.

<a id="section-7"></a>
## L’ordre des colonnes

Les colonnes doivent suivre un ordre logique.

Exemple :

Nom

↓

Entreprise

↓

Statut

↓

Date

↓

Actions

L’information importante apparaît en premier.

<a id="section-8"></a>
## Les largeurs

Toutes les colonnes n’ont pas besoin de la même largeur.

Exemple :

Nom

→ Large

Date

→ Petite

ID

→ Très petite

Description

→ Flexible

Le contenu détermine la largeur.

<a id="section-9"></a>
## Les alignements

Texte

→ Aligné à gauche.

Nombres

→ Alignés à droite.

Dates

→ Toujours alignées de manière cohérente.

Cela facilite énormément la comparaison.

<a id="section-10"></a>
## Les en-têtes

Les en-têtes doivent être immédiatement identifiables.

Ils utilisent généralement :

* une graisse supérieure ;
* un fond légèrement différent ;
* une séparation visuelle.

Les intitulés doivent rester courts.

<a id="section-11"></a>
## Les lignes

Une ligne représente un objet.

Toutes les lignes doivent avoir :

* la même hauteur ;
* les mêmes espacements ;
* le même comportement.

<a id="section-12"></a>
## Les actions

Les actions peuvent apparaître :

### Dans chaque ligne

Exemple :

Modifier

Supprimer

Voir

### Dans un menu

Exemple :

⋮

Lorsque plusieurs actions existent, le menu peut améliorer la lisibilité.

<a id="section-13"></a>
## Les sélections

Lorsque plusieurs lignes peuvent être sélectionnées :

Utiliser une case à cocher.

Exemple :

☐ Client A
☐ Client B
☐ Client C

Une fois sélectionnées :

Afficher les actions de groupe.

<a id="section-14"></a>
## Les tris

Toutes les colonnes importantes doivent être triables.

Le sens du tri doit être visible.

Exemple :

▲

Nom

ou

▼

Date

<a id="section-15"></a>
## Les filtres

Les filtres permettent de réduire rapidement le nombre de résultats.

Ils doivent être :

* visibles ;
* faciles à supprimer ;
* mémorisés lorsque cela est pertinent.

<a id="section-16"></a>
## La recherche

Une recherche est indispensable dès que le volume de données devient important.

Elle doit :

* être rapide ;
* tolérer les fautes ;
* rechercher dans plusieurs colonnes si cela est pertinent.

<a id="section-17"></a>
## La pagination

Lorsque plusieurs centaines d’éléments existent :

Afficher une pagination.

Éviter de charger plusieurs milliers de lignes simultanément.

<a id="section-18"></a>
## Le défilement

Si le tableau est très large :

Le défilement horizontal doit rester utilisable.

Les colonnes importantes peuvent rester figées.

Exemple :

Nom

reste visible.

Les autres colonnes défilent.

<a id="section-19"></a>
## Les états

Un tableau possède plusieurs états.

### Chargement

Afficher :

Skeleton

ou

Indicateur de chargement.

### Vide

Aucun résultat.
Essayez de modifier vos filtres.

Ne jamais afficher une table vide sans explication.

### Erreur

Expliquer :

Pourquoi les données ne sont pas disponibles.

Que faire ensuite.

<a id="section-20"></a>
## Les couleurs

Utiliser la couleur avec parcimonie.

Exemple :

Vert

→ Succès

Rouge

→ Erreur

Orange

→ Avertissement

Le reste du tableau reste neutre.

<a id="section-21"></a>
## Les lignes sélectionnées

Une ligne sélectionnée doit être clairement identifiable.

Exemple :

* fond légèrement coloré ;
* bordure ;
* case cochée.

<a id="section-22"></a>
## Les tableaux responsives

Sur mobile :

Un tableau comportant trop de colonnes devient difficile à utiliser.

Solutions :

* masquer certaines colonnes secondaires ;
* transformer les lignes en cartes ;
* proposer une vue simplifiée.

Ne cherche pas à reproduire exactement le desktop.

<a id="section-23"></a>
## Les performances

Pour les grands volumes :

Utiliser :

* pagination ;
* chargement progressif ;
* virtualisation des lignes lorsque nécessaire.

Une interface rapide contribue à une expérience plus fluide ; vérifier l’effet avec les mesures du produit.

<a id="section-24"></a>
## Les erreurs fréquentes

❌ Trop de colonnes.

❌ Colonnes inutiles.

❌ Largeurs incohérentes.

❌ Aucun tri.

❌ Aucun filtre.

❌ Tableau illisible sur mobile.

❌ Actions dispersées.

❌ Aucune indication de chargement.

❌ États vides oubliés.

<a id="section-25"></a>
## Cas pratique

Imaginons un CRM contenant 25 000 clients.

### Mauvaise conception

* toutes les colonnes visibles ;
* aucune recherche ;
* pas de filtre ;
* pas de tri ;
* actions mélangées.

Retrouver un client devient laborieux.

### Bonne conception

* recherche instantanée ;
* filtres par entreprise, statut et date ;
* tri sur les colonnes principales ;
* pagination ;
* actions regroupées dans un menu ;
* colonnes essentielles figées.

L’utilisateur retrouve rapidement un client.

<a id="section-26"></a>
## Checklist du chapitre

Avant de publier un tableau :

* ☐ Chaque colonne possède une fonction claire.
* ☐ Les informations importantes apparaissent en premier.
* ☐ Les nombres sont alignés à droite.
* ☐ Les textes sont alignés à gauche.
* ☐ Les en-têtes sont visibles.
* ☐ Le tri est disponible lorsque pertinent.
* ☐ Les filtres sont faciles à utiliser.
* ☐ Une recherche est proposée sur les grands ensembles.
* ☐ Les états Chargement, Vide et Erreur sont prévus.
* ☐ Le tableau reste utilisable sur mobile.

<a id="section-27"></a>
## Ce qu’il faut retenir

Un tableau n’est pas un simple conteneur de données.

C’est un outil d’analyse.

Un tableau est plus utile lorsque les utilisateurs trouvent l’information recherchée sans effort inutile ; vérifier ce point avec des tâches représentatives.

La simplicité, la cohérence et les performances sont plus importantes que la quantité d’informations affichées.
