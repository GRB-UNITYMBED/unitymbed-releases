# Revisions

## v0.1.27 — Windows and Linux
- Faster editor: typing no longer stalls on large projects; less CPU when idle.
- STM32: New project offers a Blank project only; pick or type the chip instead of
  auto-detect. A missing ST-Link driver message links to ST's STSW-LINK009 download.
- Welcome tour on the Projects page and one-time Editor tips.
- Sign in turns into the account menu right away; Your computers shows each computer's name.
- AI chat treats the open file as the source of truth.
- Thin hover-only tab scrollbar; the mouse wheel scrolls the tabs. Icons instead of emoji.
- Windows: updates arrive in the app from 0.1.26. File access stays inside the project
  folder; build and debug tools stop with the app even after a crash.
- macOS stays on 0.1.26 for now.
- SHA-256 `UnityMbed_0.1.27_x64-setup.exe`: `acde3c0c59e6d9a2106677656cb8f87a05f4ba47464237ad2cc81deab789f5a2`.
- SHA-256 `UnityMbed_0.1.27_amd64.deb`: `d3c1aedde88d0a4f0a0a987d139b4a45f26efd7dcd65539753c72fe5d6f7fd25`.

## v0.1.26 — Windows, macOS and Linux
- Windows: the app updates itself. When a newer version is out, it asks at launch, downloads
  and installs it. 0.1.25 and older cannot update themselves: install 0.1.26 once by hand.
- Closing the app also stops the local server and any build or debug tool it started.
- Linux (Ubuntu 22.04+ / Debian, x86_64): the first release since 0.1.9, built from the same
  source as Windows, including sign-in and plans on the new billing service. Same Arm GCC
  14.2.1 and `make` as Windows; flashing uses xPack OpenOCD 0.12.0-7. Updates are manual.
- macOS (Apple Silicon, macOS 13 or later): built from the same source.
- The third-party notices name the bundled fonts correctly. No crash reports.
- SHA-256 `UnityMbed_0.1.26_x64-setup.exe`: `96ab91baff0925c9bcff997e42a514f07d7ba251058428425e351af2863965ec`.
- SHA-256 `UnityMbed_0.1.26_amd64.deb`: `9ad14e8071dba1fd7f4af19e1f58e20c4bdf3c58e4f060fd8a3b89d6c72c4a9f`.

## v0.1.25 — Windows
- Replaces every earlier Windows build, including the 0.1.24 test build.
- Billing runs on the new UnityMbed billing service. Sign in with your email to get your plan;
  existing licences, devices and usage carry over.
- Each screen shows one renewal date for a paid plan.
- Building, flashing and debugging work for everyone. No crash reports.
- SHA-256 `09dd180e0792e83f6c4b97dbd2a509b8e8859e09f0b58fdfe798bafec833d902`.

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
