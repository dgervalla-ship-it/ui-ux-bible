# Boutons et CTA

Le bouton est le composant le plus important d’une interface. C’est lui qui transforme une intention en action.

## Sommaire

- [Objectif](#section-1)
- [Qu’est-ce qu’un bouton ?](#section-2)
- [Anatomie d’un bouton](#section-3)
- [Les caractéristiques d’un bon bouton](#section-4)
- [Le texte du bouton](#section-5)
- [Les types de boutons](#section-6)
- [Une seule action principale](#section-7)
- [Les dimensions](#section-8)
- [Les espacements internes](#section-9)
- [Les icônes](#section-10)
- [Les états](#section-11)
- [Les couleurs](#section-12)
- [Les coins](#section-13)
- [Les animations](#section-14)
- [Les boutons dans les formulaires](#section-15)
- [Les boutons dans les modales](#section-16)
- [Les boutons avec confirmation](#section-17)
- [Les erreurs fréquentes](#section-18)
- [Cas pratique](#section-19)
- [Checklist du chapitre](#section-20)
- [Ce qu’il faut retenir](#section-21)

<a id="section-1"></a>
## Objectif

Définir toutes les règles de conception des boutons afin de favoriser :

* une compréhension immédiate ;
* une cohérence visuelle ;
* une excellente accessibilité ;
* une action claire et mesurable.

Un bon bouton doit être vu, compris et utilisé sans hésitation.

<a id="section-2"></a>
## Qu’est-ce qu’un bouton ?

Un bouton est un élément interactif qui déclenche une action.

Exemples :

* Créer un compte
* Enregistrer
* Ajouter au panier
* Supprimer
* Télécharger
* Payer

Un bouton ne sert jamais à naviguer vers une page sans action. Dans ce cas, un lien est souvent plus approprié.

<a id="section-3"></a>
## Anatomie d’un bouton

Un bouton est composé de plusieurs éléments :

┌──────────────────────────┐
│      + Icône (optionnelle)
│
│      Texte
│
│      Padding horizontal
│
│      Padding vertical
└──────────────────────────┘

Chaque élément influence la lisibilité et la facilité d’interaction.

<a id="section-4"></a>
## Les caractéristiques d’un bon bouton

Un bouton doit être :

* identifiable ;
* facile à cliquer ;
* suffisamment contrasté ;
* cohérent avec le Design System ;
* explicite.

L’utilisateur ne doit jamais se demander :

Est-ce que c’est un bouton ?

<a id="section-5"></a>
## Le texte du bouton

Le texte est l’élément le plus important.

Utilise toujours :

✔ un verbe

✔ une action

✔ une phrase courte

### Exemples

Excellent :

Créer un compte
Enregistrer
Ajouter au panier
Télécharger le PDF
Confirmer la commande

Moyen :

Continuer
Valider
OK
Suivant

Ces mots ne décrivent pas clairement l’action.

### La longueur idéale

Entre 1 et 5 mots.

Plus le bouton est court, plus il est rapide à comprendre.

<a id="section-6"></a>
## Les types de boutons

### Bouton primaire

Action principale.

Il attire immédiatement le regard.

Exemple :

Créer un compte

Une seule action primaire est généralement suffisante par écran.

### Bouton secondaire

Action moins importante.

Exemple :

Annuler

Il doit être moins visible.

### Bouton tertiaire

Action secondaire.

Souvent présenté sous forme de texte.

Exemple :

En savoir plus

### Bouton destructif

Actions irréversibles.

Exemple :

Supprimer définitivement

Toujours accompagné d’une couleur d’alerte.

<a id="section-7"></a>
## Une seule action principale

### Erreur classique :

Créer
Modifier
Importer
Exporter
Partager

Tous les boutons ont le même style.

L’utilisateur hésite.

### Bonne pratique :

Créer un projet
──────────────
Importer
Exporter
Partager

Une seule action domine visuellement.

<a id="section-8"></a>
## Les dimensions

Un bouton doit être suffisamment grand.

Sur écran tactile, une zone interactive d’environ 44 × 44 px ou plus est souvent recommandée pour rester confortable.

Le bouton ne doit jamais être difficile à toucher.

<a id="section-9"></a>
## Les espacements internes

Le texte doit respirer.

Évite :

[Créer]

Préfère :

[   Créer un compte   ]

Le padding donne une zone d’activation plus confortable et plus facile à distinguer.

<a id="section-10"></a>
## Les icônes

Les icônes renforcent le sens.

Exemple :

⬇ Télécharger

Elles ne remplacent jamais le texte.

<a id="section-11"></a>
## Les états

Un bouton possède plusieurs états.

### Normal

État par défaut.

### Hover

L’utilisateur comprend qu’il peut interagir.

Exemple :

* légère variation de couleur ;
* légère ombre.

### Focus

Visible au clavier.

Le focus ne doit jamais être supprimé.

### Active

Moment où l’utilisateur clique.

Le bouton fournit un retour visible dès l’action.

### Loading

Le système travaille.

Le bouton indique clairement que l’action est en cours.

Exemple :

Création...

ou

⟳ Enregistrement...

### Disabled

Le bouton est indisponible.

Mais l’utilisateur doit comprendre pourquoi.

Un bouton désactivé sans explication est frustrant.

<a id="section-12"></a>
## Les couleurs

Le bouton primaire utilise :

* la couleur principale.

Le bouton secondaire :

* gris ;
* contour ;
* faible contraste.

Le bouton destructif :

* rouge.

Ne mélange jamais les significations.

<a id="section-13"></a>
## Les coins

Le rayon des coins doit être cohérent.

Exemple :

Toutes les interfaces utilisent :

* 8 px

ou

* 12 px

Pas :

6 px
14 px
3 px
18 px

La cohérence est essentielle.

<a id="section-14"></a>
## Les animations

Les animations doivent rester discrètes.

Exemple :

* changement de couleur ;
* légère élévation ;
* transition rapide.

Évite les effets spectaculaires.

Le bouton doit rester un outil, pas une distraction.

<a id="section-15"></a>
## Les boutons dans les formulaires

Le bouton principal apparaît :

* après les champs ;
* bien séparé ;
* suffisamment visible.

L’utilisateur termine naturellement le formulaire.

<a id="section-16"></a>
## Les boutons dans les modales

Ordre conseillé :

Annuler
Confirmer

L’action principale est clairement identifiable.

Les actions destructives doivent être explicites :

Supprimer définitivement

est préférable à :

OK

<a id="section-17"></a>
## Les boutons avec confirmation

Les confirmations sont utiles uniquement lorsque :

* l’action est irréversible ;
* les conséquences sont importantes.

Évite les confirmations inutiles.

<a id="section-18"></a>
## Les erreurs fréquentes

❌ Plusieurs boutons primaires.

❌ Boutons minuscules.

❌ Aucun état Hover.

❌ Focus supprimé.

❌ Boutons désactivés sans explication.

❌ Texte ambigu.

❌ Icônes sans texte.

❌ Couleurs incohérentes.

❌ Trop d’effets visuels.

<a id="section-19"></a>
## Cas pratique

Prenons une page de création de projet.

Une mauvaise interface propose cinq boutons identiques :

Créer
Importer
Exporter
Partager
Paramètres

L’utilisateur ne sait pas où commencer.

Une meilleure interface met en avant :

Créer un projet

Les autres actions sont placées dans une barre d’outils secondaire.

Le parcours devient évident.

<a id="section-20"></a>
## Checklist du chapitre

Avant de publier une interface :

* ☐ Chaque bouton déclenche une action claire.
* ☐ Le texte commence par un verbe.
* ☐ Une seule action principale est mise en avant.
* ☐ Les dimensions sont confortables sur mobile comme sur desktop.
* ☐ Les états Normal, Hover, Focus, Active, Disabled et Loading sont définis.
* ☐ Les couleurs suivent le Design System.
* ☐ Les icônes complètent le texte sans le remplacer.
* ☐ Les animations restent discrètes.
* ☐ Les boutons destructifs sont clairement identifiés.
* ☐ Les boutons sont cohérents sur toutes les pages.

<a id="section-21"></a>
## Ce qu’il faut retenir

Un bouton n’est pas seulement un élément graphique.

C’est le point de décision de l’utilisateur.

Lorsqu’il est bien conçu, l’utilisateur comprend clairement l’action déclenchée par le clic.

Lorsqu’il est mal conçu, il peut créer de l’hésitation et des erreurs ; vérifier l’effet sur le parcours réel.
