# Formulaires et validation

Chaque champ supplémentaire diminue les chances que l’utilisateur termine sa tâche.

⸻

Objectif

Les formulaires sont l’un des points de friction les plus importants d’une interface.

Ils permettent de :

* créer un compte ;
* se connecter ;
* payer ;
* réserver ;
* contacter un service ;
* rechercher des informations.

Un formulaire bien conçu réduit les erreurs, accélère la saisie et améliore considérablement le taux de conversion.

⸻

Les principes fondamentaux

Un bon formulaire doit être :

* simple ;
* rapide ;
* compréhensible ;
* rassurant ;
* accessible.

L’utilisateur ne doit jamais se demander :

Que dois-je remplir ?

⸻

La règle n°1

Demander uniquement les informations nécessaires

Chaque champ supplémentaire augmente le risque d’abandon.

Avant d’ajouter un champ, pose-toi toujours cette question :

Cette information est-elle indispensable aujourd’hui ?

Exemple :

Pour créer un compte :

✔ Email

✔ Mot de passe

Souvent, le numéro de téléphone, l’adresse postale ou la date de naissance peuvent être demandés plus tard.

⸻

Organiser les champs

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

⸻

Les labels

Chaque champ doit posséder un label visible.

✔

Adresse e-mail
[_______________]

❌

[Adresse e-mail]

Le placeholder disparaît lorsque l’utilisateur commence à saisir.

Le label doit rester visible.

⸻

Les placeholders

Le placeholder sert uniquement à montrer un exemple.

Exemple :

Nom de l'entreprise
Exemple : OpenAI

Il ne remplace jamais une explication.

⸻

Les champs obligatoires

Évite de marquer tous les champs comme obligatoires.

Deux approches sont possibles :

Option 1

Tous les champs sont obligatoires.

Les champs facultatifs sont indiqués.

✔ Recommandé.

⸻

Option 2

Tous les champs portent un astérisque.

Cette approche est plus lourde visuellement.

⸻

Les tailles des champs

La largeur doit refléter le contenu attendu.

Exemple :

Nom

──────────────

Description

──────────────────────────────────────────────

Code postal

──────

Le cerveau comprend immédiatement ce qui est attendu.

⸻

Les types de champs

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

⸻

Les messages d’aide

Le texte d’aide doit apparaître avant que l’utilisateur fasse une erreur.

Exemple :

Mot de passe
Minimum 12 caractères

Plutôt que d’afficher cette information uniquement après un échec.

⸻

La validation en temps réel

L’utilisateur doit savoir immédiatement si une valeur est correcte.

Exemple :

✔ Adresse e-mail valide

✔ Mot de passe suffisamment fort

✔ Nom disponible

Cela évite de découvrir plusieurs erreurs à la fin du formulaire.

⸻

Les messages d’erreur

Un bon message d’erreur répond à trois questions :

1. Quel est le problème ?
2. Pourquoi ?
3. Comment le corriger ?

⸻

Mauvais exemple

Erreur

⸻

Bon exemple

Le mot de passe doit contenir au moins
12 caractères et une lettre majuscule.

L’utilisateur sait quoi faire.

⸻

Les couleurs des erreurs

Ne repose jamais uniquement sur la couleur.

Ajouter :

✔ une icône ;

✔ un texte explicatif ;

✔ un contour.

Les personnes daltoniennes doivent comprendre le message.

⸻

Les mots de passe

Toujours permettre :

✔ afficher / masquer ;

✔ copier ;

✔ coller.

Ne bloque jamais le collage.

Les gestionnaires de mots de passe doivent fonctionner.

⸻

Les listes déroulantes

Une liste déroulante est adaptée lorsqu’il existe un nombre limité de choix.

Exemple :

Pays.

En revanche, si une liste contient plusieurs centaines d’éléments, ajoute une recherche.

⸻

Les cases à cocher

Utiliser une case à cocher lorsque plusieurs réponses sont possibles.

Exemple :

☐ Newsletter
☐ Offres promotionnelles
☐ Nouveautés

⸻

Les boutons radio

Les boutons radio servent lorsqu’un seul choix est possible.

Exemple :

◉ Particulier
○ Entreprise

⸻

Les interrupteurs (Switch)

Utiliser un switch uniquement pour activer ou désactiver une option immédiatement.

Exemple :

Notifications
ON

Ne l’utilise pas dans un formulaire qui sera validé plus tard.

⸻

Les champs numériques

Limiter les erreurs.

Exemple :

Âge

[-] 24 [+]

est souvent préférable à un champ libre.

⸻

Les dates

Éviter de demander :

Jour
Mois
Année

Trois champs ralentissent la saisie.

Privilégier un sélecteur de date adapté au contexte ou un champ avec un format clairement indiqué.

⸻

Les formulaires longs

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

⸻

Les confirmations

Après validation :

Toujours expliquer ce qu’il s’est passé.

Exemple :

✔ Votre compte a été créé.

✔ Votre commande a été enregistrée.

✔ Votre paiement a été accepté.

Ne laisse jamais l’utilisateur dans le doute.

⸻

Les erreurs fréquentes

❌ Trop de champs.

❌ Labels remplacés par des placeholders.

❌ Messages d’erreur vagues.

❌ Validation uniquement à la fin.

❌ Bouton désactivé sans explication.

❌ Champs mal alignés.

❌ Plusieurs colonnes inutiles sur mobile.

❌ Demander des informations non essentielles.

⸻

Cas pratique

Imaginons un formulaire d’inscription.

Mauvaise version

* 18 champs obligatoires ;
* placeholder à la place des labels ;
* aucune aide ;
* erreurs uniquement après validation ;
* mot de passe masqué sans possibilité de l’afficher.

Résultat : abandon fréquent.

Bonne version

* Email ;
* Mot de passe ;
* Confirmation du mot de passe.

Validation en temps réel.

Indicateur de robustesse du mot de passe.

Bouton principal clairement visible.

Les informations complémentaires pourront être demandées après la création du compte.

⸻

Checklist du chapitre

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

⸻

Ce qu’il faut retenir

Les formulaires sont souvent le dernier obstacle entre l’utilisateur et son objectif.

Un bon formulaire demande peu d’informations, guide la saisie, prévient les erreurs et rassure à chaque étape.

Lorsqu’il est bien conçu, il devient presque invisible : l’utilisateur se concentre sur sa tâche, pas sur l’interface.

⸻

Notes d’application

À partir du prochain chapitre, nous aborderons la navigation, l’un des sujets les plus importants de ce manuel. Nous détaillerons les règles de conception des barres de navigation, menus latéraux, onglets, fils d’Ariane, recherches et systèmes de navigation responsive, afin de construire des interfaces où l’utilisateur sait toujours où il se trouve, où il peut aller et comment revenir en arrière. Cette partie fera largement écho aux principes de Don’t Make Me Think et de The Design of Everyday Things.
