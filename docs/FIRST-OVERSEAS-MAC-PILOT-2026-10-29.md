# First overseas Kodi archive client — rollout log

**Date:** 2026-10-29 (America/Toronto)  
**Rollout:** First overseas client, existing Kodi installation on macOS  
**Distribution:** AFM Group Kodi add-ons **pilot feed**, TVHeadend OneDrive Archive `plugin.video.tvhonedrive` v0.2.8  
**State:** **Installation kit sent; installation, pairing approval and overseas playback not yet confirmed.**

## What was sent

- A Mac-specific **existing-Kodi** client kit, version v0.2.8, avoiding any unnecessary Kodi installation or changes to existing media sources, PVR clients or libraries.
- Two-page quick-start PDF, `START_HERE` instructions, checksum-verifying download helper and troubleshooting notes.
- Distribution source: `pilot/plugin.video.tvhonedrive/plugin.video.tvhonedrive-0.2.8.zip`.
- Published SHA-256: `ae005f253b782ab6191c124a356b18e4564463780092512212ca761dfb779cc8`. The source download was verified against the published checksum before the client kit was prepared.
- No Microsoft account credentials, OneDrive tokens, persistent gateway links or server-side secrets were included.

## End-user procedure

1. Open their **existing Kodi** on macOS (check Kodi version if compatibility problems arise).
2. Download and verify the v0.2.8 add-on package using the kit.
3. In Kodi, use **Add-ons → Install from zip file** and choose the `plugin.video.tvhonedrive-0.2.8.zip` (not the enclosing client-kit ZIP).
4. Under **Video add-ons**, launch **TVHeadend OneDrive Archive**, then choose **Pair this device (8-digit code)**.
5. Send the displayed short code privately to the administrator for one-device approval; do not send passwords or account tokens.
6. After approval, verify that archived recordings list and play over the overseas connection. Check seeking and playback continuation.

Existing Kodi configuration should remain unchanged. This add-on supplies a separate cloud archive and is **not** a replacement for the existing TVHeadend PVR client.

## Admin acceptance checklist

- [x] Pilot add-on v0.2.8 identified in repository metadata.
- [x] Published add-on ZIP checksum matched.
- [x] Existing-Kodi Mac package prepared and sent to the first overseas viewer.
- [ ] Client confirms installed Kodi-compatible add-on.
- [ ] Eight-digit device pairing code received.
- [ ] Device approved and labelled through the existing gateway admin workflow.
- [ ] Remote archived recording listing and playback confirmed.
- [ ] Seek/resume behavior verified or any issues documented.
- [ ] Record final deployment outcome and revise this log.

## Release classification and privacy

This is a **controlled overseas pilot**, not a general public stable release. Do not claim a successful live overseas installation until the recipient confirms. Do not include client name, location, pairing codes, device secrets, or gateway access links in GitHub. Keep administrator-controlled approval, link expiry and revocation in place.

**Related production project:** `afmgroup/tvh-onedrive-archive` (closed production server-side rollout, 2026-10-26). A successful Mac pilot does not change its server retention policy.
