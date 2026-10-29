# Judo Ceremony Desk 0.14.1 — today's categories and fetch status

This preview separates multi-day IJF competitions by their published schedule and makes connection/fetch status visible. It retains the final-block planning workflow from 0.14.

## Categories by day

The import preview and **6 Final block** open on **Today**. Only categories assigned to the event's current local date appear. Buttons such as **Day 1 · 29 Oct**, **Day 2 · 30 Oct** and **Day 3 · 31 Oct** select another day. An empty day stays empty; it does not fall back to every category. Other days remain saved with the event and can be reviewed separately.

The app reads the **Competition scheduled** table on the official IJF overview. Published DAY numbers are mapped to dates using the event start/end dates. It reads the event timezone when provided, so today's categories change at midnight in that timezone. If the timezone is unavailable, the UI identifies the PC-date fallback. An open Today view checks for date rollover every 30 seconds without fetching the network.

Missing, inconsistent or unsupported schedule data is labelled **Schedule unavailable**. Those categories are kept separately and are never assumed to compete today. Older saved 0.14 plans have no dates until **Load / reload event… → Read results → Load event & wait** imports the schedule. A temporarily unreadable schedule on reimport retains the saved dates for the same source/category.

The import action is now named **Load event & wait**. It saves the event's categories and unranked matchups by day. Day selection only filters the view; it never clears country entries or changes the loaded audience ceremony or anthem. Regular **Refresh results** updates medals; reloading the event updates the schedule and matchups too.

## Connection status

The operator header and Final block show the latest IJF connection status:

| Status | Meaning |
| --- | --- |
| IJF NOT CHECKED | No IJF response has been checked in this app session. Import or refresh to check. |
| CHECKING IJF… | A request is in progress. |
| ONLINE · IJF | A recent IJF request succeeded. |
| IJF UNAVAILABLE | The last request failed or timed out while a network connection exists. |
| OFFLINE | Windows reports no network connection. |
| IJF CHECK OUTDATED | The latest connection result is more than two minutes old. |

The tooltip gives the latest connection-check time. Status is based on actual IJF requests and Windows network availability, not a promise of continuous connectivity. The header checks local network availability every ten seconds; it does not make background HTTP requests just to keep the badge green. Optional result polling remains available while Final block is open.

## Latest successful fetch

Final block displays **Latest successful results fetch**, including date, time, seconds and UTC offset. The import preview also identifies its latest successful fetch. The saved plan retains this time across reopening. A successful fetch updates it even when medal results remain pending. A failed or cancelled fetch retains the previous successful time and saved data. This is independent of the source's medal-data time, so an incomplete page cannot erase a previously published podium.

## Compatibility and checks

Event schema remains **6**. Day, timezone and successful-fetch metadata are optional additions; earlier schema 1–5 files and undated 0.14 plans still open. Use 0.14.1 or newer to retain and use the day metadata when resaving. Portable backups include the new fields with the event.

**477 software checks passed.** Checks cover the official Abu Dhabi three-day split, a separate two-day schedule with a different category order, event-local midnight, dates outside the event, missing/conflicting schedule data, import and workspace filtering, day selection across refresh, saved day metadata, network success/failure/cancellation and preservation of the successful-fetch timestamp on errors. The live IJF full-event and schedule import also passed. Full regression and package results are included with the local build.

The live importer was checked against the [IJF Abu Dhabi Grand Slam 2026 schedule](https://www.ijf.org/competition/3157) on 29 October 2026. Its published individual categories are split 5 on Day 1, 4 on Day 2 and 5 on Day 3. The original flag and anthem assets remain unchanged.
