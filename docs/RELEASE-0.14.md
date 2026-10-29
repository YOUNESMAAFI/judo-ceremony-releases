# Judo Ceremony Desk 0.14 — load the final block and wait

This local preview adds a saved final-block workspace. An event can be prepared as soon as IJF publishes the finalists, before medal results exist. Previous preparation, staff export, ceremony controls, anthems, readiness and portable backups remain available.

## Load everything before the finals

1. Start **New event** when changing competitions. Open **Import IJF medal results…** on Preparation, or **Load / reload full event…** on **6 Final block**.
2. Paste an official IJF competition link and click **Read results**. The app reads the results, event information, Nations list and each supported individual category draw.
3. Review the source event and category group. The preview shows known **Gold-medal contest**, **Bronze A** and **Bronze B** contestants as white/blue three-letter codes. Undecided contestants are **TBD**. These are matchups, not medal assignments.
4. Select **Load all & wait**. All imported result categories and available final-block matchups are saved with the current event. Available participation and event details are included; an existing event name is retained and an empty name is filled. Category presets are merged with the existing choices. Existing manually entered medals remain intact.

Illustrated examples are included in the [user guide](../README.md).

The category list includes weights with only fifth/seventh-place results or an explicit “No results were found” notice. These say **pending medals** instead of reporting an invalid medal layout. Matchups are read from the final and bronze rounds of the published draw. Semifinal winner styling is never treated as a gold-medal result. Same-country contestants remain separate entries. No athlete names are stored.

## Wait for published results

**6 Final block** lists every saved category, the three final-block contests and medal availability. The detail pane shows published medal countries for the selected category.

- **Refresh results** checks the official result pages and updates the saved plan.
- **Refresh every 30 seconds while this tab is open** starts unchecked. Enable it to poll results while waiting. Leaving the tab stops the timer; returning resumes it if still checked. Closing the app stops requests. This preference is not persisted.
- **Load / reload full event…** rereads draws if finalists or bronze contestants have changed. Regular result refresh does not reread draws or participation lists.
- **Prepare selected podium** becomes available for a readable published result. Unusual medal layouts require the review checkbox. Preparation receives those approved medal countries; then explicitly load the preparation to the audience.

Refreshing changes the saved plan, not the entered medal countries, loaded audience flags, flag timing or anthem. A pending page cannot erase previously published medals, including during a full reload of the same source/category. Responses received after changing events or replacing the plan are discarded. Failed requests retain saved data. Results and source timestamps are snapshots; the app does not decide which official result is approved for presentation.

## Supported data and limits

Supported individual categories use the published Men/Women weight tables and standard IJF final/repechage bracket structure. Team, round-robin or changed page structures may not provide readable matchups; the app shows a notice and keeps the result data it can read. Missing contestants stay TBD. Unsupported delegation codes are shown for review rather than substituted with another flag. An unreadable medal result cannot be prepared automatically.

Full-event import uses at most three simultaneous category-draw requests. Internet access is needed for importing and refreshing. Saved plans, entered results, flags and bundled audio work offline. Optional refresh runs only in the open Final block workspace; it does not run after exiting the app. Check current organiser results before loading a podium.

## Files, history, readiness and backup

Version 0.14 writes **event schema 6** to preserve final-block categories, unranked matchups, pending states, published medal snapshots and source information. Schema 1–5 events still open with an empty final-block plan. Earlier application versions reject schema 6 instead of silently discarding the plan. Close older versions before launching 0.14.

Plans are retained by autosave, event history, ordinary tournament exports and portable event backups. Backups remain **backup format 1**, but the embedded schema 6 event requires **0.14 or newer** to restore. Older 0.13 backups still open in 0.14. Imported country recordings for known final-block contestants are included when backing up, along with other event recordings. Readiness includes the plan's countries when no participant list exists.

## Verification

Validation covers all 14 Abu Dhabi 2026 individual categories in a recorded pre-final snapshot, known gold and both bronze matchups, same-country contests, undecided future contestants, pending versus malformed result pages, and the transition to published medals using synthetic completion data. Synthetic medal results are test data, not a claim about the event outcome.

Additional checks cover schema migration, save/reopen, portable backup round trips, readiness coverage, preview controls, preservation of manually entered countries and loaded flags/audio, retention of published medals after incomplete responses, and changing events during an outstanding request. **457 software checks passed**, including native Windows decoding of all 146 bundled recordings. The self-contained 0.14.0 package passed native launch, empty startup, save migration, app-icon, 442 flag reference hashes and 146 anthem-file hashes. Full results are recorded in the local validation artifacts.

The live full-event import was also checked against the public [IJF Abu Dhabi Grand Slam 2026 event](https://www.ijf.org/competition/3157), its [results](https://www.ijf.org/competition/3157/results) and [draw](https://www.ijf.org/competition/3157/draw) on 29 October 2026. The artwork and bundled recordings are unchanged from 0.13. Physical HDMI and venue sound rehearsal remain part of event setup.
