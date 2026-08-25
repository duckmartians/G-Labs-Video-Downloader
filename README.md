# G-Labs Video Downloader

**English** | [Tiếng Việt](README.vi.md)

Desktop app for downloading videos from **YouTube, TikTok, Facebook, Instagram, X/Twitter, Twitch, Vimeo, Reddit, SoundCloud, Bilibili and 1,800+ other sites** — with a bundled self-updating multi-platform download engine. Everything ships in the app; nothing else to install.

![Main window](docs/screenshots/01-main.png)

## Features

- **Paste anything**: single videos, playlists, whole channels, YouTube Shorts — one link per line for bulk adds; a **?** button opens a detailed guide of every supported platform & link shape
- **Formats**: MP4 (best / 1080p / 720p / 480p) · MP3 192 kbps · thumbnail JPG · subtitles SRT · **extras-only mode** (thumbnail/subtitles without downloading the video)
- **Parallel queue**: 1–10 concurrent downloads with per-item progress, speed and ETA; **status filters** (in-progress / finished / errors / canceled) plus row selection with bulk "run selected"
- **Playlist / channel preview**: fetch the item list first, tick exactly what you want (Videos/Shorts tabs for YouTube channels)
- **Smart dedup**: persistent download history skips videos you already have (per format) — one click to re-download anyway
- **Retry**: per-item and retry-all for failed downloads (plus the engine's own retry with backoff)
- **Export CSV**: queue + errors, Excel-friendly (UTF-8 BOM); activity log with copy/export buttons
- **Cookies quick-import**: paste ANY format — Netscape `cookies.txt`, browser-extension JSON export, or a raw `a=1; b=2` header string — per platform or global, for age-restricted / login-required content
- **Proxy pool**: paste a LIST of proxies (any format — `host:port:user:pass`, `user:pass@host:port`, full `socks5://` URLs, IPv6) — each download rotates through them round-robin; one-click "test all"
- **Self-updating engine**: the download engine updates itself every 24 h (+ manual button) so YouTube changes don't break you
- **App auto-update**: checks GitHub Releases, downloads and installs in-app
- **6 languages**: English, Tiếng Việt, 简体中文, Español, العربية (RTL), Русский

## Screenshots

| Playlist / channel preview | Supported-links guide |
|---|---|
| ![Preview](docs/screenshots/02-preview.png) | ![Help](docs/screenshots/03-help.png) |

| Cookie quick-import | Proxy pool (round-robin) |
|---|---|
| ![Cookies](docs/screenshots/04-cookies.png) | ![Proxy](docs/screenshots/05-proxy.png) |

| Download history | RTL (العربية) |
|---|---|
| ![History](docs/screenshots/06-history.png) | ![RTL](docs/screenshots/07-rtl-arabic.png) |

## Install

Grab the latest from [Releases](https://github.com/duckmartians/G-Labs-Video-Downloader/releases):

- **Windows**: `GLabsVideoDownloader-<version>-setup.exe`
- **macOS (Apple Silicon)**: `GLabsVideoDownloader-<version>-arm64.dmg` — unsigned; first open: right-click → Open, or `xattr -dr com.apple.quarantine "/Applications/G-Labs Video Downloader.app"`

Settings and history live in the OS per-user data folder (`%APPDATA%\G-Labs Video Downloader` on Windows, `~/Library/Application Support/G-Labs Video Downloader` on macOS). Downloads default to `Documents/G-Labs Video Downloader`.
