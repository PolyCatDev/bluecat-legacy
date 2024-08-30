# BlueCat &nbsp; [![build-ublue](https://github.com/PolyCatDev/bluecat/actions/workflows/build.yml/badge.svg)](https://github.com/PolyCatDev/bluecat/actions)

An opinionated tweaked [ublue](https://universal-blue.org/) image based on silverblue-main.

## What is this?

This is my own tweaked image deployment that I maintain for myself.

If anyone is using these images please reach out with a bug report so that I don't randomly change thing on your computer.

## Changes and Features

### Tweaks

- All the uBlue backend goodies
- Firefox removed (install web browser from software centre or cmd)
- FiraCode and Hack Nerd fonts included
- [Caffeine](https://extensions.gnome.org/extension/517/caffeine/), [Tiling Assistant](https://extensions.gnome.org/extension/3733/tiling-assistant/) and [Appindicator Support](https://extensions.gnome.org/extension/615/appindicator-support/) extensions included
- [Capitaine Cursors](https://www.gnome-look.org/p/1148692) pre-installed (change in Gnome Tweaks app)
- v4l2loopback kernel module for obs virtual webcam


### Included apps
- [Loupe](https://flathub.org/apps/org.gnome.Loupe)
- [Celluloid](https://flathub.org/apps/io.github.celluloid_player.Celluloid)
- [Calendar](https://flathub.org/apps/org.gnome.Calendar)
- [ExtensionManager](https://flathub.org/apps/com.mattjakeman.ExtensionManager)
- [Flatseal](https://flathub.org/apps/com.github.tchx84.Flatseal)
- [Gearlever](https://flathub.org/apps/it.mijorus.gearlever)
- [Steam Flatpak](https://flathub.org/apps/com.valvesoftware.Steam)
- [VSCodium](https://vscodium.com/) thanks to [qoijjj](https://copr.fedorainfracloud.org/coprs/qoijjj/vscodium/)
- [Podman](https://podman.io/) and [Docker](https://www.docker.com/)
- [Open Tablet Driver](https://opentabletdriver.net/)
- [WoeUSB](https://github.com/WoeUSB/WoeUSB) for creating Windows install drives
- python3-tkinter and python3-wxpython4 pre-installed just in case

## Installation

Instructions can be found in the [wiki](https://github.com/PolyCatDev/bluecat/wiki/BlueCat-Installation-Instructions).

## ISO

If build on Fedora Atomic, you can generate an offline ISO with the instructions available [here](https://blue-build.org/learn/universal-blue/#fresh-install-from-an-iso). These ISOs cannot unfortunately be distributed on GitHub for free due to large sizes, so for public projects something else has to be used for hosting.
