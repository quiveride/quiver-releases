# Quiver — Release Mirror

This repository hosts the **release artifacts** (macOS DMGs +
electron-builder metadata) for [Quiver](https://github.com/quiveride/quiver),
a cross-project navigator for Claude Code sessions.

## Downloads

See the [**Releases**](https://github.com/quiveride/quiver-releases/releases)
tab for the latest DMG.

Two builds per release:

| File | For |
|---|---|
| `Quiver-<ver>-arm64.dmg` | Apple Silicon Macs (M1 / M2 / M3 / M4 / …) |
| `Quiver-<ver>-x64.dmg`   | Intel Macs |

First-time install on macOS:

1. Open the DMG, drag **Quiver** into Applications.
2. The first time you launch, macOS will show *"Quiver can't be opened
   because the developer cannot be verified"* — this is expected for now
   (the build is not yet signed with an Apple Developer certificate).
3. Right-click the app → **Open** → **Open** to bypass Gatekeeper. You
   only need to do this once.

## Source

The Quiver source code lives at <https://github.com/quiveride/quiver>
(currently private). Issues and discussions belong on that repo.

## Why a separate repo?

The source is private but the binaries need to be reachable by the app's
in-app update notifier without requiring auth. Splitting the release
artifacts into a public mirror solves that without exposing source code.
