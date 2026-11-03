# Sumi releases

Download the latest Sumi for Mac from [Releases](https://github.com/hsiaoming/sumi-releases/releases/latest).

Every release carries:

- `Sumi_<version>_aarch64.dmg` and `Sumi_<version>_x64.dmg` — installers for Apple Silicon and Intel;
- `Sumi_<version>_<arch>.app.tar.gz` and its `.sig` — the archive the in-app updater downloads;
- `latest.json` — the signed update manifest the app reads from
  <https://github.com/hsiaoming/sumi-releases/releases/latest/download/latest.json>.

The `.sig` files are minisign signatures made with Sumi's updater key; the app verifies them against the public key
compiled into the binary. Releases are written by the `Release` workflow in the Sumi app repository, not by hand.
