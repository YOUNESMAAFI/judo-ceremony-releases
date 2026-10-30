# Judo Ceremony Desk 0.15.0 — ceremony queue and version checks

This preview adds a saved ceremony order for each day and a manual check for newer Windows releases. It builds on the day filtering, IJF connection status and successful-fetch timestamps in [0.14.1](RELEASE-0.14.1.md).

## Plan the ceremony order

Open **6 Final block**, choose **Today** or a dated competition day, then select **Ceremony queue**.

1. Use **Add this day** to queue the selected day's scheduled categories, including categories still waiting for medals. Import the event schedule first. Adding the same day again keeps the existing entries without duplicating them.
2. Use **Add preparation** to add a category whose medal countries you have prepared manually. Choose its scheduled day if one exists. Without a published date, the selected dated day is used; Today uses the event's local date, with the PC date as fallback when no usable timezone exists.
3. Select an entry and use **Move up**, **Move down** or **Remove** to adjust the order. Moving an entry changes only its own day's order.
4. Review the selected entry's medal table. **Load selected** loads that podium; **Load next →** loads the first unfinished entry in the displayed day's saved order. Loading opens Ceremony display at the starting position. Press **Play** when ready.
5. Once the flags have finished rising and the anthem is stopped, choose **Mark finished** in the queue. Completion is explicit: reaching the top does not mark the entry finished automatically.

The queue shows **Waiting**, **Ready**, **Review layout**, **Loaded**, **Playing**, **Paused**, **Awaiting finish** or **Finished**, as applicable. A queued category becomes ready when it has a valid prepared podium or readable published medals. Imported unusual medal layouts require **I checked this unusual medal layout** before loading. A no-gold podium selects no winner anthem.

**Load next →** waits when the first unfinished entry is not ready; it does not skip ahead to a later ready category. Use **Load selected** or change the order when officials choose a different ceremony. Loading through the queue is blocked while flags are rising or paused, or while ceremony audio is active. The active entry cannot be removed during that time.

The active ceremony retains its loaded countries when Preparation is edited. Finished entries save the medal countries actually presented, so later edits do not rewrite the completed podium. A finished entry can be selected and loaded again when playback permits; this clears its finished state until it is marked finished again.

Queue order, dates and completion are saved with the event and included in portable backups. Entries follow the selected day, including queued days without an imported final-block plan. The same category can appear on different dates, but only once per date. The event supports up to 2,000 queue entries.

## Check the installed version and newer releases

The window title and version button show the installed version. Open **Version and updates**, then choose **Check for updates** to check the public Windows releases in the [official release repository](https://github.com/YOUNESMAAFI/judo-ceremony-releases).

The dialog compares numeric versions and includes published previews. Drafts and releases without a matching Windows x64 application ZIP are ignored. The result shows the newest eligible version, preview status, download size and latest successful check time.

When a newer version exists, **Download newer version** opens its official release page in the browser. Download and extract the Windows ZIP, close the older app, then run the new copy. Installation is manual.

Checking requires internet and happens only when requested. A failed or timed-out request reports **Update check unavailable** and retains the dialog's last successful check time. It does not report that the installed app is current after a failed check.

## Compatibility and backups

Event files now use **schema 7** to retain ceremony order and completion. Schema 1–6 files still open; events without queue data start with an empty queue. Files saved by 0.15 require **0.15 or newer** to reopen. Older apps reject schema 7 rather than silently dropping the queue.

Portable backups created by 0.15 also require **0.15 or newer** to restore. Earlier supported backups remain readable. Backup recording selection includes countries in completed queue podiums; readiness also includes them when no participant list supplies the country scope.

## Verification

The 0.15 build succeeded with **0 errors**. It recorded NuGet vulnerability-data warnings because the NuGet service index could not be reached.

The focused queue/update run passed **163 checks**, covering event data and backup compatibility, queue order and day filtering, duplicate prevention, pending-to-ready results, explicit completion, playback guards, completed-podium retention, unusual-layout review and update-response handling. The queue and update dialog were rendered and inspected.

The full regression passed **511 software checks**, including native Windows decoding of all 146 bundled recordings. The live unauthenticated GitHub update check passed and found the current published Windows preview. The self-contained 0.15.0 package passed native launch, fresh startup, schema 7 migration, app icon, 442 flag-reference hashes and 146 anthem hashes.

Results are recorded in `artifacts/checks-0.15`, `artifacts/checks-0.15-live` and `artifacts/release-audit-0.15`. Physical HDMI and venue audio rehearsal remain part of event setup.

The updater reads the public [GitHub releases API](https://docs.github.com/en/rest/releases/releases#list-releases). Rehearsal screenshots use illustrative queue medal results; confirm approved podiums before live presentation.
