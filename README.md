# GestiT-ches
une application web simple de gestion de tâches personnelles
 une personne peut créer une tâche (titre, description, date d'échéance), la marquer comme complétée, et la
supprimer. Le projet est divisé en deux parties : un dossier /frontend (interface utilisateur) et un dossier
/backend (API et stockage des tâches).
Enok a géré le frontend
Mouhamadou a géré le backend
Mouhamadou fait les tests
## Stratégie de branchement

Pour le projet **GestiTâches**, notre équipe a choisi d'utiliser la stratégie **GitHub Flow**.

Nous avons choisi cette stratégie parce qu'elle est simple à comprendre et à utiliser pour un projet de courte durée. Elle permet à chaque membre de l'équipe de travailler sur une fonctionnalité ou une correction dans une branche séparée sans modifier directement la branche principale.

La branche `main` contient toujours une version stable du projet.

Pour chaque nouvelle fonctionnalité ou correction, une nouvelle branche est créée à partir de `main`. Une fois le travail terminé et testé, les modifications sont intégrées dans `main` à l'aide d'une Pull Request.

### Convention de nommage des branches

Nous utiliserons la convention suivante :

- `feature/nom-court` : pour l'ajout d'une nouvelle fonctionnalité.
- `fix/nom-court` : pour la correction d'un problème ou d'un bug.

Exemples :

- `feature/ajout-tache`
- `feature/modifier-tache`
- `feature/supprimer-tache`
- `feature/interface-frontend`
- `feature/api-backend`
- `fix/validation-formulaire`
- `fix/erreur-suppression`

Les noms des branches doivent être courts, descriptifs, écrits en minuscules et utiliser des tirets `-` pour séparer les mots.

### Fonctionnement

1. Partir de la branche `main`.
2. Créer une branche pour la tâche à réaliser.
3. Effectuer les modifications nécessaires.
4. Faire des commits avec des messages clairs.
5. Envoyer la branche sur GitHub.
6. Créer une Pull Request.
7. Faire vérifier les modifications par un membre de l'équipe.
8. Fusionner la branche dans `main` lorsque le travail est validé.
9. Supprimer la branche après la fusion.

Cette méthode nous permettra de travailler en parallèle tout en gardant la branche `main` stable et organisée.
