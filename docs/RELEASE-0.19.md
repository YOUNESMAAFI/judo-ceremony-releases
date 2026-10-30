# Judo Ceremony Desk 0.19 — social posts by category

Open **7 Create social post**, immediately after **6 Final block**. The preparation **Social export…** shortcut also opens this tab. Select the competition day and category, then **Create / edit social post…** to open the editor. Choose Podium cards, Compact results, Flag grid or Winner spotlight; portrait, square and story formats remain available. Athlete photos are not used.

The category tables in Final block and Create social post use the same colours:

| Colour | Status | Meaning |
| --- | --- | --- |
| Green | Ready | Four usable medal entries, including a valid no-gold, two-silver podium. Fifth and seventh places are optional. |
| Grey | Partial | Some published or entered results, but no complete four-medal podium. |
| Grey | No results | No medal results yet. |

A shorter podium can still be edited and exported; the colour is a readiness cue. Imported categories requiring review remain grey. Day buttons preserve separation of a competition's daily programme. Unscheduled categories are under **Schedule unavailable**.

Valid editor changes are remembered automatically, including results, layout, dimensions, footer and branding. The editor displays the saved time. Reopening a category restores its own poster, and restarting the app retains it under the current event. Different events and divisions have separate records. Applying another category from the IJF importer saves that category separately. Editing the displayed heading does not rename the selected category's record.

Incomplete or invalid edits retain the last valid saved poster. Remembered posters take priority over newer preparation or final-block data; deliberately read and apply IJF results in the editor when updating them. Opening a poster file replaces the selected category's draft. Social edits do not change ceremony preparation, the queue or the audience display.

Remembered posts are stored locally in `%LOCALAPPDATA%\JudoCeremony\social-posts`, separately from event files and portable event backups. Use **Save poster…** in the editor to transfer a project to another PC. A restored event backup is a new event copy and does not inherit the original event's locally remembered posts. Poster files remain format 2 (0.18 or newer); older format-1 projects still open. Tournament schema remains 8.

Run `dist/JudoCeremony-0.19/JudoCeremony.exe` or **Start Judo Ceremony.cmd**. Keep the whole app folder together. Download the [v0.19.0 preview](https://github.com/YOUNESMAAFI/judo-ceremony-releases/releases/tag/v0.19.0).

All **668 regression checks passed**. Validation covers actual WPF row colours, tab placement and editor access, automatic saving, immediate-close saving, switching categories and events, reopening the app, imported category identity, and preservation of ceremony data. Native launch and asset verification use isolated test data. Physical HDMI and venue audio rehearsal remain separate checks on event hardware.