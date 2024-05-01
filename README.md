# BlueCat &nbsp; [![build-ublue](https://github.com/blue-build/template/actions/workflows/build.yml/badge.svg)](https://github.com/blue-build/template/actions/workflows/build.yml)

An opinionated tweaked [ublue](https://universal-blue.org/) image based on silverblue-main.

## What is this?

This is my own tweaked [ublue](https://universal-blue.org/) image deployment that I maintain for myself.

If anyone is using these images please reach out with a bug report so that I don't randomly change thing on your computer.

## Changes and Features

- All the uBlue backend goodies
- Gnome Console insetad of Gnome Terminal
- Steam pre-installed (only for AMD/Intel)
- NeoVim pre-installed
- v4l2loopback kernel module for obs virtual webcam
- Firefox replaced with LibreWolf flatpak
- A few pre-installed flatpaks (you can see in `config/recipe.yml`)
- python3-tkinter installed just in case

## Installation

To rebase an existing atomic Fedora installation to the latest build:

### AMD/Intel

- First rebase to the unsigned image, to get the proper signing keys and policies installed:
  ```
  rpm-ostree rebase ostree-unverified-registry:ghcr.io/polycatdev/bluecat:latest
  ```
- Reboot to complete the rebase:
  ```
  systemctl reboot
  ```
- Then rebase to the signed image, like so:
  ```
  rpm-ostree rebase ostree-image-signed:docker://ghcr.io/polycatdev/bluecat:latest
  ```
- Reboot again to complete the installation
  ```
  systemctl reboot
  ```

### AMD/Intel - Laptop

**ATTENTION:** Currently nonexistent. Request it thru a bug report and I'll create it for you.

- First rebase to the unsigned image, to get the proper signing keys and policies installed:
  ```
  rpm-ostree rebase ostree-unverified-registry:ghcr.io/polycatdev/bluecat-laptop:latest
  ```
- Reboot to complete the rebase:
  ```
  systemctl reboot
  ```
- Then rebase to the signed image, like so:
  ```
  rpm-ostree rebase ostree-image-signed:docker://ghcr.io/polycatdev/bluecat-laptop:latest
  ```
- Reboot again to complete the installation
  ```
  systemctl reboot
  ```

### Nvidia

**ATTENTION:** Currently offline. Request it thru a bug report and I'll enable the build for you.

- First rebase to the unsigned image, to get the proper signing keys and policies installed:
  ```
  rpm-ostree rebase ostree-unverified-registry:ghcr.io/polycatdev/bluecat-nvidia:latest
  ```
- Reboot to complete the rebase:
  ```
  systemctl reboot
  ```
- Then rebase to the signed image, like so:
  ```
  rpm-ostree rebase ostree-image-signed:docker://ghcr.io/polycatdev/bluecat-nvidia:latest
  ```
- Reboot again to complete the installation
  ```
  systemctl reboot
  ```

### Nvidia - Laptop

- First rebase to the unsigned image, to get the proper signing keys and policies installed:
  ```
  rpm-ostree rebase ostree-unverified-registry:ghcr.io/polycatdev/bluecat-nvidia-laptop:latest
  ```
- Reboot to complete the rebase:
  ```
  systemctl reboot
  ```
- Then rebase to the signed image, like so:
  ```
  rpm-ostree rebase ostree-image-signed:docker://ghcr.io/polycatdev/bluecat-nvidia-laptop:latest
  ```
- Reboot again to complete the installation
  ```
  systemctl reboot
  ```

## ISO

If build on Fedora Atomic, you can generate an offline ISO with the instructions available [here](https://blue-build.org/learn/universal-blue/#fresh-install-from-an-iso). These ISOs cannot unfortunately be distributed on GitHub for free due to large sizes, so for public projects something else has to be used for hosting.
