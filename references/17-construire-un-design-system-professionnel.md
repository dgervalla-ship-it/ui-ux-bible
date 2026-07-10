Chapitre 18 — Construire un Design System Professionnel

Un Design System n’est pas une bibliothèque de composants. C’est un langage commun entre le design, le développement et le produit.

⸻

Objectif

Un Design System permet de créer des interfaces :

* cohérentes ;
* réutilisables ;
* maintenables ;
* évolutives.

Son objectif n’est pas seulement de gagner du temps.

Il garantit que chaque nouvelle fonctionnalité respecte les mêmes standards de qualité.

⸻

Pourquoi créer un Design System ?

Sans Design System, les problèmes apparaissent rapidement :

* cinq styles de boutons différents ;
* trois nuances de bleu pour la même action ;
* plusieurs espacements pour un même composant ;
* des formulaires qui changent selon les pages ;
* des composants dupliqués.

Le résultat :

* maintenance difficile ;
* dette technique ;
* incohérence visuelle ;
* expérience utilisateur dégradée.

⸻

Les 5 couches d’un Design System

Un Design System moderne est organisé en plusieurs niveaux.

Fondations
↓
Design Tokens
↓
Composants
↓
Patterns
↓
Templates

Chaque niveau dépend du précédent.

⸻

Niveau 1 — Les Fondations

Les fondations regroupent toutes les décisions globales.

Elles définissent :

* couleurs ;
* typographie ;
* espacements ;
* ombres ;
* rayons ;
* animations ;
* iconographie ;
* grille.

Les composants utilisent ces fondations.

Ils ne les redéfinissent jamais.

⸻

Niveau 2 — Les Design Tokens

Les Design Tokens sont les variables du système.

Ils remplacent les valeurs codées en dur.

Exemple :

Primary = #2563EB
Success = #16A34A
Danger = #DC2626
Spacing M = 16 px
Radius Large = 12 px

Le développeur utilise les tokens.

Jamais directement les valeurs.

⸻

Pourquoi utiliser des tokens ?

Imagine que la couleur principale change.

Sans tokens :

500 fichiers doivent être modifiés.

Avec des tokens :

Une seule valeur change.

Toute l’application est mise à jour.

⸻

Les catégories de tokens

Couleurs

Primary
Secondary
Neutral
Success
Warning
Danger
Info

⸻

Espacements

4
8
12
16
24
32
48
64

⸻

Rayons

Small
Medium
Large
Pill

⸻

Ombres

Shadow XS
Shadow S
Shadow M
Shadow L

⸻

Typographie

Font Family
Heading XL
Heading L
Body
Caption

⸻

Animations

Fast
Normal
Slow

⸻

Niveau 3 — Les composants

Les composants utilisent uniquement les tokens.

Exemple :

Bouton

↓

Couleur Primary

↓

Radius Medium

↓

Spacing 16

↓

Font Body Medium

Le composant ne définit aucune valeur lui-même.

⸻

Niveau 4 — Les Patterns

Un pattern est un assemblage de composants.

Exemple :

Connexion

Logo
↓
Titre
↓
Email
↓
Mot de passe
↓
Bouton
↓
Lien oublié

Chaque projet réutilise ce pattern.

⸻

Autres patterns :

* Checkout
* Recherche
* Dashboard
* Profil
* Carte produit
* Tableau
* Paramètres

⸻

Niveau 5 — Les Templates

Le template représente une page.

Exemple :

Dashboard

Navigation
↓
Header
↓
KPIs
↓
Graphiques
↓
Tableau

Le template n’invente rien.

Il assemble les patterns.

⸻

Les règles de nommage

Un composant possède un nom unique.

Exemple :

Button
Button Primary
Button Secondary
Input Text
Input Password
Modal Confirmation
Card Product

Évite :

Blue Button
Big Button
New Button
Button 2

Ces noms deviennent rapidement incompréhensibles.

⸻

Les variantes

Chaque composant définit ses variantes.

Exemple :

Button

↓

Primary

↓

Secondary

↓

Ghost

↓

Danger

↓

Link

Pas davantage si elles ne répondent pas à un besoin réel.

⸻

Les tailles

Les tailles sont standardisées.

Exemple :

Small
Medium
Large

Évite :

Tiny
Mini
Extra Mini
Huge
Ultra Large

La simplicité facilite l’adoption.

⸻

Les états

Tous les composants interactifs définissent :

Default
Hover
Focus
Active
Loading
Disabled
Error
Success

Aucun état ne doit être oublié.

⸻

Les icônes

Une seule bibliothèque.

Même style.

Même épaisseur.

Même taille.

Même logique.

Ne mélange jamais plusieurs familles d’icônes.

⸻

Les illustrations

Les illustrations suivent également une charte.

Même style.

Même palette.

Même niveau de détail.

⸻

Les animations

Les animations doivent respecter :

* la même durée ;
* le même easing ;
* la même logique.

Une interface cohérente paraît plus fluide.

⸻

Documentation

Chaque composant possède une documentation.

Elle contient :

Description
Quand utiliser
Quand ne pas utiliser
Variantes
États
Accessibilité
Code
Exemples

Une bibliothèque sans documentation devient rapidement inutilisable.

⸻

Gouvernance

Le Design System appartient à toute l’équipe.

Il doit définir :

* qui crée les composants ;
* qui les valide ;
* comment les modifier ;
* comment annoncer les changements.

Sans gouvernance, le système se dégrade progressivement.

⸻

Les versions

Comme un logiciel, le Design System évolue.

Chaque version documente :

* nouveautés ;
* corrections ;
* composants supprimés ;
* changements incompatibles.

⸻

Les audits

Un audit régulier permet d’identifier :

* composants dupliqués ;
* variantes inutiles ;
* incohérences ;
* dette technique.

Un Design System est un produit vivant.

⸻

Les erreurs fréquentes

❌ Créer un composant pour chaque écran.

❌ Copier-coller au lieu de réutiliser.

❌ Modifier localement un composant.

❌ Ne pas documenter.

❌ Trop de variantes.

❌ Mélanger plusieurs styles.

❌ Utiliser des valeurs codées en dur.

❌ Absence de gouvernance.

⸻

Cas pratique

Une équipe développe un SaaS pendant deux ans.

Sans Design System :

* 18 styles de boutons ;
* 11 tailles de titres ;
* 9 nuances de bleu ;
* 4 formulaires différents.

Chaque nouvelle fonctionnalité ajoute de nouvelles incohérences.

Avec un Design System :

* un seul bouton primaire ;
* une échelle typographique unique ;
* une palette centralisée ;
* des composants partagés.

Le développement est plus rapide, les interfaces sont cohérentes et les coûts de maintenance diminuent.

⸻

Checklist du chapitre

Avant de considérer un Design System comme prêt :

* ☐ Les fondations (couleurs, typographie, espacements, etc.) sont définies.
* ☐ Tous les composants utilisent des Design Tokens.
* ☐ Les composants sont documentés.
* ☐ Les variantes sont limitées et justifiées.
* ☐ Les états interactifs sont complets.
* ☐ Les règles de nommage sont cohérentes.
* ☐ Les patterns réutilisent les composants existants.
* ☐ Les templates assemblent les patterns sans créer de nouvelles règles.
* ☐ Une gouvernance encadre les évolutions.
* ☐ Un processus d’audit est en place.

⸻

Ce qu’il faut retenir

Un Design System n’est pas un fichier Figma.

C’est une architecture.

Il transforme des décisions individuelles en règles partagées.

Lorsqu’il est bien conçu, il améliore simultanément :

* la qualité du design ;
* la vitesse de développement ;
* la cohérence du produit ;
* la collaboration entre les équipes.

⸻

Notes d’application

À partir du chapitre 19, nous passerons à la dernière grande partie du manuel : l’audit UX/UI. Nous construirons une méthode professionnelle permettant d’évaluer n’importe quelle interface à l’aide d’une grille de contrôle de plus de 500 critères, couvrant l’UX, l’UI, l’accessibilité, la performance, le marketing, la conversion et la qualité technique. Ce chapitre transformera ce guide en un véritable référentiel d’évaluation utilisable lors de revues de design ou d’audits complets.
