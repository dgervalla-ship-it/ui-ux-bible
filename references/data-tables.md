# Tableaux de données

Un tableau n’est pas seulement une liste de données. C’est un outil d’analyse et de décision.

⸻

Objectif

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

⸻

Le rôle d’un tableau

Un tableau répond principalement à trois besoins :

* consulter ;
* comparer ;
* agir.

Si le tableau ne remplit pas ces trois fonctions, il doit être repensé.

⸻

Quand utiliser un tableau ?

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

⸻

Évite les tableaux pour :

* raconter une histoire ;
* afficher un seul objet ;
* présenter du contenu éditorial.

Une carte est souvent plus adaptée dans ces cas.

⸻

Anatomie d’un tableau

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

⸻

Les colonnes

Une colonne représente toujours un attribut.

Exemple :

| Nom | Email | Société | Statut | Dernière connexion |

Ne mélange jamais plusieurs informations dans une même colonne sans raison.

⸻

L’ordre des colonnes

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

⸻

Les largeurs

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

⸻

Les alignements

Texte

→ Aligné à gauche.

Nombres

→ Alignés à droite.

Dates

→ Toujours alignées de manière cohérente.

Cela facilite énormément la comparaison.

⸻

Les en-têtes

Les en-têtes doivent être immédiatement identifiables.

Ils utilisent généralement :

* une graisse supérieure ;
* un fond légèrement différent ;
* une séparation visuelle.

Les intitulés doivent rester courts.

⸻

Les lignes

Une ligne représente un objet.

Toutes les lignes doivent avoir :

* la même hauteur ;
* les mêmes espacements ;
* le même comportement.

⸻

Les actions

Les actions peuvent apparaître :

Dans chaque ligne

Exemple :

Modifier

Supprimer

Voir

⸻

Dans un menu

Exemple :

⋮

Lorsque plusieurs actions existent, le menu améliore la lisibilité.

⸻

Les sélections

Lorsque plusieurs lignes peuvent être sélectionnées :

Utiliser une case à cocher.

Exemple :

☐ Client A
☐ Client B
☐ Client C

Une fois sélectionnées :

Afficher les actions de groupe.

⸻

Les tris

Toutes les colonnes importantes doivent être triables.

Le sens du tri doit être visible.

Exemple :

▲

Nom

ou

▼

Date

⸻

Les filtres

Les filtres permettent de réduire rapidement le nombre de résultats.

Ils doivent être :

* visibles ;
* faciles à supprimer ;
* mémorisés lorsque cela est pertinent.

⸻

La recherche

Une recherche est indispensable dès que le volume de données devient important.

Elle doit :

* être rapide ;
* tolérer les fautes ;
* rechercher dans plusieurs colonnes si cela est pertinent.

⸻

La pagination

Lorsque plusieurs centaines d’éléments existent :

Afficher une pagination.

Éviter de charger plusieurs milliers de lignes simultanément.

⸻

Le défilement

Si le tableau est très large :

Le défilement horizontal doit rester utilisable.

Les colonnes importantes peuvent rester figées.

Exemple :

Nom

reste visible.

Les autres colonnes défilent.

⸻

Les états

Un tableau possède plusieurs états.

⸻

Chargement

Afficher :

Skeleton

ou

Indicateur de chargement.

⸻

Vide

Aucun résultat.
Essayez de modifier vos filtres.

Ne jamais afficher une table vide sans explication.

⸻

Erreur

Expliquer :

Pourquoi les données ne sont pas disponibles.

Que faire ensuite.

⸻

Les couleurs

Utiliser la couleur avec parcimonie.

Exemple :

Vert

→ Succès

Rouge

→ Erreur

Orange

→ Avertissement

Le reste du tableau reste neutre.

⸻

Les lignes sélectionnées

Une ligne sélectionnée doit être clairement identifiable.

Exemple :

* fond légèrement coloré ;
* bordure ;
* case cochée.

⸻

Les tableaux responsives

Sur mobile :

Un tableau de 15 colonnes devient inutilisable.

Solutions :

* masquer certaines colonnes secondaires ;
* transformer les lignes en cartes ;
* proposer une vue simplifiée.

Ne cherche pas à reproduire exactement le desktop.

⸻

Les performances

Pour les grands volumes :

Utiliser :

* pagination ;
* chargement progressif ;
* virtualisation des lignes lorsque nécessaire.

Une interface rapide améliore directement l’expérience utilisateur.

⸻

Les erreurs fréquentes

❌ Trop de colonnes.

❌ Colonnes inutiles.

❌ Largeurs incohérentes.

❌ Aucun tri.

❌ Aucun filtre.

❌ Tableau illisible sur mobile.

❌ Actions dispersées.

❌ Aucune indication de chargement.

❌ États vides oubliés.

⸻

Cas pratique

Imaginons un CRM contenant 25 000 clients.

Mauvaise conception

* toutes les colonnes visibles ;
* aucune recherche ;
* pas de filtre ;
* pas de tri ;
* actions mélangées.

Retrouver un client prend plusieurs minutes.

Bonne conception

* recherche instantanée ;
* filtres par entreprise, statut et date ;
* tri sur les colonnes principales ;
* pagination ;
* actions regroupées dans un menu ;
* colonnes essentielles figées.

L’utilisateur retrouve un client en quelques secondes.

⸻

Checklist du chapitre

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

⸻

Ce qu’il faut retenir

Un tableau n’est pas un simple conteneur de données.

C’est un outil d’analyse.

Plus les utilisateurs trouvent rapidement l’information qu’ils recherchent, plus le tableau est efficace.

La simplicité, la cohérence et les performances sont plus importantes que la quantité d’informations affichées.

⸻

Notes d’application
