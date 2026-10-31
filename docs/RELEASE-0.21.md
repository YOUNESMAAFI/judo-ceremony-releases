# Judo Ceremony Desk 0.21 — update changes and automatic refresh

This release adds a top-bar **Changes** panel and an optional full-event refresh timer. The existing four workspaces and separate staff/audience settings are retained.

## Review what changed

1. Use **Update event** for the competition, or **Fetch category** for one selected category.
2. Open **Changes** beside Update event in the top bar.
3. Select a recent check to review its category-by-category changes.

Reports identify newly confirmed gold/silver medals, new bronze and fifth/seventh-place results, changed countries, added/corrected athlete names, removed results, updated final-block matchups and changed review notices. Previous and new values are shown for corrections.

An unchanged check has its own report. The last **20 successful checks** are retained in this app session, including checks made by the timer. Failed checks retain earlier reports. Reports are cleared when switching events or restarting; saved event results remain available and provide the baseline for the next comparison.

The comparison uses the applied event snapshot. Pending source pages that retain known medals do not falsely report deletions. Reordering two bronze, fifth or seventh results does not produce a change. Separate athletes from the same country remain separate results. The report concerns results and matchups; event metadata and participation changes are outside this summary.

## Enable the timer

Connect an IJF event first. In the top bar, check **Auto-refresh**, then select **2 seconds**, **5 seconds**, **10 seconds**, **30 seconds**, **1 minute**, **2 minutes** or **5 minutes** beside it. Select **Custom…** to enter any whole number from **2 to 3600 seconds**. One minute is the default interval. The checkbox, interval selector and countdown are always visible, without opening Changes.

The timer refreshes the full event and shared social-post results across all workspaces. It starts **off** each session and is switched off when changing events. It never opens a connection dialog or starts a request without a connected event.

Manual and automatic requests share one busy guard. The interval is measured after a check finishes, so a slow request never overlaps another check. A failed request keeps saved data and retries after the selected interval. Invalid custom values pause requests until corrected. While an event input is being edited, the timer waits. An automatic response that arrives during editing is deferred, leaving the input and keyboard focus intact. Focus in the timer's own controls does not block updates.

The timer never prepares, loads or starts an audience ceremony. Entered preparation, loaded flags and audio controls remain under the operator's control. Stop the timer by unchecking its box.

## Files and compatibility

Event files remain **schema 9**, readable by 0.20 and newer. No flag artwork, recordings or poster file formats changed. Timer preferences and the recent change-report history are session controls, not event-file fields.

## Validation

Focused checks cover multiset comparisons, duplicate-country medals, no-gold podiums, name/country corrections, top-eight additions, partial and failed fetches, quick-category isolation, report selection, header/popup geometry, countdown intervals, the actual dispatcher timer, shared request exclusion, audience/preparation preservation, editing deferral, stale responses, event switching and shutdown.

The focused report/timer checks include direct timer visibility and header geometry at 1040 and 1400 pixels. Existing event-update/workflow, category-fetch/header and focused queue/update checks also passed. The suites overlap; their counts are not a unique total. A physical HDMI and venue-audio rehearsal remains manual.
