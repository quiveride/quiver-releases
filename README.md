# Quiver — Downloads & Releases

Release artifacts (macOS DMGs + auto-update metadata) for **Quiver**, a desktop
**session manager for Claude Code & Codex**: every terminal coding-agent session
across every project — local or over SSH — in one window, with the real
terminal, real git diff, per-block staging, and a real shell.

- **Website:** <https://quiveride.github.io/>
- **Download the latest build:** [**Releases**](https://github.com/quiveride/quiver-releases/releases/latest)

## Install (macOS)

| File | For |
|---|---|
| `Quiver-<ver>-arm64.dmg` | Apple Silicon Macs (M1 / M2 / M3 / M4 / …) |
| `Quiver-<ver>-x64.dmg`   | Intel Macs |

1. Open the DMG and drag **Quiver** into Applications.
2. On first launch macOS may say *“Quiver can’t be opened because the developer
   cannot be verified.”* Right-click the app → **Open** → **Open** to approve it
   once. (Code signing & notarization are being rolled out; until a release is
   fully notarized this one-time step is expected.)

Quiver checks this repo for new releases and can update itself in place.

## Issues & ideas

Bug reports, feature requests, and discussions live **here**, in this repo’s
[**Issues**](https://github.com/quiveride/quiver-releases/issues) — the source
repository is private and code-only, so this public repo is Quiver’s tracker.

## Why a separate repo?

Quiver’s source is private, but the binaries must be reachable by the in-app
updater without authentication. This public repo carries the release artifacts
(`*.dmg`, `*.zip`, `latest-mac.yml`, blockmaps) and the issue tracker; the
source stays private.
