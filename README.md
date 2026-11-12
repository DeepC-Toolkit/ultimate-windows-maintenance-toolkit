<div align="center">

# Ultimate Windows Maintenance Toolkit

**PC insights and maintenance, in one place.**

Monitor system resources, review maintenance options, and manage optional local features from one Windows desktop app.

**Version 2.5.2 · Preview · Built by DC**

[⬇️ Download UWT 2.5.2 for Windows](https://github.com/DeepC-Toolkit/ultimate-windows-maintenance-toolkit/releases/tag/v2.5.2)

Windows 10 and Windows 11 · Intel/AMD 64-bit PCs  
Free for personal, non-commercial use

[Release notes](https://github.com/DeepC-Toolkit/ultimate-windows-maintenance-toolkit/releases/tag/v2.5.2) · [Get help](https://github.com/DeepC-Toolkit/ultimate-windows-maintenance-toolkit/issues) · [User guide](docs/USER_GUIDE.txt)

</div>

---

## Download and install

1. Open the [UWT 2.5.2 release page](https://github.com/DeepC-Toolkit/ultimate-windows-maintenance-toolkit/releases/tag/v2.5.2).
2. Under **Assets**, download `UltimateWindowsMaintenanceToolkit-2.5.2-Setup.exe`. The `.sha256` file beside it is for checking the download; the automatically listed **Source code** archives are not Windows installers.
3. In PowerShell, calculate the downloaded installer’s SHA-256:

   ```powershell
   Get-FileHash -Algorithm SHA256 -LiteralPath "$env:USERPROFILE\Downloads\UltimateWindowsMaintenanceToolkit-2.5.2-Setup.exe"
   ```

4. Compare the displayed hash with the `.sha256` asset on the release page. If they do not match, do not open the installer.
5. Close Toolkit from its system-tray menu before installing. Open Setup, review the Windows permission prompt, and follow the installer.
6. Launch Toolkit and review **Settings** for startup, Digital Wellbeing, notifications, and Gaming Mode preferences.

### Updating from 3.5.1

Version 2.5.2 begins a new version-numbering sequence. The 3.5.1 updater may not offer this lower-numbered version, so existing users need to install 2.5.2 manually from the release page. If you want to upgrade an existing installation, close Toolkit and its tracker first, then use the same installation location. Future releases are planned for the 2.5.3 sequence.

### Preview status

This installer is unsigned, so Windows or a browser may show an unknown-publisher or download warning. The checksum can confirm that a file matches the published hash; it does **not** prove who published it or certify that it is safe. Broader clean-PC, upgrade, uninstall, and compatibility testing is still pending. 32-bit Windows is not supported; ARM64 compatibility has not been verified.

---

## Take a look

> These are historical **3.5.0** interface previews. The 2.5.2 interface may differ. The screenshots use sample readings; the resource score is not a security scan.

![Ultimate Windows Maintenance Toolkit 3.5.0 dashboard preview in the light theme](docs/images/dashboard.png)

*Historical 3.5.0 light-theme preview with sample readings.*

What you can do
Feature	How it helps
Dashboard	View live CPU and RAM readings, supported GPU readings, drive usage, and other system information.
Digital Wellbeing	Optionally review app names and usage durations saved locally on your PC.
Quick Refresh	Request a brief memory refresh, followed by a bounded cleanup of eligible old temporary files for your Windows account.
Deep Refresh	Preview eligible old temporary files and review the results before confirming cleanup.
Startup Manager	Review and manage supported startup entries. Startup preferences are user-controlled.
App controls	Review supported app controls and CPU/GPU preferences.
Maintenance tools	Review Windows diagnostic, repair, update, and cleanup actions before running them. Some actions require administrator permission.
Gaming Mode	Optionally adjust the priority of selected, already-running applications and restore their previous priorities when switched off normally.
Local reports	Review maintenance results saved on your PC.


Review each maintenance action before running it. Keep independent backups of important files. A lower RAM reading does not necessarily mean better performance, and no maintenance feature guarantees a speed increase.
Understand Quick Refresh and Deep RefreshQuick Refresh
Quick Refresh requests a short-lived Windows helper to refresh memory, then checks a bounded set of eligible temporary files for your Windows account. Windows may show a permission prompt for the helper.
- It does not close your applications. Windows may briefly pause or reload memory pages.
- Cleanup is limited to eligible old files in your account’s temporary folder. Recent, locked, or otherwise skipped files are left in place.
- It does not clean Downloads, Documents, browser profiles, Windows system files, or other users’ folders.
- Results report what the cleanup actually handled. A skipped item is not treated as deleted.
- The amount of temporary data removed is not a promise of the same amount of extra physical disk space or a guaranteed performance improvement.
The result is shown as a compact, non-blocking notification. Optional details and recent task notifications are available in the Toolkit.
Deep Refresh
Deep Refresh previews a bounded set of eligible temporary files older than seven days for your Windows account. Review the list before confirming cleanup. It does not close apps or clear Windows Prefetch.

Digital Wellbeing
Digital Wellbeing is optional and stays on your PC. Enable tracking when you want it to start recording. Daily totals are split at midnight; the feature does not recreate usage from before tracking was enabled. Locked, sleeping, and idle periods are excluded from active usage.

The history records application names and usage durations. It does not record keystrokes, screenshots, window titles, or website addresses. Review or clear your local history in the Toolkit.
Gaming Mode
Gaming Mode is optional and user-controlled. Select a trusted application that is already running, then turn the mode on when you are ready.
- It can raise a matching process from Normal to Above normal priority.
- You launch the game or application yourself. Toolkit does not automatically launch an arbitrary EXE.
- It does not overclock the GPU, alter security settings, kill other processes, or promise higher FPS.
- Toolkit records the prior priority locally so it can normally restore it when Gaming Mode is turned off.
- Gaming Mode starts off when Toolkit is launched. If Toolkit or Windows closes unexpectedly during a session, follow the recovery guidance in the user guide before removing local recovery data.
Priority changes may not improve a particular game or PC. Check that the selected application is the one you intend to adjust.
New in 2.5.2
- Clearer daily accounting for optional, local Digital Wellbeing tracking.
- Quieter, non-blocking Quick Refresh and task-completion notifications.
- More informative cleanup and restore-point results, including skipped items and reported failures.
- Feedback preview before opening an email draft or a GitHub issue.
- Optional Gaming Mode for selected, already-running applications.
- A new 2.5.x version sequence; upgrades from 3.5.1 require manual installation.



Help and feedback
For a problem or feature suggestion, include:
- Toolkit version and Windows version
- What you expected to happen
- What actually happened
- The steps needed to reproduce the problem, if known
Use GitHub Issues for public reports. Issues and replies can be visible to others, so remove passwords, recovery codes, personal files, email addresses, and other private information from screenshots and descriptions before posting.

You can also contact support at uwtsupport.official@gmail.com. The Toolkit prepares a draft for you to review; it does not send feedback automatically. You decide whether to open the draft and send it.
