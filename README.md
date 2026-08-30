<div align="center">

<img src="assets/logo.png" width="128" height="128" alt="drog.ai Code logo" />

# drog.ai Code

### A native Windows AI code editor — official release channel

[![Latest release](https://img.shields.io/github/v/release/deepdrogo/drogai_windows_editor_releases?label=latest&sort=semver&color=2ea043)](https://github.com/deepdrogo/drogai_windows_editor_releases/releases/latest)
[![Downloads](https://img.shields.io/github/downloads/deepdrogo/drogai_windows_editor_releases/total?color=1f6feb&label=downloads)](https://github.com/deepdrogo/drogai_windows_editor_releases/releases)
[![Platform](https://img.shields.io/badge/platform-Windows%20x64-0078D6?logo=windows&logoColor=white)](#-download)
[![Auto update](https://img.shields.io/badge/updates-automatic-8957e5)](#-automatic-updates)
[![Release date](https://img.shields.io/github/release-date/deepdrogo/drogai_windows_editor_releases?color=57606a&label=released)](https://github.com/deepdrogo/drogai_windows_editor_releases/releases/latest)

<a href="https://github.com/deepdrogo/drogai_windows_editor_releases/releases/latest"><b>⬇️&nbsp;&nbsp;Download the latest version for Windows</b></a>

</div>

---

> **drog.ai Code** is a fast, native Windows editor with a built-in AI agent, powered by the [drog.ai](https://drog.ai) platform.
> This repository is its **public release channel** — every installer and every automatic update is served from here.
> The application source lives in a separate, private repository.

## ✨ Features

- 🤖 **AI agent, five modes** — `plain`, `checkpoint`, `agent`, `long task`, and 🛡️ **CyberSecurity** — each tuned for a different job, from a single question to a multi-stage build.
- 🛡️ **CyberSecurity Agent** — drives a real penetration-testing toolchain (Nmap, Wireshark, Burp Suite, John the Ripper, …) against a target you name, with a prompt-template library and terminal-style reports. Unlocked per account from the drog.ai admin panel.
- 🌐 **Remote workspaces over SSH** — open a folder on another machine and work on it as if it were local.
- 💻 **Integrated terminal, language servers & diagnostics** — real LSP, a problems panel, and a full terminal.
- ⚡ **AI autocomplete and inline edits** — with restore points you can rewind to at any step.
- 🧩 **Monaco editor core** plus MCP tool integrations and a browser tool.
- 🔒 **No provider keys on your machine** — the drog.ai gateway owns authentication and metering; the editor is a licensed client.

## ⬇️ Download

1. Open the **[latest release](https://github.com/deepdrogo/drogai_windows_editor_releases/releases/latest)**.
2. Download **`drog.ai_Code_<version>_x64-setup.exe`**.
3. Run it — the installer is per-user, so no administrator rights are needed.
4. Launch **drog.ai Code** and sign in with your drog.ai account.

> 💡 Deploying by policy? Every release also ships an **MSI**.

## 🔄 Automatic updates

drog.ai Code keeps itself current from this repository:

- On launch and on demand it checks the **[latest release](https://github.com/deepdrogo/drogai_windows_editor_releases/releases/latest)**.
- A newer version → the app offers a one-click **Install**; already newest → it tells you **you’re up to date**.
- Every update package is verified with a **minisign signature** before it is installed — the app refuses anything it cannot authenticate.

You never have to re-download by hand after the first install.

## 📦 What’s in each release

| Asset | Purpose |
| --- | --- |
| `drog.ai_Code_<version>_x64-setup.exe` | Windows installer (per-user, NSIS). |
| `drog.ai_Code_<version>_x64_en-US.msi` | MSI, for managed / policy deployment. |
| `latest.json` | The updater manifest the app reads. |
| `*.sig` | Detached minisign signature, for verification. |

## 🧭 How the update channel works

```text
drog.ai Code  ──►  releases/latest/download/latest.json  ──►  verify signature  ──►  install
```

The app reads the newest release from this repo, compares versions, and installs only a package whose signature matches the key built into it.

## 🔐 Source & licensing

The application is proprietary. This repository distributes **release artifacts only**; the source is private. See each release’s notes for what changed.

<div align="center">
<sub>© 2026 drog.ai · Built for Windows</sub>
</div>
