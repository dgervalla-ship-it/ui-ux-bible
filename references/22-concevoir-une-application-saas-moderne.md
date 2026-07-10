Chapitre 23 — Concevoir une Application SaaS Moderne

Une application SaaS n’est pas un site web. C’est un environnement de travail où les utilisateurs passent parfois plusieurs heures par jour.

⸻

Objectif

Les applications SaaS (Software as a Service) ont un objectif différent d’un site vitrine.

L’utilisateur ne vient pas découvrir un produit.

Il vient travailler.

Une interface SaaS doit donc privilégier :

* la rapidité ;
* la clarté ;
* l’efficacité ;
* la cohérence ;
* la productivité.

Chaque clic inutile devient une perte de temps répétée des centaines de fois.

⸻

Les différences entre un site Web et un SaaS

Site Web	Application SaaS
Convaincre	Produire
Découvrir	Travailler
Marketing	Productivité
Navigation simple	Navigation riche
Peu de données	Beaucoup de données

Ces différences influencent directement le design.

⸻

Les principes fondamentaux

Une application SaaS doit être :

* prévisible ;
* rapide ;
* stable ;
* personnalisable ;
* scalable.

⸻

Architecture générale

Une application SaaS suit souvent cette structure :

Workspace
├── Sidebar
├── Header
├── Toolbar
├── Workspace
└── Context Panel

Chaque zone possède un rôle précis.

⸻

1. La Sidebar

La Sidebar contient la navigation principale.

Elle ne change presque jamais.

Elle donne accès aux grandes sections :

Dashboard
Projets
Clients
Factures
Documents
Équipe
Paramètres

⸻

Bonnes pratiques

✔ Toujours visible.

✔ Même ordre.

✔ Icône + texte.

✔ Rubrique active identifiable.

⸻

À éviter

❌ Menus qui changent.

❌ Icônes seules.

❌ Plus de 12 sections principales.

⸻

2. Le Header

Le Header contient :

* le contexte actuel ;
* la recherche ;
* les notifications ;
* le profil ;
* les actions globales.

Exemple :

Projet Apollo
Recherche...
🔔
👤

⸻

3. La Toolbar

La Toolbar change selon le contexte.

Exemple :

Projet

↓

Créer

Filtrer

Exporter

Partager

⸻

Elle ne doit contenir que les actions utiles pour l’écran actuel.

⸻

4. Workspace

C’est la zone principale.

Elle contient :

* tableaux ;
* cartes ;
* graphiques ;
* formulaires.

Elle représente environ 80 % de l’écran.

⸻

5. Context Panel

Très utilisé dans les SaaS modernes.

Il affiche :

* détails ;
* historique ;
* commentaires ;
* activité ;
* propriétés.

Sans quitter la page.

⸻

Exemple :

Tableau
↓
Clique sur une ligne
↓
Le panneau de droite s'ouvre

L’utilisateur garde son contexte.

⸻

La règle des 3 niveaux

Une bonne interface SaaS comporte :

Niveau 1

Navigation.

⸻

Niveau 2

Contexte.

⸻

Niveau 3

Contenu.

⸻

Ne mélange jamais ces niveaux.

⸻

Les Workspaces

Chaque espace de travail doit être indépendant.

Exemple :

Entreprise A

↓

Ses utilisateurs.

Ses projets.

Ses factures.

⸻

Entreprise B

↓

Autres données.

Autres utilisateurs.

⸻

Les workspaces évitent les erreurs.

⸻

Les Permissions

Toutes les applications professionnelles possèdent des rôles.

Exemple :

Administrateur
Manager
Éditeur
Lecteur

Chaque rôle possède :

* ses actions ;
* ses menus ;
* ses permissions.

⸻

Les vues

Un même contenu peut être présenté sous différentes vues.

Exemple :

Liste

↓

Kanban

↓

Calendrier

↓

Timeline

↓

Gantt

L’utilisateur choisit selon son besoin.

⸻

Les recherches

Dans un SaaS,

la recherche est une fonctionnalité principale.

Elle doit :

* être rapide ;
* rechercher partout lorsque c’est pertinent ;
* mémoriser les recherches récentes ;
* proposer des raccourcis.

⸻

Les Command Palettes

Les meilleurs SaaS utilisent une palette de commandes.

Exemple :

Ctrl + K

Puis :

Créer un projet.

Inviter un utilisateur.

Ouvrir les paramètres.

⸻

Cette fonctionnalité accélère énormément le travail des utilisateurs expérimentés.

⸻

Les raccourcis clavier

Toutes les actions fréquentes devraient posséder un raccourci.

Exemple :

N
↓
Nouveau projet

ou

Ctrl + S
↓
Enregistrer

⸻

Les filtres

Les filtres doivent être :

* persistants lorsque cela est utile ;
* faciles à modifier ;
* visibles.

L’utilisateur ne doit jamais perdre son contexte de travail.

⸻

Les états vides

Chaque vue vide explique :

Pourquoi elle est vide.

Que faire ensuite.

Exemple :

Aucune facture.
Créez votre première facture.
[Créer]

⸻

Les actions destructives

Toujours :

* confirmation ;
* possibilité d’annuler si possible ;
* explication des conséquences.

⸻

Autosave

Les applications modernes sauvegardent automatiquement lorsque cela est pertinent.

L’utilisateur ne devrait pas craindre de perdre son travail.

Lorsque l’autosauvegarde est active, indique clairement son état :

* Enregistrement…
* Toutes les modifications sont enregistrées.
* Dernière sauvegarde à 14:32.

⸻

Historique

Permettre :

* Annuler.
* Rétablir.
* Historique des modifications.

Les utilisateurs expérimentent davantage lorsqu’ils savent qu’ils peuvent revenir en arrière.

⸻

Les notifications

Toutes les notifications ne se valent pas.

Information

Discrète.

⸻

Succès

Confirmation.

⸻

Erreur

Visible.

⸻

Urgence

Très visible.

⸻

Les notifications ne doivent jamais interrompre inutilement le travail.

⸻

Multi-tâches

Les utilisateurs SaaS changent souvent de contexte.

Ils doivent pouvoir :

* revenir rapidement ;
* retrouver leur état précédent ;
* conserver leurs filtres ;
* retrouver leur sélection.

Le produit doit accompagner ce comportement.

⸻

Performance perçue

Un SaaS doit sembler instantané.

Objectifs :

* ouverture rapide des écrans ;
* transitions fluides ;
* données visibles progressivement ;
* indicateurs de chargement lorsque nécessaire.

La perception de rapidité est aussi importante que la rapidité réelle.

⸻

Les erreurs fréquentes

❌ Tout ouvrir dans une nouvelle page.

❌ Perdre les filtres après un retour.

❌ Trop de menus.

❌ Pas de raccourcis clavier.

❌ Aucun historique.

❌ Sauvegarde manuelle obligatoire.

❌ Sidebar différente selon les pages.

❌ Trop de fenêtres modales.

❌ Rechargement complet après chaque action.

⸻

Cas pratique

Imaginons une application de gestion de projets.

Mauvaise conception

* Chaque clic ouvre une nouvelle page.
* Les filtres sont réinitialisés.
* Il faut enregistrer manuellement chaque modification.
* Les détails d’une tâche remplacent complètement la liste.

Résultat :

L’utilisateur perd constamment son contexte.

⸻

Bonne conception

* La liste reste visible.
* Les détails s’ouvrent dans un panneau latéral.
* Les modifications sont sauvegardées automatiquement.
* Les filtres sont conservés.
* Les raccourcis clavier accélèrent les actions fréquentes.
* Une palette de commandes permet d’accéder rapidement à toutes les fonctionnalités.

Le travail devient fluide et efficace.

⸻

Checklist du chapitre

Avant de publier une application SaaS :

* ☐ La navigation principale est stable.
* ☐ Le contexte est toujours visible.
* ☐ Les actions changent selon l’écran, mais restent cohérentes.
* ☐ Les utilisateurs ne perdent jamais leur contexte.
* ☐ Les filtres sont conservés lorsque c’est pertinent.
* ☐ Les détails peuvent être consultés sans quitter la vue principale.
* ☐ Les raccourcis clavier couvrent les actions fréquentes.
* ☐ Une recherche globale est disponible.
* ☐ Les modifications importantes sont sauvegardées automatiquement lorsque cela est approprié.
* ☐ Les performances permettent un travail fluide.

⸻

Ce qu’il faut retenir

Une excellente application SaaS disparaît derrière le travail de l’utilisateur.

Elle ne l’oblige pas à réfléchir à son fonctionnement.

Elle réduit les interruptions, limite les changements de contexte et accélère chaque action.

Le succès d’un SaaS se mesure moins à son apparence qu’à la vitesse avec laquelle ses utilisateurs accomplissent leurs tâches.

⸻

Notes d’application

Le chapitre 24 sera consacré au design mobile (iOS et Android). Nous y aborderons les différences entre mobile et desktop, les gestes tactiles, les zones de confort du pouce, les composants natifs, les spécificités des systèmes d’exploitation, les performances et les bonnes pratiques pour concevoir des applications mobiles professionnelles.
