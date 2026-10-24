# Base Them'All

Système de jeu vierge pour Foundry VTT v14.

## Installation

Dans Foundry, onglet « Systèmes de jeu » → « Installer un système », coller l'URL du manifeste :

```
https://github.com/ScallDePell/base-them-all/releases/latest/download/system.json
```

Ou copier ce dépôt dans `Data/systems/base-them-all/` (le nom du dossier doit être identique à l'`id` du manifeste).

Le seul fichier requis par Foundry est `system.json`. Aucun type de document, script, style ni paramètre n'est déclaré.

## Publier une release

Pousser un tag `vX.Y.Z` :

```
git tag v0.2.0
git push origin v0.2.0
```

Le workflow `.github/workflows/release.yml` met à jour `version`, `manifest` et `download` dans `system.json`, crée `base-them-all.zip` et publie la release avec ces deux fichiers.
