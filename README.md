# Memoresse public releases

Downloads of the Memoresse desktop apps. The source lives in private
repositories; this repo only hosts the release assets.

## MemPlayer

Opens a `.mem` memory file and shows the memory inside: the story, the
people, and the photos, videos, voice notes and notes. Read-only and
offline: no account, no cloud.

- **Latest release**: [releases/latest](https://github.com/Memoresse/Memoresse-public-releases/releases/latest)
- **Staging build** (every change, may be rough): [mem-player-staging](https://github.com/Memoresse/Memoresse-public-releases/releases/tag/mem-player-staging)

| Platform | Asset |
| --- | --- |
| macOS, Apple silicon | `MemPlayer-<version>-macos-arm64.zip` |
| Windows, x64 | `MemPlayer-<version>-windows-x64.zip` |

### Opening an unsigned build

The builds are not code-signed yet, so the operating system warns on the
first launch. This is expected; the steps below are needed once.

**macOS**

1. Unzip and move `MEM Player.app` to Applications.
2. Open it once. macOS says it cannot be opened. Close that dialog.
3. Open System Settings, Privacy & Security, scroll down and click
   **Open Anyway**, then confirm.

Or in Terminal: `xattr -d com.apple.quarantine "/Applications/MEM Player.app"`.

**Windows**

1. Unzip; the `MemPlayer` folder can live anywhere, for example in Documents.
2. Run `mem_player.exe`. SmartScreen says "Windows protected your PC".
3. Click **More info**, then **Run anyway**.

The browser may also flag the download as uncommon; keep it.
