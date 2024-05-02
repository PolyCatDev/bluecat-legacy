# BlueCat &nbsp; [![build-ublue](https://github.com/blue-build/template/actions/workflows/build.yml/badge.svg)](https://github.com/blue-build/template/actions/workflows/build.yml)

An opinionated tweaked [ublue](https://universal-blue.org/) image based on silverblue-main.

## What is this?

This is my own tweaked image deployment that I maintain for myself.

If anyone is using these images please reach out with a bug report so that I don't randomly change thing on your computer.

## Changes and Features

- All the uBlue backend goodies
- Gnome Console insetad of Gnome Terminal
- VSCodium preinstalled on system level thanks to [qoijjj](https://copr.fedorainfracloud.org/coprs/qoijjj/vscodium/).
- Steam pre-installed (only for AMD/Intel)
- NeoVim pre-installed
- v4l2loopback kernel module for obs virtual webcam
- Firefox replaced with LibreWolf flatpak
- A few pre-installed flatpaks (you can see in `config/recipe.yml`)
- python3-tkinter installed just in case

## Installation

Instructions can be found in the [wiki](https://github.com/PolyCatDev/bluecat/wiki/Installation-instructions).

## ISO

If build on Fedora Atomic, you can generate an offline ISO with the instructions available [here](https://blue-build.org/learn/universal-blue/#fresh-install-from-an-iso). These ISOs cannot unfortunately be distributed on GitHub for free due to large sizes, so for public projects something else has to be used for hosting.
