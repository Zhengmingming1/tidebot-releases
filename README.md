# tidebot releases

Download page for [tidebot](https://github.com/Zhengmingming1/tidebot), a small local scheduler for Claude Code tasks. The source repository is private for now; this repo only holds the release files, the release notes and a signed update manifest. There is no source code here.

## Download

| You have | File |
|---|---|
| macOS (Apple Silicon or Intel) | [tidebot-desktop-macOS-AppleSilicon-Intel.dmg](https://github.com/Zhengmingming1/tidebot-releases/releases/latest/download/tidebot-desktop-macOS-AppleSilicon-Intel.dmg) |
| Windows 10/11 x64 | [tidebot-desktop-Windows-x64-Setup.exe](https://github.com/Zhengmingming1/tidebot-releases/releases/latest/download/tidebot-desktop-Windows-x64-Setup.exe) |
| Linux x64, desktop | [AppImage](https://github.com/Zhengmingming1/tidebot-releases/releases/latest/download/tidebot-desktop-Linux-x64.AppImage) · [.deb](https://github.com/Zhengmingming1/tidebot-releases/releases/latest/download/tidebot-desktop-Linux-x64.deb) |
| A server (no GUI) | `tidebot-server_<version>_<os>_<arch>.tar.gz` / `.zip` / `.deb` on the [latest release](https://github.com/Zhengmingming1/tidebot-releases/releases/latest) |

Every release has `SHA256SUMS`. Check a file with `sha256sum -c --ignore-missing SHA256SUMS`.

## Updates

tidebot checks `latest.json` here about once a day (you can turn that off in Settings → About). The manifest is signed with an ed25519 key whose public half is built into tidebot, and every download is checked against the sha256 in the manifest before anything is replaced. Nothing is sent besides the plain HTTPS download; there is no telemetry.

## About Anthropic

tidebot drives the Claude Code CLI on your machine with your own key or subscription. It is not affiliated with, endorsed by, or sponsored by Anthropic. "Claude" and "Claude Code" are trademarks of Anthropic.
