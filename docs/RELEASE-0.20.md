# Judo Ceremony Desk 0.20 — one event update

The app now has one visible IJF fetch action: **Update event** in the top bar. Connect a competition link once and choose its category group. Later clicks refresh that competition's event details, participants, daily schedule, known final-block matchups, published medals and top-eight results together.

**Last updated** stays beside the button on every workspace and is saved with the event. Failed requests keep the previous timestamp and results. **Partial update** means some source pages could not be read; hover over the time for details. Pending pages retain previously published medals. Updating never loads or plays an audience ceremony.

## Four main tabs

| Tab | Purpose |
| --- | --- |
| Preparation | Review a podium, choose appearance and copy/save the staff image. |
| Ceremony display | Choose the HDMI monitor, load the reviewed podium and operate flags/anthem. |
| Final block | Choose today or a competition day, review published medals and prepare a podium. The ceremony queue remains here. |
| Create social post | Use the same saved event results to create and remember posters. |

**Tools** opens Event history, Anthem testing and Event readiness. **Event** contains New event, Open tournament, Save tournament and Event backup. Country filters and manual participant editing remain under **Countries**.

## Daily workflow

1. Click **Update event**. On first use, paste the official IJF competition link and choose Senior, Junior, Cadet or a custom group.
2. Open **Final block**, choose Today or the relevant dated day, select the category and review its medals. Green is a complete four-medal podium; Partial and No results remain grey.
3. Click **Prepare selected podium**. Review Preparation and copy/save the staff image if needed.
4. Open **Ceremony display**, choose the monitor and click **Load prepared →**. Press Play when ready. The controls and shortcuts remain independent of fetching event data.
5. Open **Create social post** to prepare a poster. Its editor uses the saved event snapshot; The athlete rows refresh automatically from Update event, without another button or network request.

Manual entry works without an IJF link. Start a New event to connect a different competition. An update keeps the operator's existing event title, entered category results, active workspace and loaded ceremony. Network requests are serialized; a response belonging to an event left during the request is discarded.

## Saved posters and shared results

Top-eight results are now saved with the event, available after restart and included in event files/backups. No social-specific IJF link or fetch button is needed. Remembered posters automatically receive the updated athlete rows while retaining their saved design. An already-open editor refreshes as well; no second apply step is needed.

Remembered social-poster projects remain local per event/category. Use Save poster to move their designs to another PC. The event backup includes the shared IJF result snapshot but does not include these separate saved poster projects.

## Compatibility and review

Event files now use **schema 9**, requiring **0.20 or newer**. This prevents older versions from silently dropping the shared top-eight results and update timestamp. Schema 1–8 events still open; their existing medals, queue and appearance are retained. Older events show Last updated: Never until their first unified event update. Poster projects remain format 2.

The 0.20 native launcher is `dist/JudoCeremony-0.20/JudoCeremony.exe`; **Start Judo Ceremony.cmd** selects it when present. This build is local until explicitly published. The [boss demonstration guide](BOSS-DEMO.md) gives a short review sequence. Physical HDMI, speaker routing and organizer approval of results remain checks on the event equipment.


692 regression checks passed. Native launch, fresh start, schema 9 reopening, 442 flag-reference hashes and 146 anthem hashes passed. The unchanged recordings match the successful Windows decoding audit; native audio controls were checked again. Physical HDMI and venue-speaker rehearsal remain manual.
