# fullSend — releases

Release assets for the fullSend station host, published here so that
installed stations (whose source lives in a private repository) can fetch
updates without credentials.

Each release carries:

- `fullsend-server-<target-triple>[.exe]` — the station binary per platform
- `fullsend-server_<version>_amd64.deb`, `fullsend-server-<version>.pkg`,
  `fullsend-server-<version>-x64.msi`, `PKGBUILD` — installers
- `manifest.json` + `manifest.json.sig` — the signed update manifest a
  station verifies against the public key built into its binary

Nothing here is meant to be built; the source and the release workflow are
in the private `fullsend-comms` repository.
