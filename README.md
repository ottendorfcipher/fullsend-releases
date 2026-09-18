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

## License and responsibility

Everything here is released under the MIT License (see [LICENSE](LICENSE)).
It is provided as is, without warranty of any kind, and the authors accept
no liability arising from its use.

fullSend is self-hosted software. Whoever installs and runs a station is
that station's operator: they control who can join, what is said and stored
on it, and how long transcripts are kept, and they are responsible for
running it lawfully where they are, including any consent needed to record
or retain voice and text. The authors do not operate, monitor, or have
access to stations run by others. A station's only outbound contact is the
operator-triggered update check against this repository; nothing on a
station is sent to the authors.
