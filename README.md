<p align="center">
  <img src="images/app-icon.png" width="80" alt="Judo Ceremony Desk app icon">
</p>

<h1 align="center">Judo Ceremony Desk</h1>

<p align="center">
  <strong>Prepare the podium. Share the flag positions. Run the ceremony.</strong><br>
  An offline Windows application for judo award ceremonies and HDMI audience screens.
</p>

<p align="center">
  <img alt="Version 0.9.0 Preview" src="https://img.shields.io/badge/version-0.9.0_Preview-C9A65A">
  <img alt="Windows x64" src="https://img.shields.io/badge/platform-Windows_x64-132047">
  <img alt="Offline" src="https://img.shields.io/badge/operation-offline-147D73">
  <img alt="216 software checks passed" src="https://img.shields.io/badge/software_checks-216_passed-147D73">
</p>

<p align="center">
  <a href="https://github.com/YOUNESMAAFI/judo-ceremony-releases/releases/download/v0.9.0/JudoCeremony-0.9-win-x64.zip"><strong>Download for Windows</strong></a>
  &nbsp; | &nbsp;
  <a href="https://github.com/YOUNESMAAFI/judo-ceremony-releases/releases/tag/v0.9.0">Release notes &amp; downloads</a>
  &nbsp; | &nbsp;
  <a href="https://github.com/YOUNESMAAFI/judo-ceremony-releases/releases/download/v0.9.0/Judo-Ceremony-0.7-Audit-Searchable.pdf">Searchable flag audit</a>
</p>

---

## At a glance

Judo Ceremony Desk gives the operator a preparation workspace and a separate ceremony workspace. Prepare a category, copy a clear flag-position image for staff, then raise the flags on the audience screen when the ceremony begins.

| Capability | What you can do |
| --- | --- |
| Staff images | Copy a complete image or save a **2400 × 1350 PNG**. |
| Audience display | Run the flag animation in a separate window on an HDMI screen. |
| Independent controls | Choose which titles, labels, country names and tables appear in each output. |
| Country selection | Search **255 catalog entries** using three-letter codes or country names. |
| Category memory | Enter each category separately and restore its countries when you return. |
| Event history | Save previous events locally and reopen their categories. |
| Exceptional medals | Present two silvers with no gold, missing medals and other approved layouts. |
| Event branding | Add backgrounds, three logos and a hashtag footer. |
| Offline use | Use bundled flag artwork and the included Windows runtime without an internet connection. |

**Version 0.9.0 is a preview for review and rehearsal.** Software checks and package checks pass; rehearse the actual event computer, HDMI screen and staff-image workflow before live use. Anthem audio playback is not included.

## Contents

[Download](#download) · [Quick start](#quick-start) · [Workspaces](#workspaces) · [Separate visibility controls](#separate-visibility-controls) · [Countries and categories](#countries-and-categories) · [Medal layouts](#medal-layouts) · [HDMI display](#hdmi-display) · [Shortcuts](#shortcuts) · [Branding](#branding) · [Event history and files](#event-history-and-files) · [Flag audit](#flag-audit) · [Troubleshooting](#troubleshooting) · [Support and notices](#support-and-notices)

## Download

Download the files from the [v0.9.0 release page](https://github.com/YOUNESMAAFI/judo-ceremony-releases/releases/tag/v0.9.0).

| File | Use |
| --- | --- |
| [JudoCeremony-0.9-win-x64.zip](https://github.com/YOUNESMAAFI/judo-ceremony-releases/releases/download/v0.9.0/JudoCeremony-0.9-win-x64.zip) | Complete portable Windows application, runtime, assets, examples and documentation. |
| [Flags-PNG.zip](https://github.com/YOUNESMAAFI/judo-ceremony-releases/releases/download/v0.9.0/Flags-PNG.zip) | Individual horizontal and reference-backed vertical flag PNGs. |
| [Searchable audit PDF](https://github.com/YOUNESMAAFI/judo-ceremony-releases/releases/download/v0.9.0/Judo-Ceremony-0.7-Audit-Searchable.pdf) | The flag reference review, differences table and full visual comparisons. |
| [Release notes](https://github.com/YOUNESMAAFI/judo-ceremony-releases/releases/download/v0.9.0/RELEASE-NOTES.md) | Changes, compatibility and validation for this release. |
| [README.md](https://github.com/YOUNESMAAFI/judo-ceremony-releases/releases/download/v0.9.0/README.md) | A downloadable copy of this guide. |
| [Software check result](https://github.com/YOUNESMAAFI/judo-ceremony-releases/releases/download/v0.9.0/RELEASE-0.9-checks.txt) | Confirmation of the 216 passing software checks. |
| [SHA256SUMS.txt](https://github.com/YOUNESMAAFI/judo-ceremony-releases/releases/download/v0.9.0/SHA256SUMS.txt) | SHA-256 hashes for the release downloads. |

**Platform:** Windows x64. Windows 11 x64 is the development and test platform. The application ZIP includes the .NET runtime; a separate .NET installation is not required for normal use.

To check a downloaded file in PowerShell, run the command below and compare its hash with the matching entry in `SHA256SUMS.txt`:

```powershell
Get-FileHash -Algorithm SHA256 .\JudoCeremony-0.9-win-x64.zip
```

## Quick start

1. **Extract the complete application ZIP** to a local folder. Keep `Assets`, `Notices`, `examples`, `docs` and the other package files together.
2. Close an older running copy, then open **JudoCeremony.exe** in the extracted folder.
3. On **1 Preparation**, enter the event name once and select a category, such as **Men -73 kg**.
4. Choose the medal layout and select a country for each awarded medal. Search by a three-letter code, then select a result or press Enter.
5. Choose horizontal or vertical flags. Use **Image visibility...** to select the contents of the staff image, then **Copy image** or **Save PNG**.
6. For the audience, connect the second screen in Windows **Extend** mode. Open **2 Ceremony display**, choose the monitor and click **Load prepared →**.
7. Check the **Audience screen visibility** options and raising duration, then press **Play** when ready.

Sample tournament files are included in `examples`, including standard medals, a two-silver ceremony and a blue background with a hashtag. After opening a sample, choose its saved category to restore its countries.

## Workspaces

### 1 · Preparation

The first page keeps category buttons beside event details, medal countries, appearance settings and the staff-image preview.

![Preparation workspace with category buttons, medal countries and staff-image preview](images/operator-desk.png)

The application starts with **no selected category or medal countries**. It remembers the current event settings. Select a category to begin or to restore that category's saved results.

Prepare the next podium while the current ceremony is loaded. Country, category, title and appearance edits reach the audience when you explicitly load the preparation.

### 2 · Ceremony display

This page contains monitor selection, loading, playback, elapsed time, raising duration, audience visibility options and a preview of the loaded ceremony.

The audience window is separate from the operator desk. It can run on the HDMI screen or as a windowed rehearsal on the same computer.

### 3 · Event history

Previous events and their saved category countries appear here. Select an event to inspect its categories, then choose **Open selected event**.

![Event history with a previous event and its saved medal countries](images/event-history.png)

Opening an event leaves the preparation empty until you select a category. The loaded audience ceremony continues to use its existing snapshot.

## Separate visibility controls

Staff instructions and the audience screen can show different information. Event text and artwork are shared; visibility is selected separately for each output.

| Output | Where to change it | What updates |
| --- | --- | --- |
| Staff image | **Preparation → Image visibility...** | The staff preview, **Copy image** and **Save PNG**. |
| Audience screen | **Ceremony display → Audience screen visibility** | The audience preview and HDMI output. |

Both sets independently control:

| Element | Staff image | Audience screen |
| --- | :---: | :---: |
| Tournament title | ✓ | ✓ |
| Contest category | ✓ | ✓ |
| Flags and attached labels | ✓ | ✓ |
| Medal labels | ✓ | ✓ |
| Three-letter country codes | ✓ | ✓ |
| Full country names | ✓ | ✓ |
| Results table | ✓ | ✓ |
| Event hashtag | ✓ | ✓ |
| Logos | ✓ | ✓ |

![Independent staff-image visibility controls](images/image-visibility.png)

Changes apply immediately to the corresponding output and save with the event. Audience visibility edits preserve countries, elapsed time, pause and blackout. Image visibility edits leave the audience unchanged.

Hiding flags also hides their attached labels and disables those label controls for that output. The results table is a separate option and uses three-letter codes independently of the labels under flags.

<details>
<summary><strong>Example: detailed staff image and simpler audience screen</strong></summary>

The same illustrative podium can include medal labels, codes, full country names and a results recap for staff, while the audience sees the flags and event titles.

**Staff image**

![Example staff image with medals, country names and a results recap](images/staff-image.png)

**Audience screen**

![Example audience screen with the corresponding flags and event titles](images/audience-screen.png)

</details>

## Countries and categories

### Countries

Search by a three-letter code or country name. Examples include **TJK**, **RUS**, **FRA**, **GER**, **SUI** and **EGY**. The catalog uses sports codes where supplied, with ISO alpha-3 fallbacks for other entries.

Duplicate countries are supported: the same country can appear in more than one medal position. Athlete names are not collected.

**Tab** moves to the next enabled country field and cycles back after the last field. **Shift+Tab** moves backwards. Medal selectors and country fields marked **Not awarded** are skipped.

### Categories

Choose a division, then click the visible men's or women's weight-category buttons. Presets include senior, junior, cadet and veterans divisions, plus editable open, team and other labels. **Custom...** and **Edit presets** support local event categories.

A new category starts with empty country fields and the standard medal layout. Returning to an entered category restores its own countries and medals. Different divisions and weights keep separate results, including partially entered or cleared countries.

Senior is available as a division filter but is omitted from the displayed contest title. Other division labels, such as Junior and Cadet, remain in their titles.

## Medal layouts

| Layout | Presentation |
| --- | --- |
| Standard | Gold, silver and two bronze medals. |
| No gold · two silver | Two silvers, an empty gold position and two bronzes. |
| One bronze | Gold, silver and one bronze medal. |
| Gold and silver only | Two awarded medals. |
| Gold only | One centered awarded medal. |
| Custom | Choose Gold, Silver, Bronze or Not awarded for each entry. |

The standard audience order is **silver · gold · bronze 1 · bronze 2**. Gold finishes highest; silver is lower; both bronzes finish at the same height.

For an approved two-silver, no-gold result, the display reserves an empty gold position between the silvers and bronzes. No flag or label is drawn in the missing position. Both silvers finish at the same height.

Use the result approved by event officials, including the applicable double hansoku-make outcome. The application presents the selected medals; it does not determine disqualification consequences or calculate competition results.

## HDMI display

1. Connect the audience display and press **Win+P → Extend** in Windows.
2. On Ceremony display, click **Refresh** and select the intended monitor. Use **Windowed preview (this PC)** for rehearsal without a second screen.
3. Set a raising duration between **3 and 300 seconds**. Type the value or use the up/down arrows. Load the preparation to use its new duration.
4. Click **Load prepared →** to open the audience window and capture the prepared podium.
5. Use the controls below during the ceremony.

| Control | Behavior |
| --- | --- |
| Play / Resume | Start or continue the loaded animation. |
| Pause | Freeze the flag movement. |
| Restart | Immediately replay the loaded ceremony from its beginning. |
| Reset | Return flags to the starting positions; confirms when active. |
| Black screen | Make the complete audience output black and pause movement. |
| Restore screen | Restore the picture while leaving movement paused. |
| Close display | Close the audience window; confirms when active. |

Reset an active or paused ceremony before loading a replacement. Restart uses the loaded podium and its duration; it does not load pending preparation edits.

If the audience monitor disconnects, the application pauses and closes that output window. Reconnect the monitor, refresh the list, select it and reopen the display before resuming.

## Shortcuts

| Key | Action |
| --- | --- |
| Space | Play, pause or resume. |
| F5 | Play / resume. |
| F6 | Pause. |
| F7 or Ctrl+R | Restart the loaded ceremony. |
| F8 | Reset to starting positions. |
| F9 or Ctrl+B | Black screen / restore. |
| Ctrl+Enter | Load the preparation. |
| F1 | Show shortcut help. |
| Esc in the audience window | Close the display; confirms when active. |
| Tab / Shift+Tab in country fields | Move forward / backwards between enabled country fields. |

Ceremony shortcuts work with the operator or audience window in focus. They are not system-wide hotkeys. Held keys do not repeat ceremony actions. Space retains its normal behavior in text fields, checkboxes, lists and history selection.

## Branding

Open **Appearance...** beside the staff preview to configure the event artwork.

- Choose **Guide blue**, **Blue gradient**, **Dark blue** or **White & blue**.
- Set a custom background color, or import a PNG, JPEG or BMP background.
- Adjust background darkening for readable titles.
- Add logos at the top-left, top-right and bottom-center. Logos keep their proportions and PNG transparency.
- Enter an optional event hashtag below the tournament name. A leading `#` is added when needed; multiple space-separated hashtags are supported.

Background presets are based on an IJF-published event-guide palette. They are display presets rather than event-approved artwork.

**Include appearance in staff images** selects whether staff exports use the same artwork or the white staff layout. The independent visibility checkboxes determine which elements are shown on each output. Background and logo artwork are configured through Appearance; their visibility can differ between outputs.

Imported images are embedded in the event file, so moving the original picture files does not break a saved setup. Tournament files, including embedded artwork and category results, are limited to **25 MB**.

## Event history and files

### Remember the current event

The app remembers the event name, appearance, hashtag, category presets and visibility preferences. On launch, category and country fields start empty. Select a saved category to restore its countries.

### Start another event

Choose **New event** to save the current event to history and begin an empty event. Editing the current event name renames it; New event creates a separate event identity, even when the names match.

Entered countries in an unnamed event are retained in history under **Untitled event**.

### Export and reopen

**Save tournament...** creates a `.judo.json` file containing that event's settings, category results and embedded artwork. **Open tournament** saves the current event first, then opens the selected event. Select a category to restore its results.

Event history stays on this computer. Export a tournament file to move one event to another computer or keep a backup.

| Local data | Location |
| --- | --- |
| Current event | `%LOCALAPPDATA%\JudoCeremony\last-tournament.json` |
| Event history | `%LOCALAPPDATA%\JudoCeremony\events\` |

If the current autosave cannot be read, the original is preserved in an `.invalid-...` recovery copy and the app reports the problem. Close older versions before starting another build; the session lock prevents simultaneous copies from writing to the same saved session.

### File compatibility

Version 0.9 writes **schema 4** to preserve independent staff/audience preferences and per-category results. Earlier app versions reject these files instead of silently dropping settings.

Schema 1, 2 and 3 files still open. Their saved podium is preserved as a category, and older shared visibility choices are copied to both outputs before becoming independent.

## Flag audit

The artwork was checked against **FlagChecking v1.5e** and the **IJF Flag Manual dated 1 April 2026**. The newer IJF manual takes priority when the sources disagree.

| Coverage | Count |
| --- | ---: |
| Catalog entries | 255 |
| Horizontal and vertical views reviewed | 510 |
| Countries covered by the newer IJF manual | 205 |
| Additional countries covered by the workbook supplement | 16 |
| Countries with reference-backed artwork | 221 |
| Entries outside both references, requiring organizer review | 34 |

The interface identifies selections outside the references for organizer review. The catalog is not an event-eligibility list. Special delegation gaps, source defects and remaining differences are documented in the audit.

The **16-page searchable PDF** includes a differences table with separate flag images, selectable text and the complete comparison sheets. Use **Ctrl+F** to find country names, codes or comparison results.

The PDF describes the **0.7 flag audit**; the artwork is unchanged in 0.9. Its software-test count belongs to that earlier release. **Version 0.9 passed 216 software checks**, plus native launcher, fresh-start, migration, app-icon and all 442 reference-image hash checks.

Individual flag filenames use a three-letter code and full name, for example `TJK - Tajikistan.png`. The standalone archive contains **255 horizontal PNGs** and **221 vertical reference designs**. Source artwork resolution limits sharpness when enlarged; check the actual audience screen at event distance.

## Troubleshooting

| Problem | Check |
| --- | --- |
| The application does not start | Extract the entire Windows x64 ZIP, keep the package files together and close any older running copy. |
| Country fields are empty after opening | Select a category. Empty startup is intentional; saved category results are restored when selected. |
| A new category shows no countries | Enter that category's results. Countries are not carried over from another category. |
| The audience is showing the previous podium | Load the prepared category when ready. Preparation and loaded ceremony are separate. |
| A staff-image change is missing on the HDMI screen | Set the audience's own visibility options on Ceremony display. |
| An audience change is missing from Copy image | Use Image visibility on Preparation for staff-image contents. |
| The second monitor is missing | Check Windows Extend mode, the HDMI connection and the monitor's power; then refresh the display list. |
| The restored screen is not moving | Blackout pauses playback. Press Play / Resume after restoring the picture. |
| An older app rejects the event file | Open schema 4 files with version 0.9 or a compatible newer build. |
| There is no anthem sound | Audio playback is not included; this version uses a timed flag animation. |

Before live use, rehearse the approved podium, both flag orientations, the visibility choices, HDMI resolution/scaling and reconnection, and pasting the staff image into the chosen Windows application.

## Support and notices

For a problem report, [open an issue](https://github.com/YOUNESMAAFI/judo-ceremony-releases/issues). Include the app version, Windows version, steps to reproduce the problem, expected result and what happened. For display issues, include the monitor resolution and scaling.

Artwork and data sources are listed in [THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md). Microsoft .NET license and third-party notices are included in the application package. No IJF endorsement is implied.

---

<p align="center"><strong>Judo Ceremony Desk</strong><br>Offline preparation and ceremony display for judo event teams.</p>
