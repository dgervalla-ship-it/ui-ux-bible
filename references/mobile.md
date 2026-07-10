# Mobile
## Sommaire

- [Objectif](#section-1)
- [Les performances](#section-2)
- [Cas pratique](#section-3)
- [Checklist du chapitre](#section-4)

<a id="section-1"></a>
## Objectif
Concevoir une application mobile ne consiste pas à réduire une interface desktop.

Le mobile possède :

* ses propres contraintes ;
* ses propres comportements ;
* ses propres composants ;
* ses propres attentes.

Une excellente application mobile est pensée mobile-first, et non adaptée après coup.

Les différences entre Desktop et Mobile

Desktop	Mobile
Grande surface	Surface limitée
Souris + clavier	Doigts
Plusieurs fenêtres	Une seule vue
Utilisation longue	Sessions courtes
Haute précision	Précision limitée

Ces différences influencent chaque décision de design.

Le contexte d’utilisation

Un utilisateur mobile peut être :

* dans les transports ;
* en marchant ;
* au soleil ;
* avec une seule main ;
* interrompu à tout moment.

L’interface doit rester efficace dans ces conditions.

Les objectifs du design mobile

Une bonne application mobile est :

* rapide ;
* simple ;
* lisible ;
* tactile ;
* tolérante aux erreurs.

Le pouce

Le pouce est le principal outil d’interaction.

Les actions fréquentes doivent être placées dans les zones les plus accessibles.

Exemple simplifié :

┌──────────────┐
│ Zone difficile│
│              │
│ Zone moyenne │
│              │
│ Zone idéale  │
└──────────────┘

Les CTA principaux doivent être proches de cette zone confortable.

Les zones tactiles

Les éléments interactifs doivent être suffisamment grands.

Objectif :

* faciles à toucher ;
* suffisamment espacés.

Éviter :

❌ Deux petits boutons très proches.

Privilégier :

✔ Des boutons larges avec un espacement suffisant.

Une seule tâche par écran

Chaque écran doit répondre à une question.

Exemple :

Écran Paiement.

↓

Uniquement le paiement.

Évite de mélanger :

* profil ;
* paramètres ;
* historique ;
* paiement.

La navigation mobile

Les modèles les plus utilisés sont :

Barre de navigation inférieure

Idéale pour :

* 3 à 5 sections principales.

Exemple :

Accueil
Recherche
Ajouter
Notifications
Profil

Navigation latérale

Adaptée aux applications riches.

Elle doit rester secondaire.

Les actions principales ne doivent pas être cachées uniquement dans un menu latéral.

Navigation par onglets

Très utile lorsque plusieurs vues concernent le même contenu.

Exemple :

Articles
Favoris
Téléchargés

Les gestes

Les gestes doivent compléter les contrôles visibles.

Ils ne doivent jamais les remplacer.

Exemple :

Le balayage pour supprimer est utile.

Mais un bouton « Supprimer » reste nécessaire.

Les gestes cachés sont difficiles à découvrir.

Le clavier

Le clavier masque une partie importante de l’écran.

Le formulaire doit :

* rester visible ;
* faire défiler automatiquement le champ actif ;
* adapter le type de clavier (email, téléphone, numérique, etc.) au contenu attendu.

Les formulaires mobiles

Réduis au maximum la saisie.

Utilise :

* listes ;
* sélecteurs ;
* scan ;
* géolocalisation ;
* remplissage automatique.

Moins l’utilisateur tape, meilleure est l’expérience.

Les composants natifs

Les composants natifs d’iOS et d’Android répondent déjà aux attentes des utilisateurs.

Lorsque cela est pertinent, réutilise-les plutôt que de créer des composants entièrement personnalisés.

Tu bénéficies ainsi :

* d’une meilleure cohérence ;
* d’une meilleure accessibilité ;
* d’une meilleure intégration au système.

Les notifications

Les notifications push doivent apporter une valeur réelle.

Elles doivent être :

* utiles ;
* pertinentes ;
* peu fréquentes.

Une application qui envoie trop de notifications risque d’être désactivée.

Les états hors connexion

Les utilisateurs mobiles perdent plus souvent leur connexion.

L’application doit :

* détecter l’absence de réseau ;
* expliquer la situation ;
* permettre de reprendre une action lorsque la connexion revient.

Lorsque c’est possible, les données déjà consultées peuvent rester accessibles.
<a id="section-2"></a>
## Les performances
Sur mobile :

Chaque milliseconde compte.

Optimiser :

* images ;
* vidéos ;
* animations ;
* requêtes réseau ;
* mémoire.

Une application lente est rapidement abandonnée.

Les animations

Les transitions doivent :

* expliquer les changements ;
* rester courtes ;
* préserver le contexte.

Évite les animations longues qui ralentissent la navigation.

Les permissions

Demande une permission uniquement lorsqu’elle est nécessaire.

Exemple :

Ne demande pas l’accès à la localisation au premier lancement si cette fonctionnalité n’est pas encore utilisée.

Explique toujours pourquoi cette permission est utile.

Les écrans de chargement

Préfère :

* Skeleton ;
* indicateur de progression ;
* contenu progressif.

Évite les écrans vides avec un simple spinner lorsque des éléments peuvent déjà être affichés.

Les listes

Les listes sont omniprésentes sur mobile.

Elles doivent :

* défiler de manière fluide ;
* proposer une recherche si elles sont longues ;
* charger progressivement les données lorsque nécessaire.

Les cartes

Les cartes mobiles doivent :

* rester simples ;
* éviter la surcharge d’informations ;
* mettre en avant une seule action principale.

Les erreurs fréquentes

❌ Boutons trop petits.

❌ Navigation complexe.

❌ Menus cachés pour les actions principales.

❌ Trop de texte.

❌ Formulaires interminables.

❌ Animations trop lentes.

❌ Notifications excessives.

❌ Demande prématurée de permissions.

❌ Mauvaise gestion du mode hors connexion.
<a id="section-3"></a>
## Cas pratique
Imaginons une application bancaire.

Mauvaise conception

* Navigation composée de dix rubriques.
* Boutons très rapprochés.
* Formulaire de virement avec quinze champs.
* Aucun remplissage automatique.
* Impossible de reprendre une opération après une coupure réseau.

L’expérience devient frustrante.

Bonne conception

* Barre de navigation limitée aux fonctions essentielles.
* Boutons larges et faciles à atteindre.
* Formulaire simplifié.
* Clavier adapté au type de saisie.
* Sauvegarde automatique des informations déjà saisies.
* Synchronisation lorsque la connexion revient.

Le parcours est plus rapide et plus fiable.
<a id="section-4"></a>
## Checklist du chapitre
Avant de publier une application mobile :

* ☐ Les actions principales sont accessibles avec le pouce.
* ☐ Les zones tactiles sont suffisamment grandes.
* ☐ Chaque écran a un objectif unique.
* ☐ Les formulaires limitent la saisie.
* ☐ Le type de clavier est adapté au champ.
* ☐ Les composants natifs sont utilisés lorsque cela est pertinent.
* ☐ Les animations sont courtes et utiles.
* ☐ Les états hors connexion sont prévus.
* ☐ Les permissions sont demandées au bon moment.
* ☐ Les performances restent fluides sur des appareils de différentes gammes.

Ce qu’il faut retenir

Le mobile n’est pas une version réduite du desktop.

C’est un contexte d’utilisation différent, avec des contraintes propres.

Une application mobile réussie réduit les efforts de saisie, privilégie les interactions tactiles, reste performante dans toutes les situations et accompagne l’utilisateur, même lorsqu’il est interrompu ou hors connexion.

Le chapitre 25 sera consacré à un domaine devenu incontournable : les interfaces conversationnelles et les produits intégrant de l’intelligence artificielle. Nous y verrons comment concevoir des assistants, des interfaces de chat, des expériences pilotées par des modèles de langage, la gestion des prompts, des réponses, des erreurs, des sources, de la confiance et des interactions hybrides entre IA et interface graphique. Ce chapitre fera le lien entre les principes classiques de l’UX et les nouveaux usages de l’IA générative.
