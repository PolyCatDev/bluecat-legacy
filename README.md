# BlueCat &nbsp; [![build-ublue](https://github.com/PolyCatDev/bluecat/actions/workflows/build.yml/badge.svg)](https://github.com/PolyCatDev/bluecat/actions)

An opinionated tweaked [ublue](https://universal-blue.org/) image based on silverblue-main.

## What is this?

This is my own tweaked image deployment that I maintain for myself.

If anyone is using these images please reach out with a bug report so that I don't randomly change thing on your computer.

## Changes and Features

- All the uBlue backend goodies
- Firefox removed (install web browser from software centre or cmd)
- [Capitaine Cursors](https://www.gnome-look.org/p/1148692) pre-installed (change in Gnome Tweaks app)
- VSCodium preinstalled on system level thanks to [qoijjj](https://copr.fedorainfracloud.org/coprs/qoijjj/vscodium/)
- Steam flatpak pre-installed
- v4l2loopback kernel module for obs virtual webcam
- A few pre-installed core gnome flatpak apps
- WoeUSB installed for creating Windows install drives
- python3-tkinter and gcc preinstalled just in case

## Installation

Instructions can be found in the [wiki](https://github.com/PolyCatDev/bluecat/wiki/BlueCat-Installation-Instructions).

## ISO

If build on Fedora Atomic, you can generate an offline ISO with the instructions available [here](https://blue-build.org/learn/universal-blue/#fresh-install-from-an-iso). These ISOs cannot unfortunately be distributed on GitHub for free due to large sizes, so for public projects something else has to be used for hosting.
