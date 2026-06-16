# FocusOS — Releases

Public distribution + auto-update feed for **FocusOS** (the source lives in a
private repo). Each release ships a notarized `.dmg` as a GitHub Release asset,
and the [Sparkle](https://sparkle-project.org) auto-updater reads
[`appcast.xml`](appcast.xml) to deliver updates to installed apps.

## Install

Download the latest `FocusOS-x.y.z.dmg` from
**[Releases](https://github.com/kflmhm/focusos-releases/releases/latest)**, open
it, and drag **FocusOS** to Applications.

## Updates

The app checks this feed automatically and prompts when a new version is
available. You can also trigger a check from **Settings → Check for Updates…**.

The update feed URL is:

```
https://raw.githubusercontent.com/kflmhm/focusos-releases/main/appcast.xml
```

Updates are cryptographically verified with an EdDSA (Ed25519) signature in
addition to the app's Developer ID notarization.
