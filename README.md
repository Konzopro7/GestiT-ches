# GestiTâches

GestiTâches est un petit projet d'équipe autour d'une application de gestion des tâches personnelles. L'idée est simple : permettre à une personne d'ajouter une tâche avec un titre, une description et une date d'échéance, de la marquer comme terminée ou de la supprimer.

Le dépôt sert aussi à mettre en pratique le travail collaboratif avec Git et GitHub. L'application est organisée en deux parties :

- `frontend/` : l'interface utilisée par la personne.
- `backend/` : l'API et le stockage des tâches.

## Équipe

- **Enock** : responsable de l'interface (frontend).
- **Mouhamadou** : responsable de l'API et du stockage (backend), des tests et de la coordination technique.

## Où en est le projet ?

Le dépôt prépare l'organisation de l'équipe et le backlog. Les dossiers de l'application peuvent être complétés au fil des prochaines tâches; ce dépôt ne prétend pas présenter une application déjà terminée.

## Travailler avec GitHub Flow

Nous utilisons GitHub Flow pour que chaque changement puisse être relu avant d'entrer dans `main`.

1. Mettre `main` à jour avant de commencer : `git switch main` puis `git pull`.
2. Créer une branche pour une seule tâche : `git switch -c feature/ajout-tache` ou `git switch -c fix/validation-titre`.
3. Faire des commits courts qui expliquent le changement, par exemple `Ajoute la validation du titre`.
4. Envoyer la branche sur GitHub avec `git push -u origin feature/ajout-tache`.
5. Ouvrir une Pull Request vers `main`. Expliquer ce qui a changé, pourquoi, et comment le vérifier.
6. Demander une revue à l'autre membre. Répondre aux commentaires et pousser les ajustements sur la même branche.
7. Après approbation et vérifications, fusionner la PR puis supprimer la branche.

La branche `main` est la version de référence du projet. On évite d'y pousser directement : les changements passent par une Pull Request. Les branches commencent par `feature/` pour une nouveauté ou `fix/` pour une correction. Le reste du nom est court, en minuscules, et les mots sont séparés par des tirets.

### Vérifier son accès au dépôt

Après avoir obtenu l'accès au dépôt, on peut vérifier que l'authentification fonctionne sans toucher à `main` :

```bash
git clone https://github.com/Konzopro7/GestiT-ches.git
cd GestiT-ches
git switch -c test/nom-prenom
echo "Vérification d'accès Git" > test-acces.txt
git add test-acces.txt
git commit -m "Vérifie l'accès au dépôt"
git push -u origin test/nom-prenom
```

Une fois le push confirmé, supprimer le fichier et la branche de test, ou ouvrir une PR de nettoyage si le fichier a déjà été partagé. Ne pas tester les permissions en tentant de contourner les règles de `main`.

## Backlog et contributions

Le fichier [BACKLOG.md](BACKLOG.md) décrit les premières user stories et leurs critères d'acceptation. Les modèles de Pull Request et d'issues se trouvent dans `.github/`. Avant d'ouvrir une issue, vérifier qu'une demande équivalente n'existe pas déjà.

## Démarrage

Les dossiers `frontend/` et `backend/` décrivent leur périmètre et leur état actuel. Les étapes d'installation et de lancement seront ajoutées lorsque les technologies de l'application seront choisies.
