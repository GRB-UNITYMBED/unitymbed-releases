# UnityMbed — Download

**AI-native firmware IDE for Nations N32 MCUs.** Write firmware in plain language and
flash to real hardware in minutes. The Arm GCC toolchain, OpenOCD, `make` and `gdb`
are bundled — one download, nothing else to install.

> 🌐 Prefer no install? Use the web version: <https://enterpriseunitymbed.web.app>

---

## ⬇️ Download — latest **v0.1.9** (macOS) · **v0.1.24** (Windows)

### 🍎 macOS — Apple Silicon (M1 / M2 / M3 / M4)
**[UnityMbed_0.1.9_aarch64.dmg](https://github.com/GRB-UNITYMBED/unitymbed-releases/releases/download/v0.1.9/UnityMbed_0.1.9_aarch64.dmg)** · ~250 MB

Open the `.dmg`, drag **UnityMbed** to Applications, and launch — the app is
**signed & notarized by Apple**, so it opens right away (no Terminal steps).
It keeps itself up to date automatically.

### 🐧 Linux — Ubuntu 22.04+ / Debian (x86_64)
**[UnityMbed_0.1.9_amd64.deb](https://github.com/GRB-UNITYMBED/unitymbed-releases/releases/download/v0.1.9/UnityMbed_0.1.9_amd64.deb)** · ~216 MB
```
sudo apt install ./UnityMbed_0.1.9_amd64.deb
```
Dependencies and USB-probe access are configured automatically. Launch **UnityMbed**
from the application menu.

### 🪟 Windows 10 / 11 (x64)
**[UnityMbed_0.1.24_x64-setup.exe](https://github.com/GRB-UNITYMBED/unitymbed-releases/releases/download/v0.1.24/UnityMbed_0.1.24_x64-setup.exe)** · ~72 MB

Run the installer — installs per-user, no admin required. The Arm GCC toolchain, OpenOCD,
`make` and `gdb` are bundled. To flash hardware you need a CMSIS-DAP / DAPLink probe.

> Updates are manual for now — re-download this page to get a newer version.

---

## 📋 Revisions

Full history on the **[Releases page](https://github.com/GRB-UNITYMBED/unitymbed-releases/releases)** · summary in [CHANGELOG.md](CHANGELOG.md).

**v0.1.24** — 🪟 Windows, for the current test group, replacing every earlier Windows build:
plan changes on the website reach the app while you are signed in · sign-in lasts 30 days
from last use instead of 30 minutes · Manage billing opens your account page · the Ctrl+F
close button works · Compare plans opens the pricing section · billing still in **test mode**.

**v0.1.23** — 🪟 Windows, for the current test group: new look across the app in light
and dark · sign-in asks for the Terms, Privacy Policy and an 18+ confirmation (the legal
texts are the draft under legal review, marked "Beta draft") · a one-time notice before
the first AI request, with switches for the automatic AI features · credits refill on
the plan's renewal date · billing still in **test mode** · no crash reports.

**v0.1.22** — 🪟 Windows, for the current test group: sign-in, plans, licences and AI
run on the new billing service in **test mode** (invited test accounts only; building,
flashing and debugging work for everyone) · STM32 flashes with xPack OpenOCD 0.12.0-7 ·
N32G031 project examples · export a project bundle, add folders, click a GCC error to jump
to the line · the installer stops OpenOCD, GDB and make before an upgrade.

**v0.1.9** — 🍎 macOS: **signed & notarized** (opens with no Terminal steps) · first-run
**consent gate** (EULA · privacy · hardware-safety · AI-usage & generated-code
disclaimer) · license auto-sync (logging in also activates the CLI — Check hardware
works out of the box) · Check-hardware reliability fixes · dark-theme contrast fixes.

**v0.1.8** — 🪟 Windows: **Serial Plotter** (real-time oscilloscope window), and
old-format projects now open with a one-click manifest update.

**v0.1.7** — 🪟 **Windows** first release: self-contained installer (Arm GCC + OpenOCD +
`make` + `gdb` bundled, per-user install).

**v0.1.6** — build console scroll & resize, copy output, **Fix with AI** on failed
builds, and build-status history (macOS + Linux).
