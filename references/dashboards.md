# Dashboards et visualisation

Un bon dashboard ne montre pas toutes les données. Il montre les bonnes données, au bon moment, pour prendre une décision.

⸻

Objectif

Un dashboard (tableau de bord) transforme des données brutes en informations exploitables.

Il permet à l’utilisateur de :

* surveiller une activité ;
* détecter un problème ;
* identifier une opportunité ;
* prendre une décision rapidement.

Le rôle d’un dashboard n’est pas d’afficher toutes les informations disponibles.

Son rôle est d’aider à agir.

⸻

Les principes fondamentaux

Un bon dashboard est :

* orienté décision ;
* simple ;
* rapide à comprendre ;
* hiérarchisé ;
* personnalisable lorsque nécessaire.

L’utilisateur doit comprendre l’état du système en moins de 10 secondes.

⸻

Une question = un dashboard

Avant de commencer la conception, pose cette question :

Quelle décision ce dashboard doit-il permettre de prendre ?

Exemples :

* Les ventes sont-elles en hausse ?
* Quels projets sont en retard ?
* Quels clients nécessitent une action ?
* Quel est le chiffre d’affaires du mois ?

Si le dashboard ne répond pas clairement à cette question, il doit être repensé.

⸻

La hiérarchie d’un dashboard

Un dashboard suit généralement cette structure :

┌────────────────────────────────────────────┐
│ Titre + période + filtres                  │
├────────────────────────────────────────────┤
│ KPI principaux                             │
├────────────────────────────────────────────┤
│ Graphiques                                 │
├────────────────────────────────────────────┤
│ Tableaux                                  │
├────────────────────────────────────────────┤
│ Activités récentes                         │
└────────────────────────────────────────────┘

Le regard suit naturellement cette progression.

⸻

Les KPI (Key Performance Indicators)

Les KPI sont les indicateurs principaux.

Ils répondent immédiatement à la question :

Comment se porte l’activité ?

Exemple :

Chiffre d'affaires
125 450 €
+12 %

La valeur est dominante.

La variation apporte le contexte.

⸻

Combien de KPI afficher ?

Entre 3 et 6 KPI principaux suffisent dans la majorité des cas.

Au-delà, l’utilisateur ne sait plus où regarder.

Si davantage d’indicateurs sont nécessaires, répartis-les sur plusieurs vues ou sections.

⸻

Les graphiques

Les graphiques servent à montrer des tendances.

Ils répondent à des questions comme :

* Évolution ?
* Comparaison ?
* Répartition ?
* Corrélation ?

Ils ne doivent jamais être décoratifs.

⸻

Choisir le bon graphique

Besoin	Graphique recommandé
Évolution dans le temps	Courbe
Comparaison	Barres
Répartition	Barres empilées ou secteurs (avec modération)
Progression	Jauge ou barre de progression
Distribution	Histogramme

Un mauvais choix de graphique rend les données difficiles à interpréter.

⸻

Les filtres

Les dashboards doivent être interactifs.

Les filtres permettent de répondre à différentes questions sans créer plusieurs écrans.

Exemples :

* période ;
* équipe ;
* pays ;
* produit ;
* client.

Les filtres actifs doivent être visibles.

⸻

La période

Toujours afficher clairement la période analysée.

Exemple :

Janvier 2026
30 derniers jours
Cette année

Une donnée sans contexte temporel perd une grande partie de sa valeur.

⸻

Les comparaisons

Une valeur seule est rarement suffisante.

Préfère :

12 540 €
+18 % par rapport au mois précédent

plutôt que :

12 540 €

Le contexte facilite la décision.

⸻

Les couleurs

Les couleurs renforcent le sens.

Exemple :

* Vert : amélioration.
* Rouge : baisse ou erreur.
* Orange : vigilance.

Ne multiplie pas les couleurs sans nécessité.

⸻

Les cartes de KPI

Une carte KPI contient généralement :

Titre
Valeur
Variation
Période

Évite d’ajouter trop d’informations dans une seule carte.

⸻

Les tableaux

Les tableaux complètent les graphiques.

Le graphique répond à :

Que se passe-t-il ?

Le tableau répond à :

Quels éléments sont concernés ?

Les deux sont complémentaires.

⸻

Les activités récentes

Afficher les dernières actions importantes.

Exemple :

* Nouveau client.
* Paiement reçu.
* Projet terminé.
* Ticket créé.

Ces informations doivent rester secondaires par rapport aux KPI.

⸻

Les alertes

Un dashboard doit attirer l’attention sur les situations importantes.

Exemple :

⚠ 5 paiements en attente
⚠ Stock critique
⚠ Serveur indisponible

Les alertes doivent être limitées aux événements nécessitant une action.

⸻

Les états vides

Si aucune donnée n’est disponible :

Aucune donnée disponible pour cette période.
Essayez de modifier les filtres.

Évite les graphiques vides ou les tableaux sans explication.

⸻

Les performances

Un dashboard doit s’afficher rapidement.

Pour les gros volumes :

* chargement progressif ;
* mise en cache ;
* rafraîchissement intelligent ;
* indicateurs de chargement.

Une attente prolongée réduit la confiance dans l’outil.

⸻

Le responsive

Sur mobile :

* les KPI sont empilés verticalement ;
* les graphiques sont simplifiés ;
* les tableaux deviennent des cartes ou des listes ;
* les filtres sont regroupés dans un panneau dédié.

L’objectif est de préserver les informations essentielles.

⸻

Personnalisation

Pour les applications complexes, permettre à l’utilisateur de :

* réorganiser les widgets ;
* masquer certains indicateurs ;
* enregistrer des vues personnalisées.

Cette flexibilité améliore l’efficacité pour les utilisateurs avancés.

⸻

Les erreurs fréquentes

❌ Trop de KPI.

❌ Graphiques décoratifs.

❌ Absence de contexte temporel.

❌ Couleurs incohérentes.

❌ Données non prioritaires mises en avant.

❌ Trop de graphiques sur un seul écran.

❌ Aucun état vide.

❌ Performances insuffisantes.

⸻

Cas pratique

Imaginons un dashboard commercial.

Mauvaise conception

* 15 KPI affichés simultanément ;
* 8 graphiques de tailles identiques ;
* aucune hiérarchie ;
* couleurs aléatoires ;
* filtres cachés.

Le responsable commercial ne sait pas où porter son attention.

Bonne conception

* 4 KPI principaux en haut de page ;
* un graphique d’évolution des ventes ;
* un tableau des meilleurs clients ;
* des alertes sur les objectifs non atteints ;
* des filtres visibles pour changer rapidement de période ou de région.

En quelques secondes, il comprend la situation et peut agir.

⸻

Checklist du chapitre

Avant de publier un dashboard :

* ☐ Une question métier claire guide la conception.
* ☐ Les KPI principaux sont visibles immédiatement.
* ☐ Les graphiques répondent à un besoin précis.
* ☐ Les données sont contextualisées (période, comparaison).
* ☐ Les filtres sont accessibles et compréhensibles.
* ☐ Les alertes mettent en avant les situations critiques.
* ☐ Les tableaux complètent les graphiques sans les dupliquer.
* ☐ Les états de chargement, d’erreur et d’absence de données sont prévus.
* ☐ Le dashboard reste lisible sur mobile.
* ☐ Les performances permettent une consultation fluide.

⸻

Ce qu’il faut retenir

Un dashboard n’est pas un rapport.

C’est un outil d’aide à la décision.

Chaque élément affiché doit aider l’utilisateur à répondre à une question, comprendre une situation ou prendre une action.

La qualité d’un dashboard ne se mesure pas au nombre de graphiques qu’il contient, mais à la rapidité avec laquelle un utilisateur peut comprendre ce qui est important.

⸻

Notes d’application

À partir du chapitre 15, nous allons entrer dans une partie très influencée par Le Grand Livre du Marketing Digital. Nous aborderons les Landing Pages, les tunnels de conversion, le copywriting, les appels à l’action (CTA), la preuve sociale, les formulaires de conversion et les stratégies d’optimisation. Cette section reliera directement les principes d’UX à ceux du marketing afin de concevoir des interfaces qui sont non seulement agréables à utiliser, mais aussi efficaces pour atteindre des objectifs métier.
