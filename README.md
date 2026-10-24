# Base Them'All

A blank game system for Foundry VTT v14.

## Installation

In Foundry, go to the "Game Systems" tab → "Install System" and paste the manifest URL:

```
https://github.com/ScallDePell/base-them-all/releases/latest/download/system.json
```

Or copy this repository into `Data/systems/base-them-all/` (the folder name must match the manifest `id`).

The only file Foundry requires is `system.json`. No document types, scripts, styles or settings are declared.

## Publishing a release

In the repository's "Actions" tab, select the "Release" workflow, click "Run workflow" and enter the version (e.g. `0.2.0`). The `v0.2.0` tag is created automatically.

Or push a `vX.Y.Z` tag:

```
git tag v0.2.0
git push origin v0.2.0
```

The `.github/workflows/release.yml` workflow updates `version`, `manifest` and `download` in `system.json`, builds `base-them-all.zip` and publishes the release with both files.
