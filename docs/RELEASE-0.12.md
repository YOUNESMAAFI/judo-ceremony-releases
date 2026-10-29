# Judo Ceremony Desk 0.12 — event readiness and IJF medal results

## Event readiness

Open **5 Event readiness**. The panel checks the current event and preparation without changing countries, starting audio or moving flags. Use **Refresh checks** after changing participation, importing recordings or reconnecting a display. The report records its check time; it is a snapshot, not continuous monitoring.

If a competition participant list exists, the country table checks the entire list, including countries outside the selected regional filter. Unmatched IJF delegation codes remain visible. With no participant list, the report checks countries already entered across the current and saved categories. An empty event asks for participants or medal entries instead of auditing unrelated worldwide entries.

The panel reports:

- Event name and whether the current category has complete medal entries.
- Flag files for the selected horizontal/vertical orientation. Pinned IJF/Excel hashes detect changed reference files; uncovered artwork is marked for organiser review. Missing or unreadable files are identified independently of the scene cache.
- Missing, unreadable or changed anthem files. Failed tests known to the Anthem testing panel appear as needing attention. Available files are labelled bundled or imported.
- Connected screens, the selected audience target, whether the audience window is open and which category is loaded. Windowed preview is identified explicitly.
- Embedded background/logo readability. Custom backgrounds and logos remain optional.

**Anthem testing** and **Ceremony display** buttons open those workspaces. File availability does not prove Windows decoding, correct recording version, speaker routing, picture visibility or event approval. The venue rehearsal item remains for actual listening and screen inspection. Readiness is informational and does not block ceremony operation.

## Import medal results

On **1 Preparation**, click **Import IJF medal results…** below the tournament name. The event's saved IJF source link is filled in when available. Paste an official IJF competition URL and choose **Read results**. Nation/category query filters are removed so the importer reads the complete published individual results page.

The preview shows the source event, import time, category list, medal ranks, three-letter source codes and resolved full country names. The current category is selected when its label matches; otherwise select a category. Review the category group (Senior, Junior, Cadet or your own text), then choose **Apply this category**.

Applying fills preparation, selects that category and saves its country/medal entries. It retains the event identity, title, appearance, filters, other saved categories and the loaded audience ceremony/anthem. Load the preparation explicitly when ready to show it. Switching away and back restores the imported result; exported event files and history retain it like manual entries. Cancel and failed imports keep the current preparation unchanged.

Only published first, second and third places become medals. Repeated countries remain separate medal entries. Two bronze medals stay independent. Fifth/seventh places never become medals. A missing gold, two silvers or another short supported podium is shown exactly as published and needs the unusual-layout review checkbox before applying. Confirm that the published result is complete and approved; missing medals are never guessed.

Unknown delegation codes, missing medal markup, unsupported layouts and conflicting screen/print copies prevent automatic application for the affected category. Enter the result approved by officials manually in those cases. Identical print/screen copies are not combined. Team and other unsupported category formats are not imported as individual podiums.

When the saved IJF competition source differs from the results source, the preview requires acknowledging that change before applying. Start **New event** first when preparing a different competition. A custom event name alone is not an authoritative source identifier; always review the prominently displayed source event.

Results require internet access to download. Applied countries and medals work offline; the app does not continuously synchronize results or automatically load them to the audience.

## Compatibility and verification

Version 0.12 continues to use **schema 5**, shared with 0.11. Files from schema 1–4 still open; versions before 0.11 reject schema 5 exports. No new personal or athlete data is stored by medal import: the app reads category, place and delegation facts.

Verification includes recorded public IJF result facts and structure, real live result import, aliases, same-country medals, both bronze entries, no-gold/two-silver and short podiums, missing/unknown/conflicting results, rejected links/redirects, save/reopen/category isolation, preview Apply/Cancel, readiness file tampering and preservation of loaded flags/audio. The recorded fixture contains 14 completed Dushanbe 2026 individual categories. Country, flag and anthem assets are unchanged from 0.11.

Source: [IJF Dushanbe 2026 published results](https://www.ijf.org/competition/3353/results).

**Validation:** 400 software checks passed. The native Windows launcher, fresh start, icon, all 442 reference-image hashes and 146 anthem hashes passed package verification. Live IJF medal import passed for all 14 Dushanbe podiums. Physical event hardware rehearsal remains manual.
