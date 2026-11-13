<div align="center">

# Ultimate Windows Maintenance Toolkit

**PC insights and maintenance, in one place.**

Monitor system resources, review maintenance actions, and manage your Windows experience from one desktop app.

**Version 2.5.2 · Preview · Built by DC**

## [↓ Download UWT 2.5.2 for Windows](https://github.com/DeepC-Toolkit/ultimate-windows-maintenance-toolkit/releases/tag/v2.5.2)

Windows 10 and Windows 11 · Intel/AMD x64 (64-bit) PCs  
Free for personal, non-commercial use

[Release notes](https://github.com/DeepC-Toolkit/ultimate-windows-maintenance-toolkit/releases/tag/v2.5.2) · [Get help](#help-and-feedback) · [User guide](https://github.com/DeepC-Toolkit/ultimate-windows-maintenance-toolkit/blob/main/docs/USER_GUIDE.txt)

</div>

---

UWT brings resource readings, optional Digital Wellbeing, maintenance tools, and app controls together. You choose which actions to run, when tracking starts, and whether to check for updates. Usage history and maintenance reports are stored on your PC.

> **Preview status:** The installer is unsigned, and wider installation and compatibility testing remains pending. Windows or your browser may display a publisher or download-reputation notice. Keep Windows security protections enabled and review any detection before proceeding. UWT is a maintenance utility, not an antivirus product.

**Explore:** [Install](#download-and-install) · [Screenshots](#take-a-look) · [Features](#what-you-can-do) · [What's new](#new-in-252) · [Updates](#updates-and-version-numbering) · [Troubleshooting](#troubleshooting) · [Privacy](#privacy-and-network-connections) · [License](#license-and-third-party-components)

## Download and install

1. Open the [official 2.5.2 release page](https://github.com/DeepC-Toolkit/ultimate-windows-maintenance-toolkit/releases/tag/v2.5.2).
2. Expand **Assets** and download **`UltimateWindowsMaintenanceToolkit-2.5.2-Setup.exe`**. The accompanying **`.exe.sha256`** file is available for checking that your download matches the release checksum.
3. Finish any running maintenance. Choose **Exit** from the Toolkit system tray menu before installing. Close its background tracker as well; use the **Pause Toolkit for update** shortcut if it is available in your installation.
4. Open the installer, review its prompts, and complete setup. For an existing installation, use its existing installation folder.
5. Open Toolkit and check **About** for version **2.5.2**. Review startup, Digital Wellbeing, notifications, and Gaming Mode preferences.

**Moving from 3.5.1:** Version 2.5.2 begins a new numbering sequence. Install it manually from the release page; the older 3.5.1 updater does not treat the lower number as a newer version. The migration is intended to retain existing settings and history. Keep a backup before changing versions, since wider upgrade testing remains pending.

<details>
<summary><strong>Which file should I download?</strong></summary>

| File | Purpose |
| --- | --- |
| `UltimateWindowsMaintenanceToolkit-2.5.2-Setup.exe` | Windows installer for UWT 2.5.2 |
| `UltimateWindowsMaintenanceToolkit-2.5.2-Setup.exe.sha256` | Text containing the installer checksum |
| GitHub's **Source code (zip)** / **Source code (tar.gz)** | Archives of this public documentation repository; they are not the Windows installer or the private Toolkit application source |

Use the version-specific release link above to select 2.5.2 Preview. GitHub's **Latest** link may point to a different release.

</details>

<details>
<summary><strong>Optional: check your download with SHA-256</strong></summary>

A checksum comparison helps confirm that the downloaded file matches the checksum supplied with the release.

1. Download the installer and its `.exe.sha256` asset from the same official release page.
2. Open the `.sha256` file in a text editor and locate its 64-character checksum.
3. In PowerShell, run the following command after replacing the example path with the location of your downloaded installer:

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath "C:\path\to\UltimateWindowsMaintenanceToolkit-2.5.2-Setup.exe"
```

4. Compare the entire **Hash** value with the checksum in the downloaded sidecar. Uppercase and lowercase letters are equivalent.

A match confirms file integrity relative to that checksum. It does not identify the publisher or certify that software is free from malware. If the values differ, do not install that copy; check the filenames and download again from the official release page.

<!-- REVIEW NOTE: A fixed release checksum is intentionally not printed here. Two local sidecars match the maintainer's supplied value, but the live release sidecar could not be retrieved for independent comparison during preparation. -->

</details>

<details>
<summary><strong>System requirements and installation notes</strong></summary>

- Intended for Windows 10 and Windows 11 on Intel/AMD x64 PCs.
- 32-bit Windows is not supported. ARM64/Snapdragon compatibility is not verified.
- Some readings depend on hardware and Windows support; an unavailable GPU reading should not be interpreted as a hardware fault.
- Selected maintenance and repair actions require administrator permission. Review the Windows permission prompt for the action you requested.
- Internet access is needed for update checks, downloads, external support pages, and Windows operations that contact online services.
- Keep backups of important files before cleanup, repair, or version migration.

</details>

## Take a look


The dashboard combines resource readings and shortcuts to maintenance tools. Its **System Health** percentage represents resource headroom; it is not a malware-scan result or a security certification.


## What you can do

| Feature | How it helps |
| --- | --- |
| **Dashboard** | View CPU, RAM, drive usage, supported GPU readings, and system uptime |
| **Digital Wellbeing** | Review optional daily active-app usage recorded locally, with tracking and startup controls |
| **Quick Refresh** | Request RAM cleanup and eligible temporary-file cleanup, with a quiet completion notification |
| **Deep Refresh** | Preview eligible old temporary files before confirming cleanup |
| **Gaming Mode** | Apply a reversible priority preference to selected, already-running applications |
| **Startup Manager** | Review and manage supported startup entries for your Windows account |
| **App controls** | Use supported pause/resume, process-priority, and GPU-preference controls |
| **Maintenance and repair** | Access selected Windows diagnostic, cleanup, repair, and update operations |
| **Restore points** | Request a restore point and see prerequisite or service problems clearly |
| **Notifications and reports** | Receive brief task results and open local reports when you need detail |
| **Feedback** | Preview a report before opening an email draft or GitHub support page |

Review the action shown before running it. A maintenance tool can change Windows or remove eligible files; its presence in the app does not mean every action is appropriate for every PC.

<details>
<summary><strong>Digital Wellbeing: daily usage, uptime, and startup</strong></summary>

**Daily active usage and system uptime measure different things.** Uptime is time since the last system restart. Digital Wellbeing records active foreground-app usage while tracking is enabled and running.

- Enable tracking when you want to begin recording. Time before tracking started cannot be reconstructed.
- Usage is divided into local calendar days at midnight. Idle, locked, and sleeping periods are excluded from active usage.
- Recorded app names and durations stay on your PC. Tracking does not record keystrokes, screenshots, window titles, or website addresses.
- Tracking and the main application's startup preference are separate controls. Fresh installations leave tracking and GUI startup off; existing saved choices are preserved.
- When enabled, the collector can start for future sign-ins. Windows startup restrictions can prevent this, so check your preferences if recording does not resume.
- Minimizing Toolkit to the tray can keep it running. Choosing **Exit** stops the collector; a later launch or configured sign-in startup can start it again.
- Clearing Digital Wellbeing history requires confirmation. Maintenance reports are separate from usage history.

For an accurate interpretation, compare usage only across periods when the tracker was enabled and running.

</details>

<details>
<summary><strong>Quick Refresh: a short result without extra report windows</strong></summary>

Quick Refresh is available from the dashboard and tray. It requests the selected RAM-cleanup operation and then cleans eligible old temporary files. Completion is reported through a brief notification instead of automatically opening a detailed report window.

- RAM cleanup can require a Windows administrator prompt. Declining that prompt cancels this Quick Refresh operation, including its subsequent temporary-file cleanup.
- Temporary-file cleanup is limited to eligible old files in the current user's temporary folder, with an age threshold of more than seven days.
- Recent, locked, read-only, and reparse-point entries are skipped. It does not target Documents, Downloads, browser profiles, other users' folders, or Windows TEMP through this limited refresh action.
- A zero-byte result can be valid: there may be no eligible removable files.
- The reported removed-file size is not a guarantee of an identical change in free disk space, which can change as other apps run.
- A short cooldown prevents repeated Quick Refresh requests; allow 60 seconds before trying again.

RAM can refill as Windows and applications use it. Apps may briefly pause while memory pages are reloaded. Lower RAM usage alone does not demonstrate better performance.

</details>

<details>
<summary><strong>Deep Refresh: preview before cleanup</strong></summary>

Deep Refresh previews a limited set of eligible temporary files older than seven days for the current Windows account. Review the preview and confirm only when you want those files removed.

It does not force applications to close or clear Windows Prefetch. Protected, busy, recent, or otherwise excluded entries can remain. A partial result describes what was completed and what was skipped, rather than presenting every skipped file as a failure.

Cleanup work is bounded, and cancellation or access restrictions can leave some eligible files untouched. Use the local result details when you need to understand a partial operation.

</details>

<details>
<summary><strong>Gaming Mode: selected applications and reversible priorities</strong></summary>

Gaming Mode is optional and available through the app's account controls and system tray. Add the executable path of an application you trust, then launch that application yourself.

When an eligible matching process is already running at **Normal** priority, Gaming Mode can change it to **Above Normal**. Switching the mode off normally restores the priorities it changed.

- Adding a path does not automatically launch the executable.
- Gaming Mode starts off each time Toolkit launches.
- Selected paths and recovery information stay local.
- It does not overclock the GPU, force RAM trimming, disable security protections, or terminate other applications.
- It cannot guarantee higher FPS, lower latency, or a particular resource reduction. Results depend on the application and system load.

**After an unexpected interruption:** If Toolkit was forcibly terminated while Gaming Mode was active, turning Gaming Mode on again can process pending priority recovery information. Closing the affected game normally also ends that process. Do not delete recovery state as a substitute for restoring priorities.

</details>

<details>
<summary><strong>Startup Manager and app controls</strong></summary>

Startup Manager supports selected current-user startup mechanisms, including supported Run entries, shortcuts, and MSIX entries. Windows-managed or policy-controlled entries may not be editable through Toolkit.

App controls provide supported pause/resume, priority, and GPU-preference options. Pausing an application can interrupt its audio, downloads, or other work and does not necessarily release its RAM. Review the selected application and the action before proceeding.

Windows permissions and application restrictions can limit these controls. Toolkit should report that limitation instead of implying that a change succeeded.

</details>

<details>
<summary><strong>Maintenance, Windows repair, and restore points</strong></summary>

Toolkit provides access to selected Windows maintenance, diagnostics, and repair operations. Choose operations individually and review their scope. Administrator permission is requested for actions that need it; the main interface does not require every task to run elevated.

Restore-point creation depends on Windows System Protection and its required services. If a prerequisite is unavailable or a service is disabled, the result explains the problem instead of silently enabling services or claiming success. A restore point is not a replacement for an independent backup of personal files.

Busy or protected files may be skipped during cleanup. Windows repair operations can take time, and network-reset operations can interrupt connectivity. Keep the result details when reporting an unexpected failure.

</details>

<details>
<summary><strong>Notifications and local reports</strong></summary>

Quick Refresh and supported tray actions use non-blocking notifications. Task results can also be reviewed through the app's bounded session notification history. Detailed activity reports remain available to open when needed.

A notification is a summary, not proof that every requested item changed. Review details for a partial, unavailable, or failed operation. Windows notification settings can affect whether a notification appears.

</details>

## New in 2.5.2

- **Clearer daily usage:** Digital Wellbeing separates active usage from uptime and accounts for local-day boundaries.
- **User-controlled startup and tracking:** Review and choose background tracking and application startup preferences.
- **Quieter task completion:** Quick Refresh and tray actions use brief notifications, with reports available separately.
- **More useful results:** Cleanup distinguishes skipped entries, and restore-point results explain missing prerequisites.
- **Simpler feedback:** Preview the message before opening an email draft or external support page.
- **Optional Gaming Mode:** Select trusted application paths and apply reversible priority preferences to matching running processes.
- **New version sequence:** This release follows 3.5.1 under the 2.5.x numbering scheme; future versions are planned to continue with 2.5.3.

[Read the 2.5.2 release notes](https://github.com/DeepC-Toolkit/ultimate-windows-maintenance-toolkit/releases/tag/v2.5.2) · [Earlier changelog](https://github.com/DeepC-Toolkit/ultimate-windows-maintenance-toolkit/blob/main/CHANGELOG.md)

## Updates and version numbering

Open **About → Toolkit updates → Check again** to request an update check. Update checks require internet access. Automatic checking is off for fresh installations; when enabled, checks occur at launch and periodically while the app runs. You choose when to download and install.

**3.5.1 → 2.5.2 requires a manual installation.** The number changed intentionally, so an older version comparison can consider 2.5.2 lower than 3.5.1. Changing a README or GitHub release label does not change the updater inside an already-installed application.

The 2.5.x updater excludes legacy 3.x releases from its candidates. Preview handling and GitHub's **Latest** badge are separate concepts: use the explicit [2.5.2 release page](https://github.com/DeepC-Toolkit/ultimate-windows-maintenance-toolkit/releases/tag/v2.5.2) for this preview.

A failed network check means update status is unknown; it does not establish that the installed version is current. A download or notification alone does not complete installation.

## Troubleshooting

| What you see | What to do |
| --- | --- |
| GitHub's sidebar shows an older **Latest** release | Open the version-specific 2.5.2 link. This release is a Preview/pre-release. |
| Installed 3.5.1 does not offer 2.5.2 | Download 2.5.2 manually, exit Toolkit and its tracker, and run setup. |
| About still shows an older version | Finish setup and reopen the installed app. Check that the shortcut points to the intended installation. |
| Daily usage is less than system uptime | Check that tracking was enabled and running; idle, locked, sleeping, and unrecorded periods do not count as active usage. |
| Quick Refresh reports 0 bytes removed | There may be no eligible old files. Locked or excluded files can remain without needing forced deletion. |
| A cleanup action reports skipped entries | Review details. Do not force access to protected or in-use files solely to obtain a zero-skipped result. |
| Restore-point creation is unavailable | Review the reported Windows System Protection or service prerequisite and open System Protection if offered. |
| Gaming Mode cannot affect a process | Check the selected executable path and whether the process is running and eligible; permissions can limit changes. |
| No completion notification appears | Check Toolkit's notification history, local reports, and Windows notification settings. |
| An email draft does not open | Use the support address below in your preferred email service and paste only the details you want to share. |
| Update checking fails | Check connectivity and try again later, or use the official release page. |

**Removing Toolkit:** Exit it from the tray, then use Windows **Settings → Apps** to uninstall. Local settings, reports, or history may remain; review any retained data before deleting it if you want to preserve a backup.

## Help and feedback

Choose the channel that suits your report:

| Channel | Account and visibility |
| --- | --- |
| **[Email support](mailto:uwtsupport.official@gmail.com)** | No GitHub account required. The message goes to the support mailbox rather than a public issue. Your email provider handles sending. |
| **[GitHub Issues](https://github.com/DeepC-Toolkit/ultimate-windows-maintenance-toolkit/issues)** | Requires a GitHub account. Reports and replies are public. |

In Toolkit, open **About → Feedback / report a problem**. Review the message before opening an email draft or GitHub page. Opening a draft does not send it: complete and submit it yourself in the selected service. This is not an anonymous in-app messaging server.

For a useful report, include:

- Toolkit version and Windows version.
- The action you selected and the steps needed to reproduce the issue.
- What you expected and what actually happened.
- A relevant error message or a sanitized screenshot, if helpful.

Remove passwords, tokens, recovery codes, personal paths, account names, and unrelated activity before sharing. For a possible security issue or sensitive report, use email rather than posting private details in a public issue.

[Additional support information](https://github.com/DeepC-Toolkit/ultimate-windows-maintenance-toolkit/blob/main/SUPPORT.md)

## Privacy and network connections

Settings, maintenance reports, selected Gaming Mode paths, and optional Digital Wellbeing history are stored locally. Digital Wellbeing records app names and usage durations; it does not record keystrokes, screenshots, window titles, or website addresses.

| Activity | What happens |
| --- | --- |
| Resource dashboard and optional usage tracking | Readings and usage records are processed locally |
| Maintenance reports | Saved on your PC; review them before sharing |
| Toolkit update checks and downloads | Contact GitHub or its download infrastructure; usage history and maintenance reports are not uploaded as part of these checks |
| Email feedback | Your chosen email service sends the message after you submit it |
| GitHub Issues and external help links | Open external services with their own account and privacy practices |
| Windows Update and requested network diagnostics | May contact the relevant Windows or network services |

External services can receive ordinary connection metadata, such as your public IP address. “Local usage history” does not mean every feature works without a network connection.

<details>
<summary><strong>Your local data and sharing choices</strong></summary>

Toolkit data is stored under `%LOCALAPPDATA%\UltimateWindowsMaintenance`. Tracking and startup are controlled through your preferences. Review existing choices after an upgrade.

Reports may contain paths or network information relevant to the task you ran. Do not publish the entire data folder or a personal backup to report a problem. Share only the specific information needed after reviewing it.

Feedback is user initiated. Toolkit does not automatically send your usage history, private reports, or credentials to the developer.

[Privacy documentation](https://github.com/DeepC-Toolkit/ultimate-windows-maintenance-toolkit/blob/main/docs/PRIVACY.md)

</details>

## License and third-party components

UWT is free for **personal, non-commercial use** under the included [DC Proprietary Software License](https://github.com/DeepC-Toolkit/ultimate-windows-maintenance-toolkit/blob/main/LICENSE). Read that license for permissions, restrictions, and exceptions. Share the official release link so others can obtain the official package.

This public repository provides downloads, documentation, and support. The original Toolkit application's source code is private. Public availability of the installer does not make the application copyright-free or grant an open-source license to its original code.

Third-party components retain their own licenses and rights. The Toolkit license does not replace those terms.

- [Third-party notices](https://github.com/DeepC-Toolkit/ultimate-windows-maintenance-toolkit/blob/main/THIRD_PARTY_NOTICES.txt)
- [Third-party licenses](https://github.com/DeepC-Toolkit/ultimate-windows-maintenance-toolkit/tree/main/third_party_licenses)
- [Library source and replacement information](https://github.com/DeepC-Toolkit/ultimate-windows-maintenance-toolkit/blob/main/THIRD_PARTY_REPLACEMENT.txt)
- [Provided third-party sources](https://github.com/DeepC-Toolkit/ultimate-windows-maintenance-toolkit/tree/main/third_party_sources)

---

[Download 2.5.2 Preview](https://github.com/DeepC-Toolkit/ultimate-windows-maintenance-toolkit/releases/tag/v2.5.2) · [All releases](https://github.com/DeepC-Toolkit/ultimate-windows-maintenance-toolkit/releases) · [Email support](mailto:uwtsupport.official@gmail.com)

© 2026 DC
