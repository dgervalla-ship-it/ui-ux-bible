# Refonte contrôlée de `ui-ux-bible`

Date : 10 juillet 2026

## Objectif

Transformer le dépôt actuel en un skill Codex fiable, rapide à déclencher et facile à consulter, tout en conservant sa vocation de manuel UI/UX personnel et ses sources privées.

Le résultat doit corriger les incohérences éditoriales, actualiser les exigences normatives, réduire le coût de lecture et rester compatible avec les demandes de conception, d'audit et d'amélioration d'interfaces.

## Périmètre

La refonte couvre :

- le frontmatter et le routeur de `SKILL.md` ;
- les métadonnées UI dans `agents/openai.yaml` ;
- l'organisation et le format Markdown des références ;
- le découpage Navigation, Cartes et Data Tables ;
- le chapitre manquant sur les tests utilisateurs et l'expérimentation ;
- la suppression des résidus conversationnels et des promesses non réalisées ;
- la mise à jour des règles normatives depuis des sources officielles actuelles ;
- les index de sources, notamment pour le marketing et les OCR visuels ;
- les tests d'usage, les contrôles d'intégrité et la publication sur GitHub.

La refonte ne doit pas :

- séparer le dépôt en plusieurs skills ;
- réécrire ou redistribuer les ouvrages privés complets ;
- inventer des recommandations lorsque les sources sont ambiguës ;
- présenter une préférence éditoriale comme une exigence normative ;
- ajouter au package final des documents de processus inutiles à l'exécution du skill.

## Architecture cible

### Routeur principal

`SKILL.md` devient un routeur opérationnel compact :

1. une description de déclenchement inférieure à 1 024 caractères ;
2. un workflow court indiquant quelles références ouvrir et dans quel ordre ;
3. des invariants transversaux concis ;
4. une table sujet → référence ;
5. une procédure d'audit et de vérification avant livraison ;
6. des règles explicites pour rechercher dans les sources volumineuses sans les charger entièrement.

Le skill reste volontairement large sur les tâches UI/UX, mais le marketing général est traité comme une capacité secondaire : les informations dépendantes des plateformes ou du temps doivent être vérifiées auprès de sources actuelles.

### Références

Les références conservent une profondeur unique sous `references/`. Les noms deviennent explicites et stables ; la numérotation éditoriale ne doit plus être nécessaire pour trouver un sujet.

Chaque référence comprend au minimum :

- un titre Markdown unique ;
- un résumé opérationnel ;
- des sections navigables ;
- des règles ou critères vérifiables ;
- une checklist lorsque le sujet s'y prête ;
- une section de provenance pour les exigences normatives ou datées.

Le contenu Cartes et Data Tables est extrait du fichier Navigation. Le chapitre manquant couvre la préparation, la conduite et l'analyse des tests utilisateurs, ainsi que les conditions d'emploi et les limites des tests A/B.

### Sources privées

Les fichiers de `sources/` restent privés et inchangés, sauf leurs index et indications d'usage. Les deux OCR de *Refactoring UI* restent disponibles comme variantes d'extraction, sans être chargés ensemble par défaut.

Les index doivent :

- fournir des motifs de recherche ou des cartes sujet → section ;
- distinguer source historique, source normative et OCR brut ;
- corriger les affirmations factuellement fausses, notamment le nombre de palettes ;
- signaler que les galeries OCR ont perdu leur mise en page visuelle ;
- identifier le contenu marketing de 2018 comme historique et exiger une vérification actuelle pour les plateformes, politiques et tactiques changeantes.

### Métadonnées Codex

Ajouter `agents/openai.yaml` avec un nom lisible, une description courte et un prompt par défaut qui invoque explicitement `$ui-ux-bible`. Les valeurs doivent rester cohérentes avec le frontmatter de `SKILL.md`.

## Mise à jour du contenu

Les affirmations normatives sont vérifiées en priorité auprès de sources officielles actuelles, notamment W3C/WAI pour WCAG 2.2 et ARIA. Les recommandations propres aux plateformes s'appuient sur leurs guides officiels lorsque cela est nécessaire.

Chaque règle est classée implicitement ou explicitement comme :

- exigence normative ;
- convention de plateforme ;
- heuristique UX ;
- préférence du manuel.

Les formulations absolues sont conservées uniquement lorsqu'elles sont réellement universelles. Les règles telles que « une page = un seul objectif » ou « l'utilisateur ne doit jamais réfléchir » sont reformulées pour rester utiles dans les produits experts et les écrans complexes.

## Validation

La refonte suit un cycle RED–GREEN–REFACTOR appliqué au skill :

1. exécuter des scénarios sans le skill puis avec la version actuelle ;
2. conserver les échecs observables comme critères de correction ;
3. exécuter les mêmes scénarios avec la version révisée ;
4. corriger les lacunes sans élargir inutilement le périmètre.

Les scénarios couvrent au minimum :

- la spécification d'un écran d'inscription SaaS ;
- l'audit d'une interface existante ;
- la recherche d'une règle d'accessibilité précise ;
- une demande marketing dont les données peuvent être obsolètes.

Les contrôles finaux vérifient :

- la validité du frontmatter et de `agents/openai.yaml` ;
- la longueur de la description ;
- tous les chemins et liens internes ;
- l'absence de chapitres fusionnés, manquants ou annoncés à tort ;
- l'absence de résidus conversationnels et de promesses quantitatives non prouvées ;
- la présence de titres et de routes pour chaque référence ;
- le statut Git propre après commit ;
- la correspondance entre le commit local et la branche distante après publication.

## Publication

Les changements sont committés de façon intentionnelle sur `master`, puis poussés vers `origin/master`, conformément à la demande de mise à jour directe du dépôt GitHub.

Les sources privées ne doivent apparaître dans aucune sortie publique supplémentaire. Aucun pull request n'est requis pour ce dépôt personnel.

## Critères d'acceptation

La refonte est terminée lorsque :

- le skill passe les validations structurelles ;
- un agent trouve les bonnes références sans lecture excessive ;
- les scénarios de test produisent des réponses plus précises et traçables ;
- les incohérences recensées par l'audit sont corrigées ou explicitement déclassées ;
- le package final ne contient que les fichiers nécessaires au skill et à son dépôt ;
- `origin/master` contient les changements vérifiés.
