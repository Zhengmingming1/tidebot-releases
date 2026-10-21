# tidebot releases

Download page and update channel for tidebot, a small local scheduler for Claude Code tasks. This repo only holds the release files, the release notes and the signed update manifest (`latest.json`) that installed copies check.

**Source code:** [github.com/Zhengmingming1/tidebot](https://github.com/Zhengmingming1/tidebot). It's open source under the [GNU AGPL-3.0-only](https://github.com/Zhengmingming1/tidebot/blob/main/LICENSE). Issues, PRs and security reports ([SECURITY.md](https://github.com/Zhengmingming1/tidebot/blob/main/SECURITY.md)) go there.

## Download

| You have | File |
|---|---|
| macOS (Apple Silicon or Intel) | [tidebot-desktop-macOS-AppleSilicon-Intel.dmg](https://github.com/Zhengmingming1/tidebot-releases/releases/latest/download/tidebot-desktop-macOS-AppleSilicon-Intel.dmg) |
| Windows 10/11 x64 | [tidebot-desktop-Windows-x64-Setup.exe](https://github.com/Zhengmingming1/tidebot-releases/releases/latest/download/tidebot-desktop-Windows-x64-Setup.exe) |
| Linux x64, desktop | [AppImage](https://github.com/Zhengmingming1/tidebot-releases/releases/latest/download/tidebot-desktop-Linux-x64.AppImage) · [.deb](https://github.com/Zhengmingming1/tidebot-releases/releases/latest/download/tidebot-desktop-Linux-x64.deb) |
| A server (no GUI) | `tidebot-server_<version>_<os>_<arch>.tar.gz` / `.zip` / `.deb` on the [latest release](https://github.com/Zhengmingming1/tidebot-releases/releases/latest) |

Every release has `SHA256SUMS`. Check a file with `sha256sum -c --ignore-missing SHA256SUMS`.

## Updates

tidebot checks `latest.json` here about once a day (you can turn that off in Settings → About). The manifest is signed with an ed25519 key whose public half is built into tidebot, and every download is checked against the sha256 in the manifest before anything is replaced. Nothing is sent besides the plain HTTPS download; there is no telemetry. Only the official builds from this page replace themselves. A copy you build from source just tells you a new release exists ([details](https://github.com/Zhengmingming1/tidebot/blob/main/docs/building.md)).

## About Anthropic

tidebot drives the Claude Code CLI on your machine with your own key or subscription. It is not affiliated with, endorsed by, or sponsored by Anthropic. "Claude" and "Claude Code" are trademarks of Anthropic.
