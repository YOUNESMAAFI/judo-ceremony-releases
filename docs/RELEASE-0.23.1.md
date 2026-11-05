# Judo Ceremony Desk v0.23.1 Preview — guided event creation

Start a competition with the visible **+ New event** button or **Event → New event**. The setup window offers three routes:

- **Choose from IJF:** select a year, click **Load IJF calendar**, search by name or location, and filter **Past**, **Current**, **Upcoming**, or **Dates unavailable**. Select a competition to fill the link and category group, then **Connect event**. **Copy selected link** copies its official IJF URL.
- **Paste a link:** paste an official IJF competition URL directly and choose **Connect event**. This route remains available if calendar loading fails.
- **Create manually:** enter a local event name and choose **Create manual event**. Manual preparation works offline.

The current event is saved to history after accepting setup. Cancel keeps it open. Creating another event preserves the loaded audience ceremony. A selected IJF event's name, dates and source link are saved before fetching results, so an upcoming event can be set up before medals are published. Use **Update event** later to retry or refresh.

The calendar includes all IJF competition categories for the chosen year. Current includes both the published start and end date, compared with the PC's local date. Postponed and TBD entries retain the published notice without guessed dates. Loading the calendar and fetching event data require internet access. Existing saved event files remain schema 9, compatible with 0.20 and later.

## Validation

- 16 event-creation checks passed: calendar parsing, date boundaries, postponed events, search, filters, selection, clipboard copying, link validation, cancellation, history preservation, manual creation, and upcoming events with unavailable results.
- 813 regression checks passed. Native audio transport reran; unchanged bundled recordings matched the existing successful Windows decoder audit by SHA-256.
- 31 focused event-workflow checks passed (included in the regression suite).
- Live calendar import loaded 212 competitions, seven without published dates, on 5 November 2026 (Africa/Lagos).
- Native Windows x64 package verification passed fresh startup, saved-event reopening/autosave, clean shutdown, embedded icon, schema 9, 442 reference-flag hashes and 146 anthem hashes.

## Install

Download **JudoCeremony-0.23.1-win-x64.zip**, close the older app, extract the entire ZIP and open **JudoCeremony.exe**. The Windows runtime, flag assets, bundled recordings, examples and guide are included. No separate .NET installation is required. Published as a preview, consistent with the previous release.
