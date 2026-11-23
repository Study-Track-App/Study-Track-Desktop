# Study-Track Desktop

Official desktop releases for **Study-Track**, a study planner and focus tracker for students.

This repository distributes the **macOS and Windows installers** and update files used by the Study-Track desktop apps. It is a release repository, not the desktop application's source code.

**[Study-Track website](https://study-track.app)** · **[Download for desktop](https://study-track.app/downloads)** · **[Documentation](https://docs.study-track.app)**

## Download Study-Track

**Get the desktop app from the official [Study-Track downloads page](https://study-track.app/downloads).**

That page is the recommended starting point: it provides the appropriate download for your platform and instructions when an existing installation needs to be replaced.

You can also browse the [GitHub Releases](https://github.com/Study-Track-App/Study-Track-Desktop/releases) published in this repository. Releases appear here as they are approved and rolled out; a build being tested is not necessarily available to everyone yet.

## Platforms and updates

| Platform | Distribution | How updates arrive |
|---|---|---|
| macOS | Direct download | The installed app checks the Study-Track update feed |
| Windows | Direct download | The installed app checks the Study-Track update feed |
| macOS | Mac App Store, when available | Updates are managed by Apple |
| Windows | Microsoft Store, when available | Updates are managed by Microsoft |

The desktop apps load the live Study-Track web experience. Most website improvements therefore appear without downloading a new installer. A new desktop release is needed when the native application itself changes.

If you are using an older Mac release, you may need to **download and install a newer app once** because the macOS application identifier changed. Follow the instructions on the [downloads page](https://study-track.app/downloads); your Study-Track account and cloud-saved study data are not tied to the old installer.

## What this repository contains

Published releases may include:

- Signed macOS installers and the archives required for native updates.
- Windows installers and their update assets.
- Versioned release artifacts and checksums or update metadata.

**This repository does not contain the desktop source code, student account data, or signing credentials.** It exists to keep downloads and update assets separate from the web application's deployment.

## How releases work

1. Changes to the Study-Track desktop application are built and checked by GitHub Actions in the main application repository.
2. New native builds are signed and verified before release.
3. An explicitly started release workflow publishes the approved direct-download binaries here.
4. A separate change updates the official download and update feed after verification.
5. Installed direct-download apps use that feed to discover updates. Store-distributed builds use their respective stores.

A website deployment alone does **not** create a new installer or publish a store update.

Release procedures, platform-specific verification and rollback instructions belong in the [Study-Track engineering documentation](https://docs.study-track.app), not in this artifact repository.

## Related repositories

| Repository | Purpose |
|---|---|
| [Study-Track](https://github.com/flodlol/Study-Track) | Main web application, Firebase backend, desktop application code and release automation |
| [Study-Track-Mobile](https://github.com/Study-Track-App/Study-Track-Mobile) | iOS and Android application |
| [Study-Track-Docs](https://github.com/Study-Track-App/Study-Track-Docs) | Canonical technical and product documentation |
| **Study-Track-Desktop** (this repository) | Public desktop installers, releases and update artifacts |

Some development repositories are private; use the [public documentation](https://docs.study-track.app) for product guides and general information.

## Help and feedback

For installation help, update issues or feature information, start at [study-track.app](https://study-track.app) or [docs.study-track.app](https://docs.study-track.app).

If an update fails, include your operating system, installed app version and how the app was installed when reporting the problem. **Never post passwords, tokens, signing certificates or personal study data.**

---

Study-Track is proprietary software. The availability of release artifacts here does not grant permission to redistribute or modify the application outside the applicable terms.
