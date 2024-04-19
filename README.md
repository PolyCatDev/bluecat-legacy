# BlueCat &nbsp; [![build-ublue](https://github.com/blue-build/template/actions/workflows/build.yml/badge.svg)](https://github.com/blue-build/template/actions/workflows/build.yml)

An opinionated tweaked [ublue](https://universal-blue.org/) image of silverblue-main.

## Changes and Features
- All the uBlue backend goodies
- Gnome Console insetad of Gnome Terminal
- Steam pre-installed (only for AMD/Intel)
- NeoVim pre-installed
- v4l2loopback kernel module for obs virtual webcam (currently not enabled)
- Firefox replaced with LibreWolf flatpak
- A few pre-installed flatpaks (you can see in `config/recipe.yml`)

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

### Nvidia

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

The `latest` tag will automatically point to the latest build. That build will still always use the Fedora version specified in `recipe.yml`, so you won't get accidentally updated to the next major version.

## ISO

If build on Fedora Atomic, you can generate an offline ISO with the instructions available [here](https://blue-build.org/learn/universal-blue/#fresh-install-from-an-iso). These ISOs cannot unfortunately be distributed on GitHub for free due to large sizes, so for public projects something else has to be used for hosting.

## Verification

These images are signed with [Sigstore](https://www.sigstore.dev/)'s [cosign](https://github.com/sigstore/cosign). You can verify the signature by downloading the `cosign.pub` file from this repo and running the following command:

```bash
cosign verify --key cosign.pub ghcr.io/blue-build/legacy-template
```
