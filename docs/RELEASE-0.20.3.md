# Judo Ceremony Desk 0.20.3 — quick category fetch and aligned header

Select a category in **Final block → Category results**, then click **Fetch category** beside its heading. This reads the IJF results page once and updates only that category's medals and top-eight athlete rows. It also updates that category's remembered or open social post while retaining its design.

The quick operation skips event details, participant lists, schedules and draw downloads. Other categories, other saved posters, manual preparation and the loaded audience ceremony are retained. The selected category shows its own **Category checked** time. The top bar retains the last full-event update time; a quick fetch does not claim that every category was refreshed.

Use **Update event** for a complete event refresh. Full and quick fetches share one busy guard. Failed or missing-category responses keep the previous results and checked time. A pending source cannot erase previously published medals, and responses from an event left during the request are discarded.

All header buttons now have the same 38-pixel height and alignment. The timestamp and connection badge sit on a separate status line. Opening Tools does not change the button's label or shift the header.

Close an older running copy and open **JudoCeremony.exe** from the complete 0.20.3 folder. The project launcher also selects this build when present. Event files remain schema 9; poster projects remain format 2. Download the [v0.20.3 Preview](https://github.com/YOUNESMAAFI/judo-ceremony-releases/releases/tag/v0.20.3).
