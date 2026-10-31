<p align="center"><img src="images/app-icon.png" width="72" alt="Judo Ceremony Desk icon"></p>

# Judo Ceremony Desk 0.20.3

**[Download for Windows](https://github.com/YOUNESMAAFI/judo-ceremony-releases/releases/download/v0.20.3/JudoCeremony-0.20.3-win-x64.zip)** · [Release notes](https://github.com/YOUNESMAAFI/judo-ceremony-releases/releases/tag/v0.20.3) · [Demonstration guide](docs/BOSS-DEMO.md)

**Compatibility:** newly saved event files use schema 9 and need **0.20 or newer**. Existing schema 1–8 events still open.

| Download | Contents |
| --- | --- |
| [Windows application ZIP](https://github.com/YOUNESMAAFI/judo-ceremony-releases/releases/download/v0.20.3/JudoCeremony-0.20.3-win-x64.zip) | Complete portable app, runtime, assets, examples and guide. Extract the entire folder. |
| [Flag PNGs](https://github.com/YOUNESMAAFI/judo-ceremony-releases/releases/download/v0.20.3/Flags-PNG.zip) | Individual horizontal and reference-backed vertical flags. |
| [Searchable flag audit](https://github.com/YOUNESMAAFI/judo-ceremony-releases/releases/download/v0.20.3/Judo-Ceremony-0.7-Audit-Searchable.pdf) | Unchanged artwork audit with searchable text and comparisons. |
| [Release notes](https://github.com/YOUNESMAAFI/judo-ceremony-releases/releases/download/v0.20.3/RELEASE-NOTES.md) | Changes, compatibility and validation. |
| [README](https://github.com/YOUNESMAAFI/judo-ceremony-releases/releases/download/v0.20.3/README.md) | Downloadable user guide. |
| [Check report](https://github.com/YOUNESMAAFI/judo-ceremony-releases/releases/download/v0.20.3/RELEASE-0.20.3-checks.txt) | Focused software checks and native-package verification. |
| [SHA-256 checksums](https://github.com/YOUNESMAAFI/judo-ceremony-releases/releases/download/v0.20.3/SHA256SUMS.txt) | Verify downloaded files. |

**Full-event updates, quick category fetches and four clear workspaces.**

An offline Windows application for judo award ceremonies, HDMI audience screens, staff images and social posts. Download the **v0.20.3 Preview** below. The complete Windows x64 package includes the runtime, flags, recordings and illustrated guide.

## Start here

Open `JudoCeremony.exe` from the complete extracted application folder. No separate .NET installation is needed. Close an older running copy first.

1. **Update event** in the top bar: connect an IJF competition link once, then refresh event details, countries, days, final-block matchups, medals and top-eight results together.
2. **Final block**: choose today or another competition day, select a category, review the medals and click **Prepare selected podium**.
3. **Preparation**: review the flags and countries, set appearance, then **Copy image** or **Save PNG** for staff.
4. **Ceremony display**: choose the HDMI monitor, **Load prepared →**, then **Play** when ready.
5. **Create social post**: use the same saved results, choose a layout and export a poster.

Manual entry remains available without an IJF link. Event updates never load or start the audience ceremony.

## Update once

**Last updated** appears beside Update event on every workspace. It records the last successful shared update and survives restart. A failed request keeps the previous timestamp and saved data. **Partial update** indicates unavailable pages; hover over the timestamp for details. Known medals are retained when a later page says results are pending.

Event information, participation, matchups and medal results now share the same update action. For a quick check, select a category in Final block and use **Fetch category** beside its heading. This reads the results page once and applies only the selected category, including its social-post athletes. It skips event details, participant, schedule and draw downloads. The category has its own checked time; the top bar retains the last full-event update time. Use **Event → New event** to connect a different competition.

![The four-workspace desk with one event update and daily category results](images/unified-event-desk.png)

*Illustrative rehearsal data.*

## Four main workspaces

| Workspace | What to do |
| --- | --- |
| Preparation | Enter/review medal countries, set backgrounds/logos and export a 2400 × 1350 staff image. |
| Ceremony display | Select the audience monitor; load, play, pause, restart or black out the ceremony. |
| Final block | Separate daily categories, review final-block matches and published medals, and arrange a ceremony queue. |
| Create social post | Create and remember posts using the shared event results. |

Green categories have four usable medal entries, including a valid no-gold/two-silver case. Partial and empty categories are grey. Fifth/seventh places are optional for readiness. Shorter approved podiums can still be entered and used.

**Tools** opens Event history, Anthem testing and Event readiness. **Event** contains New event, Open tournament, Save tournament and Event backup. **Countries** contains regional filters and manual participation editing.

## Staff image and audience screen

Search countries by three-letter code or full name. New categories start empty; returning to an entered category restores its own countries. Event settings are remembered, while preparation starts with no selected podium on launch.

The staff image and audience screen have separate visibility settings. Titles, codes, country names, medal labels, results table, hashtag and logos can be configured independently. Athlete names are optional in preparation images and social posts; they are always omitted from the audience screen.

Connect the second monitor in Windows **Extend** mode. The audience can also run in a window for rehearsal. Preparing another category or updating the event keeps the currently loaded ceremony intact until you explicitly load a replacement.

| Shortcut | Action |
| --- | --- |
| Ctrl+Enter | Load the prepared podium |
| F5 | Play/resume flags |
| F6 | Pause |
| F7 / Ctrl+R | Restart the loaded ceremony |
| F8 | Reset |
| F9 / Ctrl+B | Black screen / restore |
| F1 | Shortcut help |

## Social posts

Choose **Podium cards**, **Compact results**, **Flag grid** or **Winner spotlight**. Formats are portrait 1080 × 1350, square 1080 × 1080 and story 1080 × 1920. There are no athlete photos.

The editor reads the event's saved top-eight results. **Update event** automatically refreshes the athlete rows, including all eight when published. No second import/apply step is needed. Review codes and names, choose the design, then Copy image or Save PNG. No-gold spotlight layouts show the medallists without inventing a gold winner.

Valid poster edits are remembered locally per event, division and category. The saved design is preserved, while Update event automatically replaces athlete rows with the latest published results, including both 5th and both 7th places when available.

**Save poster…** exports a `.judo-social.json` project for another PC. These poster projects are separate from event backups; the shared IJF result snapshot is included in event files/backups.

## Anthems and checks

Anthems work offline, with independent controls and optional linking to flags. **Anthem playback is beta:** verify the recording and venue routing with event officials. No responsibility is accepted for anthem accuracy or playback. Test recordings through **Tools → Anthem testing** and run **Tools → Event readiness** before the ceremony.

The flag audit remains based on the April 2026 IJF manual, with the audited Excel supplement where applicable: 205 IJF countries, 16 supplemental entries and 34 catalog entries requiring organizer review. This is reference coverage, not an eligibility list. See the searchable PDF in `docs/audit/Release-Audit.pdf` and [third-party notices](THIRD-PARTY-NOTICES.md).

## Save, move and reopen

Use **Event → Save tournament…** to export an event, or **Event → Event backup…** to include embedded branding and relevant imported recordings. Restore previews the content and creates a new event identity. Previous events remain under Tools → Event history.

0.20 writes **event schema 9**, including shared top-eight results and Last updated. Use **0.20 or newer** to reopen those files. Schema 1–8 events still open. Poster files remain format 2, compatible with 0.18 and newer. Local data stays under `%LOCALAPPDATA%\JudoCeremony`.

See the [0.20 changes and workflow](docs/RELEASE-0.20.md) and [short boss demonstration](docs/BOSS-DEMO.md). Rehearse the actual HDMI monitor, scaling and speakers before live use.


## Validation

The final build passed **17 category-fetch/header checks**, **31 event-workflow checks** and **270 queue/update checks**. These suites overlap; the counts are not a unique total. The earlier 0.20 base passed 692 regression checks.

The Windows package passed native launch, empty startup, event reopening, embedded icon, all **442 reference-image hashes** and **146 anthem hashes**. The unchanged recordings also match the existing successful Windows decoder audit. Physical HDMI and venue-speaker rehearsal remain manual.

See [the current release notes](docs/RELEASE-0.20.3.md) and [short demonstration guide](docs/BOSS-DEMO.md). The automatic top-eight correction and clearer results tabs are included.
