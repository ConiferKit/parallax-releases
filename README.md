# Parallax

Every coding agent you run, in one place. Connect Claude Code, Codex and the rest, use your own subscriptions in the
exact harness you want, switch models with Parallax's built-in router, watch every session live, and steer any of them.

This repository holds the public releases of Parallax for Mac, plus the `parallax` command for Linux.

## Install

**Download the app:** [**Parallax-macos.dmg**](https://github.com/ConiferKit/parallax-releases/releases/latest/download/Parallax-macos.dmg).
Open it and drag Parallax to Applications.

**Or install from a terminal:**

```sh
d=$(mktemp -d) && curl -fsSLo "$d/install.sh" https://github.com/ConiferKit/parallax-releases/releases/latest/download/install.sh && sh "$d/install.sh"
```

The terminal install puts the app in `/Applications` (or in `~/Applications` if you can't write to `/Applications`).
It also puts the `parallax` command in `~/.local/bin`.

On Linux (x86-64 or arm64), the same line installs the `parallax` command and starts its daemon. Then open
http://127.0.0.1:7878.

## Requirements

- macOS 12 Monterey or later.
- Apple silicon or Intel: the app is universal.

## Signed and notarized

Parallax is signed with an Apple Developer ID and notarized by Apple. Apple's ticket is stapled to both the app and the
dmg, so the app opens with a double-click and no warning, even offline.

## Updates

Parallax updates itself. When a new release is published here, the app downloads it and installs it at an idle moment,
with nothing to click. Your running sessions carry on across the update.

To review each update before it installs, turn off **Update automatically** in Settings.

## Files in each release

| File | What it is |
| --- | --- |
| `Parallax-macos.dmg` | The Mac app, to drag to Applications |
| `install.sh` | The terminal installer above |
| `Parallax-macos-arm64.zip` | The same app, zipped. The updater downloads this. Despite the name, it is universal. |
| `parallax-<os>-<arch>.tar.gz` | The `parallax` command alone, for macOS and Linux |
| `SHA256SUMS` | Checksums for every file |

Each file is also published under its versioned name, for example `Parallax-v1.0.0-macos.dmg`. The links above always
point to the newest release.

## Feedback

Found a bug or want a feature? [Open an issue](https://github.com/ConiferKit/parallax-releases/issues/new).
