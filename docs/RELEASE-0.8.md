# Judo Ceremony Desk 0.8

## Event preparation

- The application starts with no selected category, no medal countries and no prepared flag/recap graphics. The current event name, appearance, hashtag, category presets and display preferences are remembered.
- Select a category to enter its results. A category not yet entered has empty countries and the standard gold/silver/two-bronze medals.
- Return to a previously entered category to restore its own countries and medal layout. Different age divisions and weights have independent results. Incomplete entries and cleared countries are preserved too.
- New event saves the current event to history and starts an empty event. Editing the current name renames that event; New event creates a separate identity, including when event names match.
- Event history lists previous events and their saved category countries. Open an event, then choose a category to restore its results. The event being left is saved first. Entered countries in an unnamed event are retained under Untitled event.
- Starting or opening another event and changing category leave the loaded audience ceremony unchanged until explicitly loaded. Visibility checkboxes retain their existing immediate behavior.

## Country keyboard navigation

Tab moves to the next enabled country field and cycles from the fourth back to the first. Shift+Tab moves backwards. Medal-rank dropdowns are skipped, and Not awarded country fields are skipped. Dropdowns remain available by mouse. The medal-layout preset is outside this country-field cycle.

## Storage and compatibility

The current event autosaves in `%LOCALAPPDATA%/JudoCeremony/last-tournament.json`. Event history uses the `events` subfolder, with individual event files and an index. History stays on this PC; exported tournament files contain that event's categories, not other events.

Version 0.8 saves schema 3. Earlier releases reject these files instead of silently dropping category results. Schema 1 and 2 files are still accepted: their existing podium becomes a saved category before the preparation screen is cleared. Select that category to retrieve the original countries.

Close older versions before launching 0.8. Keep the entire portable folder together. The existing session lock prevents simultaneous copies from writing to the same saved session.

## Verification

The regression suite exercises category isolation, exceptional medals, same-name event identities, renaming, unnamed event drafts, damaged history indexes, old-session migration, empty startup/restart, real WPF history controls and both directions of country Tab navigation. Tests run with automatic app startup disabled and isolated data directories, so the running event session is not opened by the test host.

`docs/RELEASE-0.8-checks.txt` contains the final check count. The native Windows package is also checked with `scripts/verify-release.ps1` using an isolated saved sample.

The flag artwork is unchanged from the searchable 0.7 audit included under `docs/audit`. That report's software check count describes 0.7. Physical HDMI, DPI, cable reconnection and staff clipboard rehearsal remain necessary on event hardware; anthem audio remains deferred.
