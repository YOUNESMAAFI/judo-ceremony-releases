# Judo Ceremony Desk 0.23 — country standings for social media

**Create social post → Country standings** adds national result tables for one competition day or the whole event. The existing Category posts view and its four athlete layouts remain available alongside it.

Tables include horizontal flags, three-letter codes, full country names, gold/silver/bronze counts, fifth and seventh places, and total medals. Ranking compares gold, silver, bronze, fifth, then seventh. Exact ties share a competition rank (1, 1, 3), with codes ordering tied rows consistently. Two athletes from the same nation are counted separately; a two-silver/no-gold result never adds a gold medal.

Select Whole event, Today, a dated day, or Schedule unavailable. Today uses the event timezone where available. Whole event includes undated categories; day filters do not mix those categories into a dated day. Medal-winning nations appear by default; a checkbox also includes nations with only fifth/seventh places.

Choose Light, Navy, Magenta or Teal and portrait (1080 × 1350), square (1080 × 1080), or story (1080 × 1920). Optional event backgrounds, three logos and the hashtag carry into the export. Copy or save the current page, or save all pages to a separate folder. Portrait pages hold 15 nations, square pages 10, and story pages 20. Each page keeps its global ranks, source-check time and page number. A multi-page export captures one dataset so updates arriving during export cannot mix snapshots. Existing output files are preserved.

The table reads the shared saved IJF event snapshot, including every nation regardless of the country-picker filter. The top-bar Update event, automatic refresh and selected-category fetch update its totals. It has no additional network/import action. It uses medals once from the medal list, and only fifth/seventh rows from the top-eight list. Category poster edits, preparation and audience controls remain independent.

Pending categories are listed, usable partial medals count, and disputed category results are excluded. Missing/disputed lower placings or unmapped codes are disclosed and mark the exported table provisional. No missing results are inferred. An event with no eligible results has export controls disabled.

Saved event files and backups already include the shared results, so country standings can be recreated offline without another fetch. This feature adds no event schema fields: files remain schema 9. Standings export preferences are retained within the current event/session; their format, theme and filter selections reset for another event and are not separate saved poster projects. Manual preparation and poster-only entries do not feed the national table.

This build also includes the 0.22 confirmed-winner highlights in Final block. See [the winner notes](RELEASE-0.22.md) for identity matching and older-draw behavior.

These changes are included in [v0.23.0 Preview](https://github.com/YOUNESMAAFI/judo-ceremony-releases/releases/tag/v0.23.0). Close an older copy, extract the complete Windows ZIP and open JudoCeremony.exe.

Validation passed: 56 country-standings checks, 29 winner-highlight checks, 31 event-update/workflow checks and 269 focused social checks (suites overlap). The native Windows x64 build passed fresh startup, saved-event reopening/autosave, embedded icon, schema-9, country-region snapshot and all 442 reference-flag and 146 anthem file hashes. Portrait, square, story and the WPF workspace screenshots were inspected visually. These checks used fictional data and isolated storage, without changing the operator's current event.
