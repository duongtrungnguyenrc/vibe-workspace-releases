# Vibe Workspace — desktop releases

Installers for the Vibe Workspace desktop app, and the feed the app checks for automatic updates. The source lives in a
private repository; this one only holds releases.

## Download

Open the [latest release](https://github.com/duongtrungnguyenrc/vibe-workspace-releases/releases/latest) and pick the
file for your machine:

| System | File |
| --- | --- |
| macOS, Apple silicon | `Vibe-Workspace-<version>-mac-arm64.dmg` |
| macOS, Intel | `Vibe-Workspace-<version>-mac-x64.dmg` |
| Windows | `Vibe-Workspace-<version>-win-x64.exe` (installer) |
| Linux | `Vibe-Workspace-<version>-linux-x86_64.AppImage` or `.deb` |

`SHA256SUMS.txt` in each release lists the checksum of every file.

## Updates

The app checks this repository for new versions and installs them from **About & updates** in its settings. Beta
versions are published as pre-releases and only reach installs that chose the beta channel.

- **macOS:** automatic updates need a signed build. While builds are unsigned, the app links here instead; the first
  launch may need right-click → Open (or `xattr -dr com.apple.quarantine "/Applications/Vibe Workspace.app"`).
- **Windows:** the installer updates itself. SmartScreen may warn about an unsigned build: More info → Run anyway.
- **Linux:** the AppImage updates itself; `.deb` installs get a link to the new version.
