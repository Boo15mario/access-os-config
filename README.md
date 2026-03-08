# access-os-config

Configuration files for installed Access OS systems.

## Package repositories

`etc/pacman.conf` enables the Access OS package repositories:

- `access-os-core`
- `access-os-extra`

These repositories are published by the `access-os-packages` repository.

- package metadata is served from GitHub Pages
- package files are served from GitHub Releases

## Expected maintenance workflow

Package building and publishing is expected to happen from a local Arch Linux system in the `access-os-packages` repository.

After new packages are published there, this config repo can consume them through the pacman configuration already included in `etc/pacman.conf`.
