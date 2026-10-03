# Cams for Linux

Builds of Cams, a viewer for Wyze cameras, for 64-bit Linux (x86_64). Only the
builds are here; the source is private.

## Install or update

In a terminal (no sudo; it installs for your user):

    wget -qO- https://github.com/fuelingtheweb/cams-linux/releases/latest/download/install.sh | sh

`curl -fsSL <same address> | sh` works too. It downloads the newest package,
checks its SHA-256 against `latest.json`, and runs the package's `install.sh`.
Running it again updates Cams and keeps your Wyze sign-in. Once installed,
Cams also updates itself when it's opened.

## What each release has

- `Cams-<version>-linux-x86_64.tar.gz`: the package. Unpack it and run
  `sh install.sh` to install by hand. Its README.txt says more.
- `install.sh`: the one-step installer above.
- `latest.json`: what an installed Cams checks when it's opened. When a newer
  version is out, it downloads it, checks that its SHA-256 matches and that
  the release is signed with the key built into Cams, and opens the new one.

Cams includes [go2rtc](https://github.com/AlexxIT/go2rtc) (MIT License); its
license is in THIRD-PARTY.txt in the package.
