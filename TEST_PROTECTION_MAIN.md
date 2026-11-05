# Vérifier la protection de `main`

Le dépôt exige une Pull Request et au moins une approbation avant une fusion. Les règles s'appliquent aussi aux administrateurs.

Dans un terminal ouvert à la racine du dépôt, exécute les commandes suivantes :

```bash
git switch main
git pull --ff-only origin main
git switch -c test/refus-push-main
git commit --allow-empty -m "Test protection de main"
git push origin HEAD:main
```

Le dernier push doit être refusé. Le test effectué sur ce dépôt a retourné :

```text
remote: error: GH006: Protected branch update failed for refs/heads/main.
remote: - Changes must be made through a pull request.
! [remote rejected] HEAD -> main (protected branch hook declined)
```

Prends une capture où l'on voit la commande et ce refus. Après la capture, supprime la branche de test locale :

```bash
git switch feature/organisation-td-collaboratif
git branch -D test/refus-push-main
```

Le commit vide est créé uniquement sur la branche de test locale. Le push refusé ne modifie pas `main`.
