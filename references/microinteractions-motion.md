# Micro-interactions et motion

Les utilisateurs remarquent rarement une bonne animation. En revanche, ils remarquent immédiatement son absence lorsqu’ils ne comprennent plus ce qui se passe.

⸻

Objectif

Les micro-interactions rendent une interface plus compréhensible.

Elles permettent de :

* confirmer une action ;
* guider l’attention ;
* expliquer un changement ;
* réduire l’incertitude ;
* améliorer la perception de fluidité.

Une animation n’est jamais un élément décoratif.

Elle est un outil de communication.

⸻

Qu’est-ce qu’une micro-interaction ?

Une micro-interaction est une réaction visuelle à une action de l’utilisateur.

Exemples :

* cliquer sur un bouton ;
* ouvrir un menu ;
* ajouter un produit au panier ;
* supprimer un élément ;
* recevoir une notification ;
* activer un interrupteur.

⸻

Les quatre éléments d’une micro-interaction

Toute micro-interaction est composée de quatre parties.

Déclencheur
↓
Règle
↓
Feedback
↓
Fin

⸻

Déclencheur

C’est l’action qui lance l’interaction.

Exemple :

Clique sur :

Ajouter au panier

⸻

Règle

Le système décide :

Que doit-il se passer ?

Exemple :

* ajouter le produit ;
* mettre à jour le compteur ;
* afficher une confirmation.

⸻

Feedback

Le système informe immédiatement l’utilisateur.

Exemple :

✔ Animation

✔ Son (optionnel)

✔ Changement de couleur

✔ Notification

⸻

Fin

L’interaction revient à un état stable.

⸻

Pourquoi les animations sont importantes ?

Sans animation :

Menu
↓
Disparaît

Le cerveau perd le contexte.

⸻

Avec animation :

Menu
↓
Glisse
↓
Disparaît

Le cerveau comprend naturellement le changement.

⸻

Les objectifs d’une animation

Une animation doit toujours répondre à une question.

Exemple :

Que s’est-il passé ?

↓

Le bouton devient vert.

⸻

Où est passé l’élément ?

↓

Il glisse hors de l’écran.

⸻

Que dois-je regarder ?

↓

Une légère animation attire l’œil.

⸻

Si l’animation ne répond à aucune question,

elle est probablement inutile.

⸻

Les principes fondamentaux

Une bonne animation est :

* rapide ;
* discrète ;
* cohérente ;
* utile.

Elle ne cherche jamais à impressionner.

⸻

Les durées

Les transitions doivent être courtes.

En pratique :

Type	Durée indicative
Très rapide	100 à 150 ms
Standard	150 à 250 ms
Complexe	250 à 400 ms

Des animations plus longues donnent souvent une impression de lenteur.

⸻

Les boutons

Lorsqu’un bouton est cliqué :

Il doit répondre immédiatement.

Exemple :

* légère réduction de taille ;
* changement de couleur ;
* apparition d’un état de chargement si nécessaire.

Le bouton ne doit jamais rester immobile.

⸻

Les menus

Un menu doit apparaître progressivement.

Éviter :

Invisible
↓
Visible

Préférer :

Invisible
↓
Fondu
↓
Visible

ou

Invisible
↓
Glissement
↓
Visible

Le mouvement crée un lien logique entre les états.

⸻

Les modales

Une modale doit sembler venir de quelque part.

Exemple :

* léger agrandissement ;
* fondu ;
* arrière-plan assombri.

La fermeture suit le mouvement inverse.

⸻

Les notifications

Une notification apparaît :

* rapidement ;
* sans masquer l’information importante ;
* puis disparaît lorsque cela est approprié ou après action de l’utilisateur.

Les notifications critiques ne doivent pas disparaître automatiquement avant d’avoir été lues.

⸻

Les Skeletons

Pendant le chargement :

Éviter :

Chargement...

Privilégier :

Un squelette représentant la future interface.

Les Skeletons réduisent la perception du temps d’attente.

⸻

Les transitions entre pages

Le changement d’écran ne doit pas sembler brutal.

Une transition légère aide l’utilisateur à conserver son contexte.

Elle ne doit jamais ralentir la navigation.

⸻

Les listes

Lorsqu’un élément est ajouté :

Il apparaît progressivement.

Lorsqu’il est supprimé :

Il disparaît progressivement.

Le cerveau comprend ce changement beaucoup plus facilement.

⸻

Les drag & drop

Le déplacement doit être visible.

L’utilisateur doit toujours savoir :

* quel élément il déplace ;
* où il va être déposé.

Les zones de dépôt doivent être mises en évidence.

⸻

Les formulaires

Une erreur apparaît :

* près du champ concerné ;
* avec une transition discrète ;
* sans faire sauter toute la page.

Une validation réussie peut être accompagnée d’un changement visuel léger.

⸻

Les graphiques

Les graphiques peuvent animer :

* l’apparition des données ;
* les changements de filtres ;
* les mises à jour.

Les animations doivent aider à comprendre les évolutions, pas les masquer.

⸻

Les transitions d’état

Chaque état doit être relié visuellement au précédent.

Exemple :

Bouton
↓
Loading
↓
Succès

Une transition progressive est plus compréhensible qu’un changement instantané.

⸻

Les animations à éviter

❌ Rotation permanente.

❌ Clignotements rapides.

❌ Parallaxe excessive.

❌ Animations décoratives sans fonction.

❌ Durées trop longues.

❌ Effets différents sur chaque écran.

⸻

Les préférences utilisateur

Certains utilisateurs préfèrent limiter les animations.

Lorsque le système d’exploitation indique une préférence de réduction des mouvements, l’interface doit en tenir compte :

* supprimer les animations non essentielles ;
* conserver uniquement les transitions nécessaires à la compréhension.

⸻

Les erreurs fréquentes

❌ Aucune animation.

❌ Animations trop lentes.

❌ Effets différents selon les pages.

❌ Animation qui retarde l’action.

❌ Pas de retour après un clic.

❌ Mouvement excessif.

❌ Transitions incohérentes.

⸻

Cas pratique

Imaginons une application de gestion de tâches.

Mauvaise conception

L’utilisateur clique sur :

Terminer

La tâche disparaît instantanément.

Aucun retour.

L’utilisateur hésite :

Ai-je vraiment terminé cette tâche ?

⸻

Bonne conception

Après le clic :

* la case se coche ;
* la ligne devient légèrement plus claire ;
* une animation de disparition est jouée ;
* un message confirme que la tâche est terminée.

Le changement est immédiatement compris.

⸻

Checklist du chapitre

Avant de publier une interface :

* ☐ Chaque interaction reçoit un retour visuel.
* ☐ Les animations ont une fonction précise.
* ☐ Les durées restent courtes et cohérentes.
* ☐ Les transitions expliquent les changements d’état.
* ☐ Les menus apparaissent progressivement.
* ☐ Les boutons réagissent immédiatement au clic.
* ☐ Les états de chargement sont visibles.
* ☐ Les notifications n’interrompent pas inutilement le travail.
* ☐ Les animations respectent la préférence de réduction des mouvements.
* ☐ Aucun effet décoratif ne nuit à la lisibilité.

⸻

Ce qu’il faut retenir

Le motion design ne sert pas à rendre une interface spectaculaire.

Il sert à rendre les interactions compréhensibles.

Une bonne animation est presque invisible : elle accompagne naturellement l’utilisateur, réduit les incertitudes et renforce la sensation de fluidité.

Lorsqu’une interface paraît « vivante » sans devenir distrayante, les micro-interactions ont parfaitement rempli leur rôle.

⸻

Notes d’application

Le prochain chapitre sera consacré au Design des applications SaaS modernes. Nous verrons comment organiser les espaces de travail, les tableaux de bord, les vues détaillées, les workflows complexes, les systèmes de permissions, les filtres avancés et les interfaces orientées productivité. Ce chapitre synthétisera les pratiques observées dans des produits comme Linear, Notion, Figma, GitHub ou Stripe, tout en restant fondé sur les principes UX présentés dans ce manuel.
