# Formulaires et validation

Chaque champ supplémentaire peut augmenter la friction du parcours.

## Sommaire

- [Objectif](#section-1)
- [Les principes fondamentaux](#section-2)
- [La règle n°1](#section-3)
- [Organiser les champs](#section-4)
- [Les labels](#section-5)
- [Les placeholders](#section-6)
- [Les champs obligatoires](#section-7)
- [Les tailles des champs](#section-8)
- [Les types de champs](#section-9)
- [Les messages d’aide](#section-10)
- [La validation en temps réel](#section-11)
- [Les messages d’erreur](#section-12)
- [Les couleurs des erreurs](#section-13)
- [Les mots de passe](#section-14)
- [Les listes déroulantes](#section-15)
- [Les cases à cocher](#section-16)
- [Les boutons radio](#section-17)
- [Les interrupteurs (Switch)](#section-18)
- [Les champs numériques](#section-19)
- [Les dates](#section-20)
- [Les formulaires longs](#section-21)
- [Les confirmations](#section-22)
- [Les erreurs fréquentes](#section-23)
- [Cas pratique](#section-24)
- [Checklist du chapitre](#section-25)
- [Ce qu’il faut retenir](#section-26)

<a id="section-1"></a>
## Objectif

Les formulaires sont l’un des points de friction les plus importants d’une interface.

Ils permettent de :

* créer un compte ;
* se connecter ;
* payer ;
* réserver ;
* contacter un service ;
* rechercher des informations.

Un formulaire bien conçu réduit les erreurs et accélère la saisie ; son effet sur la conversion doit être mesuré dans le contexte réel.

<a id="section-2"></a>
## Les principes fondamentaux

Un bon formulaire doit être :

* simple ;
* rapide ;
* compréhensible ;
* rassurant ;
* accessible.

L’utilisateur ne doit jamais se demander :

Que dois-je remplir ?

<a id="section-3"></a>
## La règle n°1

### Demander uniquement les informations nécessaires

Chaque champ supplémentaire peut augmenter le risque d’abandon ; vérifier ce risque dans le contexte réel.

Avant d’ajouter un champ, pose-toi toujours cette question :

Cette information est-elle indispensable aujourd’hui ?

Exemple :

Pour créer un compte :

✔ Email

✔ Mot de passe

Souvent, le numéro de téléphone, l’adresse postale ou la date de naissance peuvent être demandés plus tard.

<a id="section-4"></a>
## Organiser les champs

Les informations doivent suivre un ordre logique.

Exemple :

Informations personnelles
Nom
Prénom
Email
Téléphone

Puis :

Adresse
Rue
Ville
Code postal
Pays

Le cerveau comprend naturellement cette organisation.

<a id="section-5"></a>
## Les labels

Chaque champ doit posséder un label visible.

✔

Adresse e-mail
[_______________]

❌

[Adresse e-mail]

Le placeholder disparaît lorsque l’utilisateur commence à saisir.

Le label doit rester visible.

<a id="section-6"></a>
## Les placeholders

Le placeholder sert uniquement à montrer un exemple.

Exemple :

Nom de l'entreprise
Exemple : OpenAI

Il ne remplace jamais une explication.

<a id="section-7"></a>
## Les champs obligatoires

Évite de marquer tous les champs comme obligatoires.

Deux approches sont possibles :

### Option 1

Tous les champs sont obligatoires.

Les champs facultatifs sont indiqués.

✔ Recommandé.

### Option 2

Tous les champs portent un astérisque.

Cette approche est plus lourde visuellement.

<a id="section-8"></a>
## Les tailles des champs

La largeur doit refléter le contenu attendu.

Exemple :

Nom

──────────────

Description

──────────────────────────────────────────────

Code postal

──────

Le cerveau comprend immédiatement ce qui est attendu.

<a id="section-9"></a>
## Les types de champs

Chaque donnée possède son composant.

Donnée	Composant recommandé
Nom	Champ texte
Mot de passe	Champ sécurisé
Date	Sélecteur de date
Pays	Liste déroulante
Quantité	Champ numérique
Oui / Non	Radio ou Switch
Plusieurs choix	Cases à cocher

Ne force pas un utilisateur à saisir un format qui pourrait être sélectionné.

<a id="section-10"></a>
## Les messages d’aide

Le texte d’aide doit apparaître avant que l’utilisateur fasse une erreur.

Exemple :

Mot de passe
Minimum 12 caractères

Plutôt que d’afficher cette information uniquement après un échec.

<a id="section-11"></a>
## La validation en temps réel

L’utilisateur doit savoir immédiatement si une valeur est correcte.

Exemple :

✔ Adresse e-mail valide

✔ Mot de passe suffisamment fort

✔ Nom disponible

Cela évite de découvrir plusieurs erreurs à la fin du formulaire.

<a id="section-12"></a>
## Les messages d’erreur

Un bon message d’erreur répond à trois questions :

1. Quel est le problème ?
2. Pourquoi ?
3. Comment le corriger ?

### Mauvais exemple

Erreur

### Bon exemple

Le mot de passe doit contenir au moins
12 caractères et une lettre majuscule.

L’utilisateur sait quoi faire.

<a id="section-13"></a>
## Les couleurs des erreurs

Ne repose jamais uniquement sur la couleur.

Ajouter :

✔ une icône ;

✔ un texte explicatif ;

✔ un contour.

Les personnes daltoniennes doivent comprendre le message.

<a id="section-14"></a>
## Les mots de passe

Toujours permettre :

✔ afficher / masquer ;

✔ copier ;

✔ coller.

Ne bloque jamais le collage.

Les gestionnaires de mots de passe doivent fonctionner.

<a id="section-15"></a>
## Les listes déroulantes

Une liste déroulante est adaptée lorsqu’il existe un nombre limité de choix.

Exemple :

Pays.

En revanche, si une liste contient plusieurs centaines d’éléments, ajoute une recherche.

<a id="section-16"></a>
## Les cases à cocher

Utiliser une case à cocher lorsque plusieurs réponses sont possibles.

Exemple :

☐ Newsletter
☐ Offres promotionnelles
☐ Nouveautés

<a id="section-17"></a>
## Les boutons radio

Les boutons radio servent lorsqu’un seul choix est possible.

Exemple :

◉ Particulier
○ Entreprise

<a id="section-18"></a>
## Les interrupteurs (Switch)

Utiliser un switch uniquement pour activer ou désactiver une option immédiatement.

Exemple :

Notifications
ON

Ne l’utilise pas dans un formulaire qui sera validé plus tard.

<a id="section-19"></a>
## Les champs numériques

Limiter les erreurs.

Exemple :

Âge

[-] 24 [+]

est souvent préférable à un champ libre.

<a id="section-20"></a>
## Les dates

Éviter de demander :

Jour
Mois
Année

Trois champs ralentissent la saisie.

Privilégier un sélecteur de date adapté au contexte ou un champ avec un format clairement indiqué.

<a id="section-21"></a>
## Les formulaires longs

Découper le formulaire en plusieurs étapes.

Exemple :

Étape 1

Informations personnelles

↓

Étape 2

Adresse

↓

Étape 3

Paiement

Une barre de progression rassure l’utilisateur.

<a id="section-22"></a>
## Les confirmations

Après validation :

Toujours expliquer ce qu’il s’est passé.

Exemple :

✔ Votre compte a été créé.

✔ Votre commande a été enregistrée.

✔ Votre paiement a été accepté.

Ne laisse jamais l’utilisateur dans le doute.

<a id="section-23"></a>
## Les erreurs fréquentes

❌ Trop de champs.

❌ Labels remplacés par des placeholders.

❌ Messages d’erreur vagues.

❌ Validation uniquement à la fin.

❌ Bouton désactivé sans explication.

❌ Champs mal alignés.

❌ Plusieurs colonnes inutiles sur mobile.

❌ Demander des informations non essentielles.

<a id="section-24"></a>
## Cas pratique

Imaginons un formulaire d’inscription.

### Mauvaise version

* 18 champs obligatoires ;
* placeholder à la place des labels ;
* aucune aide ;
* erreurs uniquement après validation ;
* mot de passe masqué sans possibilité de l’afficher.

Résultat : abandon fréquent.

### Bonne version

* Email ;
* Mot de passe ;
* Confirmation du mot de passe.

Validation en temps réel.

Indicateur de robustesse du mot de passe.

Bouton principal clairement visible.

Les informations complémentaires pourront être demandées après la création du compte.

<a id="section-25"></a>
## Checklist du chapitre

Avant de publier un formulaire :

* ☐ Chaque champ est indispensable.
* ☐ Les champs sont regroupés de manière logique.
* ☐ Les labels restent visibles.
* ☐ Les placeholders servent uniquement d’exemple.
* ☐ Les messages d’aide sont affichés avant les erreurs.
* ☐ La validation intervient dès que possible.
* ☐ Les messages d’erreur expliquent la solution.
* ☐ Les composants correspondent au type de donnée.
* ☐ Le formulaire est entièrement navigable au clavier.
* ☐ La confirmation finale rassure l’utilisateur.

<a id="section-26"></a>
## Ce qu’il faut retenir

Les formulaires sont souvent le dernier obstacle entre l’utilisateur et son objectif.

Un bon formulaire demande peu d’informations, guide la saisie, prévient les erreurs et rassure à chaque étape.

Lorsqu’il est bien conçu, il devient presque invisible : l’utilisateur se concentre sur sa tâche, pas sur l’interface.
