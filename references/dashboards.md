# Dashboards et visualisation

Un bon dashboard ne montre pas toutes les données. Il montre les bonnes données, au bon moment, pour prendre une décision.

## Sommaire

- [Objectif](#section-1)
- [Les principes fondamentaux](#section-2)
- [Une question = un dashboard](#section-3)
- [La hiérarchie d’un dashboard](#section-4)
- [Les KPI (Key Performance Indicators)](#section-5)
- [Combien de KPI afficher ?](#section-6)
- [Les graphiques](#section-7)
- [Choisir le bon graphique](#section-8)
- [Les filtres](#section-9)
- [La période](#section-10)
- [Les comparaisons](#section-11)
- [Les couleurs](#section-12)
- [Les cartes de KPI](#section-13)
- [Les tableaux](#section-14)
- [Les activités récentes](#section-15)
- [Les alertes](#section-16)
- [Les états vides](#section-17)
- [Les performances](#section-18)
- [Le responsive](#section-19)
- [Personnalisation](#section-20)
- [Les erreurs fréquentes](#section-21)
- [Cas pratique](#section-22)
- [Checklist du chapitre](#section-23)
- [Ce qu’il faut retenir](#section-24)

<a id="section-1"></a>
## Objectif

Un dashboard (tableau de bord) transforme des données brutes en informations exploitables.

Il permet à l’utilisateur de :

* surveiller une activité ;
* détecter un problème ;
* identifier une opportunité ;
* prendre une décision rapidement.

Le rôle d’un dashboard n’est pas d’afficher toutes les informations disponibles.

Son rôle est d’aider à agir.

<a id="section-2"></a>
## Les principes fondamentaux

Un bon dashboard est :

* orienté décision ;
* simple ;
* rapide à comprendre ;
* hiérarchisé ;
* personnalisable lorsque nécessaire.

<a id="section-3"></a>
## Une question = un dashboard

Avant de commencer la conception, pose cette question :

Quelle décision ce dashboard doit-il permettre de prendre ?

Exemples :

* Les ventes sont-elles en hausse ?
* Quels projets sont en retard ?
* Quels clients nécessitent une action ?
* Quel est le chiffre d’affaires du mois ?

Si le dashboard ne répond pas clairement à cette question, il doit être repensé.

<a id="section-4"></a>
## La hiérarchie d’un dashboard

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

<a id="section-5"></a>
## Les KPI (Key Performance Indicators)

Les KPI sont les indicateurs principaux.

Ils répondent immédiatement à la question :

Comment se porte l’activité ?

Exemple :

Chiffre d'affaires
125 450 €
+12 %

La valeur est dominante.

La variation apporte le contexte.

<a id="section-6"></a>
## Combien de KPI afficher ?

Limite le nombre de KPI principaux afin de préserver la hiérarchie.

Lorsque trop d’indicateurs sont présentés au même niveau, l’utilisateur ne sait plus où regarder.

Si davantage d’indicateurs sont nécessaires, répartis-les sur plusieurs vues ou sections.

<a id="section-7"></a>
## Les graphiques

Les graphiques servent à montrer des tendances.

Ils répondent à des questions comme :

* Évolution ?
* Comparaison ?
* Répartition ?
* Corrélation ?

Ils ne doivent jamais être décoratifs.

<a id="section-8"></a>
## Choisir le bon graphique

Besoin	Graphique recommandé
Évolution dans le temps	Courbe
Comparaison	Barres
Répartition	Barres empilées ou secteurs (avec modération)
Progression	Jauge ou barre de progression
Distribution	Histogramme

Un mauvais choix de graphique rend les données difficiles à interpréter.

<a id="section-9"></a>
## Les filtres

Les dashboards doivent être interactifs.

Les filtres permettent de répondre à différentes questions sans créer plusieurs écrans.

Exemples :

* période ;
* équipe ;
* pays ;
* produit ;
* client.

Les filtres actifs doivent être visibles.

<a id="section-10"></a>
## La période

Toujours afficher clairement la période analysée.

Exemple :

Janvier 2026
30 derniers jours
Cette année

Une donnée sans contexte temporel perd une grande partie de sa valeur.

<a id="section-11"></a>
## Les comparaisons

Une valeur seule est rarement suffisante.

Préfère :

12 540 €
+18 % par rapport au mois précédent

plutôt que :

12 540 €

Le contexte facilite la décision.

<a id="section-12"></a>
## Les couleurs

Les couleurs renforcent le sens.

Exemple :

* Vert : amélioration.
* Rouge : baisse ou erreur.
* Orange : vigilance.

Ne multiplie pas les couleurs sans nécessité.

<a id="section-13"></a>
## Les cartes de KPI

Une carte KPI contient généralement :

Titre
Valeur
Variation
Période

Évite d’ajouter trop d’informations dans une seule carte.

<a id="section-14"></a>
## Les tableaux

Les tableaux complètent les graphiques.

Le graphique répond à :

Que se passe-t-il ?

Le tableau répond à :

Quels éléments sont concernés ?

Les deux sont complémentaires.

<a id="section-15"></a>
## Les activités récentes

Afficher les dernières actions importantes.

Exemple :

* Nouveau client.
* Paiement reçu.
* Projet terminé.
* Ticket créé.

Ces informations doivent rester secondaires par rapport aux KPI.

<a id="section-16"></a>
## Les alertes

Un dashboard doit attirer l’attention sur les situations importantes.

Exemple :

⚠ 5 paiements en attente
⚠ Stock critique
⚠ Serveur indisponible

Les alertes doivent être limitées aux événements nécessitant une action.

<a id="section-17"></a>
## Les états vides

Si aucune donnée n’est disponible :

Aucune donnée disponible pour cette période.
Essayez de modifier les filtres.

Évite les graphiques vides ou les tableaux sans explication.

<a id="section-18"></a>
## Les performances

Un dashboard doit communiquer son état de chargement et éviter une attente silencieuse.

Pour les gros volumes :

* chargement progressif ;
* mise en cache ;
* rafraîchissement intelligent ;
* indicateurs de chargement.

Une attente prolongée peut réduire la confiance dans l’outil ; afficher sa progression et mesurer son impact.

<a id="section-19"></a>
## Le responsive

Sur mobile :

* les KPI sont empilés verticalement ;
* les graphiques sont simplifiés ;
* les tableaux deviennent des cartes ou des listes ;
* les filtres sont regroupés dans un panneau dédié.

L’objectif est de préserver les informations essentielles.

<a id="section-20"></a>
## Personnalisation

Pour les applications complexes, permettre à l’utilisateur de :

* réorganiser les widgets ;
* masquer certains indicateurs ;
* enregistrer des vues personnalisées.

Cette flexibilité peut soutenir l’efficacité des utilisateurs avancés ; vérifier l’usage réel.

<a id="section-21"></a>
## Les erreurs fréquentes

❌ Trop de KPI.

❌ Graphiques décoratifs.

❌ Absence de contexte temporel.

❌ Couleurs incohérentes.

❌ Données non prioritaires mises en avant.

❌ Trop de graphiques sur un seul écran.

❌ Aucun état vide.

❌ Performances insuffisantes.

<a id="section-22"></a>
## Cas pratique

Imaginons un dashboard commercial.

### Mauvaise conception

* 15 KPI affichés simultanément ;
* 8 graphiques de tailles identiques ;
* aucune hiérarchie ;
* couleurs aléatoires ;
* filtres cachés.

Le responsable commercial ne sait pas où porter son attention.

### Bonne conception

* 4 KPI principaux en haut de page ;
* un graphique d’évolution des ventes ;
* un tableau des meilleurs clients ;
* des alertes sur les objectifs non atteints ;
* des filtres visibles pour changer rapidement de période ou de région.

Il comprend rapidement la situation et peut agir.

<a id="section-23"></a>
## Checklist du chapitre

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

<a id="section-24"></a>
## Ce qu’il faut retenir

Un dashboard n’est pas un rapport.

C’est un outil d’aide à la décision.

Chaque élément affiché doit aider l’utilisateur à répondre à une question, comprendre une situation ou prendre une action.

La qualité d’un dashboard ne se mesure pas au nombre de graphiques qu’il contient, mais à la rapidité avec laquelle un utilisateur peut comprendre ce qui est important.
