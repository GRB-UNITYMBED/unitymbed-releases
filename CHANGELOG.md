# Revisions

## v0.1.24 — Windows (test group)
- Replaces every earlier Windows build; older installers are no longer offered.
- Plan changes made on the website reach the app while you are signed in: the plan name and
  the AI models follow an upgrade or a downgrade, and a plan bought on the website while the
  app is open on Free switches it without entering a key.
- Sign-in lasts 30 days from your last use (at most 90) instead of 30 minutes; when it ends,
  the app says so once. Your computers and Manage billing work again.
- Manage billing opens your account page (change or cancel the plan, Keep plan, update the card).
- The find bar (Ctrl+F) closes with its X button; Compare plans opens the pricing section.
- The installer includes the licence texts and third-party notices. Billing stays in
  **test mode** (Stripe Test). No crash reports.

## v0.1.23 — Windows (test group)
- New look across the app (Projects, editor, dialogs and panels) in light and dark; the dark
  editor matches the app, and Thai text uses IBM Plex Sans Thai.
- File and Help menus in the title bar, dialogs that fit the 960×600 minimum window, and an
  editor that works offline.
- Sign-in asks you to agree to the Terms of Service and Privacy Policy and to confirm you are
  18 or older; the Terms changed, so you are asked again at your next sign-in. The legal texts
  in the app and the installer are the draft under legal review, marked "Beta draft".
- A one-time notice before the first AI request shows what is sent to Google Gemini, with
  switches for inline completion and automatic debug analysis (Help > AI data & settings).
- Monthly credits refill on the plan's renewal date; an upgrade adds the prorated difference.
  Plan changes on the account page show the exact price first, and Keep plan undoes a
  scheduled downgrade. Billing stays in **test mode** (Stripe Test).
- This build sends no crash reports.
- SHA-256 `aca563f4d15b769a23d43baaec3ad2d1cf8f9b715bdec3725b1df273c2fbb510`.

## v0.1.22 — Windows (test group)
- Sign-in, plans, licences and AI run on the new billing service in **test mode**
  (Stripe Test). They work for invited test accounts only; other accounts see
  "Your test access has ended." Building, flashing and debugging work for everyone.
- STM32 boards on Windows flash with xPack OpenOCD 0.12.0-7, and older ST-Link (HLA)
  projects no longer fail on `reset_config` (re-create them or run `unitymbed detect --apply`).
- Project examples for N32G031 (6 examples with icons); N32G45x boards start from a blank project.
- Export a project bundle, add folders from the file tree, and click a GCC error to jump to the line.
- The installer stops OpenOCD, GDB and make inside the install folder before an upgrade or uninstall.
- SHA-256 `10a28a7e3d9c9b10854243796c5c9d69e591fd37c6ff6d17217cd89572f24c6f`.

## v0.1.8 — Windows
- **Serial Plotter** — real-time oscilloscope window, opened from the Serial Monitor
  (previously macOS/Linux only).
- Plotter-open failures now show in the monitor error bar instead of failing silently.
- Projects created by older UnityMbed versions (manifest without a top-level `mcu`)
  now open with a one-click manifest update instead of a parse error.
- Legal pages render markdown properly.

## v0.1.7 — Windows first release
- First **Windows** build — self-contained NSIS installer (`UnityMbed_0.1.7_x64-setup.exe`),
  per-user install, no admin required.
- Bundled Arm GCC toolchain, OpenOCD, `make` and `gdb` — nothing else to install.
- Flashing needs a CMSIS-DAP / DAPLink probe.
- Updates are manual for now (re-download to update).

## v0.1.6 — macOS + Linux
- Build console scrolls properly and can be resized (drag the top edge).
- Copy button for the build output.
- **Fix with AI** button on a failed build — hands the error to the assistant.
- History marks each restore point as build pass / fail.

## v0.1.5 — Linux first release + macOS
- First Linux **.deb** — self-contained (Arm GCC, OpenOCD, make bundled); USB-probe
  access set up automatically on install.
- macOS: the update prompt now opens in front of the main window.

## v0.1.1 – v0.1.4 — macOS
- Automatic updates, Bare-Metal (offline) mode, and editor / file-manager fixes.

## v0.1.0 — macOS first beta
- Self-contained `.dmg`: bundled Arm GCC + OpenOCD + make + gdb. No Homebrew required.
