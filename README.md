# UnityMbed — Download

**AI-native firmware IDE for Nations N32 MCUs.** Write firmware in plain language and
flash to real hardware in minutes. The Arm GCC toolchain, OpenOCD, `make` and `gdb`
are bundled — one download, nothing else to install.

> 🌐 Prefer no install? Use the web version: <https://enterpriseunitymbed.web.app>

---

## ⬇️ Download — latest **v0.1.6**

### 🍎 macOS — Apple Silicon (M1 / M2 / M3 / M4)
**[UnityMbed_0.1.6_aarch64.dmg](https://github.com/GRB-UNITYMBED/unitymbed-releases/releases/download/v0.1.6/UnityMbed_0.1.6_aarch64.dmg)** · ~248 MB

Open the `.dmg`, drag **UnityMbed** to Applications. Not notarized yet, so on the first
launch run this once in Terminal:
```
xattr -dr com.apple.quarantine /Applications/UnityMbed.app
```
After that the app keeps itself up to date automatically.

### 🐧 Linux — Ubuntu 22.04+ / Debian (x86_64)
**[UnityMbed_0.1.6_amd64.deb](https://github.com/GRB-UNITYMBED/unitymbed-releases/releases/download/v0.1.6/UnityMbed_0.1.6_amd64.deb)** · ~216 MB
```
sudo apt install ./UnityMbed_0.1.6_amd64.deb
```
Dependencies and USB-probe access are configured automatically. Launch **UnityMbed**
from the application menu.

### 🪟 Windows
Coming soon.

---

## 📋 Revisions

Full history on the **[Releases page](https://github.com/GRB-UNITYMBED/unitymbed-releases/releases)** · summary in [CHANGELOG.md](CHANGELOG.md).

**v0.1.6** — build console scroll & resize, copy output, **Fix with AI** on failed
builds, and build-status history (macOS + Linux).
