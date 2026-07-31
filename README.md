# Dead Weight — release channel

Packaged Windows builds of the **Dead Weight** client, and the `manifest.json`
each build is described by. Nothing else lives here: no source, no design
documents, no server code.

## Getting the game

Grab the latest zip from [Releases](../../releases). Unzip it anywhere and run
`DeadWeight.exe`. There is no installer.

The client updates itself: at boot it reads the `channel-public` manifest from
this repository, and if a newer build is listed it downloads and swaps itself
before you sign in. You should not need to come back here after the first
download.

## Channels

`channel-public` is a release tag that is updated in place and always holds the
current manifest for that channel. Every versioned build is also kept as its own
release, so a rollback is just repointing the channel manifest at an older
asset.

## Status

Alpha. It connects to a single small server; expect it to be down sometimes, and
expect to lose progress between builds.

## Reporting problems

Press F12 in game to file a bug report — it carries the logs with it, which is
far more useful than a description. Otherwise open an issue here.

---

Built from a private source repository. Third-party asset licences travel inside
each build; the character rig and its animations are Quaternius' Universal
Animation Library (CC0).
