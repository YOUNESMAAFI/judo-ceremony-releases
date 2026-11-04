# Judo Ceremony Desk 0.22 — confirmed winners in Final block

The gold and bronze matchup columns now highlight the confirmed winner's three-letter code with a gold background, bold text and a checkmark. The other contestant remains unmarked. Hover over a matchup to see the contestant names and confirmed winner.

Winner marks use published medals, not bracket CSS styling. Completed bronze contests can show winners while the gold final is still pending. Pending, incomplete, conflicting and ambiguous matchups remain neutral. A two-silver/no-gold result does not invent a gold winner.

The draw importer now retains optional contestant names. They distinguish same-country matchups and countries appearing in both bronze contests. Use **Update event** once to refresh older saved draws; **Fetch category** continues to read only the results page and retains the existing draw names.

For an old saved matchup with unique country codes, country-only evidence can identify a winner. If the same country occurs more than once and contestant identity is missing or ambiguous, the app leaves it neutral rather than guessing. Comma separators, whitespace and case are normalized; other name mismatches remain unconfirmed.

Published corrections update the marks after a full or selected-category fetch. A later pending page retains marks for previously retained medals. Category readiness colours, manual preparation, the loaded audience and the ceremony queue keep their existing behavior.

Event files remain schema 9. Contestant names are optional fields; older files open without migration. Older apps can ignore or drop the optional names when saving, so refresh the full event again when returning to 0.22 if same-country marks are missing. Staff/ceremony output preferences and poster formats are unchanged.

These changes are included in [v0.23.0 Preview](https://github.com/YOUNESMAAFI/judo-ceremony-releases/releases/tag/v0.23.0). Close an older copy, extract the complete Windows ZIP and open JudoCeremony.exe.

The build passed 29 winner-highlighting checks, 17 category-fetch/header checks, 31 event-update/workflow checks and 262 focused final-block checks. These suites overlap. Coverage includes partial medals, same-country matchups, repeated countries, ambiguous names, no-gold results, saved data, real WPF rendering, result corrections and preparation/audience isolation.
