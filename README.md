# AFM Group Kodi Add-ons

Kodi add-on distribution for the **TVHeadend OneDrive Archive**.

## Current status — controlled pilot

The repository's `pilot/` feed contains a working installable **TVHeadend OneDrive Archive v0.2.8** (`plugin.video.tvhonedrive`), plus Kodi repository metadata. It is a **pilot distribution**, not a declared general stable release.

On **2026-10-29**, the first **overseas macOS client** was sent an existing-Kodi installation package, with checksum-verifying downloader, pairing instructions and troubleshooting guide. **Client installation, device pairing and live playback remain unconfirmed** until the recipient reports back.

See the [first overseas Mac pilot rollout log](docs/FIRST-OVERSEAS-MAC-PILOT-2026-10-29.md) for the precise status and acceptance checklist.

## Pilot add-on

- Kodi add-on: `plugin.video.tvhonedrive`, version `0.2.8`
- Distribution file: [pilot/plugin.video.tvhonedrive/plugin.video.tvhonedrive-0.2.8.zip](pilot/plugin.video.tvhonedrive/plugin.video.tvhonedrive-0.2.8.zip)
- Verify downloads against [pilot/SHA256SUMS.txt](pilot/SHA256SUMS.txt).
- Device authorization requires an administrator-approved eight-digit pairing code. Never commit pairing codes or access links.
- Existing Kodi libraries, other add-ons and PVR settings do not need modification.

The source code, automated tests, development builds, production server configuration and credentials live outside this public distribution repository. No credentials or tokens belong here.

**Production infrastructure:** [afmgroup/tvh-onedrive-archive](https://github.com/afmgroup/tvh-onedrive-archive) (private; access required).

Maintainer: AFM Group.
