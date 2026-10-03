# Cams for Linux

Builds of Cams, a viewer for Wyze cameras, for 64-bit Linux (x86_64). Only the
builds are here; the source is private.

Each release has two files:

- `Cams-<version>-linux-x86_64.tar.gz`: unpack it and run `sh install.sh`
  (no admin password; it installs for your user). Its README.txt says more.
- `latest.json`: what an installed Cams checks when it's opened. When a newer
  version is out, it downloads it, checks that its SHA-256 matches and that
  the release is signed with the key built into Cams, and opens the new one.

Cams includes [go2rtc](https://github.com/AlexxIT/go2rtc) (MIT License); its
license is in THIRD-PARTY.txt in the package.
