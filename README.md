# Nexent Releases

English | [简体中文](README_CN.md)

macOS installers and the auto-update manifest for [Nexent](https://github.com/TTTABC-pri/nexent). This repository only hosts releases; it contains no source code.

## Install

Requires macOS 13 or later (Apple Silicon or Intel), with [Claude Code](https://docs.claude.com/en/docs/claude-code) and git installed.

1. Download `Nexent_<version>_universal.dmg` from the [latest release](https://github.com/TTTABC-pri/nexent-releases/releases/latest).
2. Open the dmg and drag Nexent into Applications.

### First launch

Nexent is not signed with an Apple Developer ID or notarized yet, so macOS blocks the first launch. Allow it in either of these ways:

- **System Settings**: open Nexent once. macOS says it cannot verify the developer; close that message. Then open **System Settings → Privacy & Security**, find Nexent under **Security**, click **Open Anyway**, then click **Open Anyway** in the dialog and enter your login password.
- **Terminal**:

  ```bash
  xattr -dr com.apple.quarantine /Applications/Nexent.app
  ```

You only need to do this once. Later versions install through the in-app updater (Settings → About → Check for updates).
