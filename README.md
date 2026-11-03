# Ultimate Windows Maintenance Toolkit

**Clear system insights. Careful maintenance.** Built by DC.

View PC resources, manage startup apps, review maintenance actions and keep local reports in one Windows desktop app.

**[Download 3.5.0 Setup EXE](https://github.com/DeepC-Toolkit/ultimate-windows-maintenance-toolkit/releases/download/v3.5.0/UltimateWindowsMaintenanceToolkit-3.5.0-Setup.exe)** · [Release notes & checksums](https://github.com/DeepC-Toolkit/ultimate-windows-maintenance-toolkit/releases/tag/v3.5.0) · [Report a problem](https://github.com/DeepC-Toolkit/ultimate-windows-maintenance-toolkit/issues/new/choose)

Public Beta · Windows 10 / Windows 11 · Intel/AMD x64 · Free personal, non-commercial use

![Toolkit dashboard, light theme, sample readings](docs/images/dashboard.png)
*3.5.0 interface preview using sample readings. The resource score describes available resources; it is not a security scan.*

## What's new in 3.5.0

- **Readable updates:** installed and available versions are separate; long notes scroll while Download/Install buttons stay visible.
- **Deep Refresh:** preview more account Temp files older than seven days, then confirm cleanup of that reviewed set.
- **Responsive navigation:** debounced search and shared background discovery; fixed sidebar without scrolling.
- **Useful account menu:** click your account card for preferences, reports, Windows account settings, updates and feedback.
- **Reminder choices:** 5 / 15 / 30 / 45 / 60 minutes, with 30 minutes as the default. Existing notification opt-outs are preserved.

## What you can do

| Area | Purpose |
| --- | --- |
| Dashboard | CPU, RAM, supported GPU readings and drive usage |
| Quick Refresh | User-requested system RAM cleanup, followed by old account Temp cleanup |
| Deep Refresh | Bounded preview and cleanup of old account Temp files; keeps open apps running |
| Startup & app controls | Startup registrations, supported app pause/resume and CPU/GPU preferences |
| Maintenance | Review cleanup, diagnostics, Windows repair and update actions |
| Digital Wellbeing | Optional local foreground app names and usage durations |
| Reports | Review results stored on your PC |

Quick Refresh can briefly pause apps as Windows reloads memory pages. Lower RAM use does not guarantee better performance. Deep Refresh is a storage cleanup, and does not close apps, clear Windows Prefetch or promise a speed increase. Service discovery is not malware detection.

## Install or upgrade

1. Download the **Setup.exe** from the release above. The repository's “Source code” ZIP is not the installer.
2. Finish current maintenance, then choose **Exit** from the Toolkit tray menu. If only the tracker remains, use **Pause Toolkit for update** from Start.
3. Open Setup, review Windows' permission request and choose the installation folder. Existing settings/history are kept when upgrading the same installation.
4. Launch Toolkit. **About → Toolkit updates** shows the installed version and checks for new releases.

The installer is currently unsigned; Windows/Edge may show an unknown-publisher or download-reputation warning. A checksum verifies file consistency, not code-signing identity. Additional PC and display-scale testing is ongoing. ARM64/Snapdragon is not verified; 32-bit Windows is not supported.

## Updates and feedback

With automatic checking enabled, Toolkit checks official GitHub releases on launch and every six hours while running, including public betas. You choose when to download and install. Editing this README does not update an installed app.

**About → Feedback / report a problem** creates a draft for review, then opens GitHub Issues. A GitHub account is needed to submit. Nothing is posted automatically. Issues and replies are public; remove private information before submitting. See [support](SUPPORT.md).

## Privacy and choices

Settings, reports and optional Digital Wellbeing history stay locally. Digital Wellbeing records app names and durations, not keystrokes, screenshots, window titles or website addresses. Fresh installs enable startup and Digital Wellbeing; both can be changed, and saved opt-outs survive upgrades. High-load reminders require two minutes of sustained very high CPU/RAM before the selected repeat interval applies.

Update checks contact GitHub; requested diagnostics and Windows Update may contact their services. No reports or usage history are uploaded by Toolkit update checks. Hosting services can see ordinary connection information, such as the public IP. [Privacy details](docs/PRIVACY.md).

## License and project contents

Original Toolkit materials use the [DC Proprietary Software License](LICENSE). This repository provides official releases, documentation and support. The original application's source is private.

Third-party components retain their own rights and licenses. See [notices](THIRD_PARTY_NOTICES.txt), [license texts](third_party_licenses/) and [pystray source/replacement information](THIRD_PARTY_REPLACEMENT.txt). This repository includes that library's required source material, not the proprietary Toolkit source.

[User guide](docs/USER_GUIDE.txt) · [Changelog](CHANGELOG.md) · [All releases](https://github.com/DeepC-Toolkit/ultimate-windows-maintenance-toolkit/releases)

© 2026 DC
