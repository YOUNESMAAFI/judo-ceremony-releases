# Judo Ceremony Desk 0.9 - separate image and ceremony controls

On **1 Preparation**, open **Image visibility...** beside the staff preview. Its checkboxes control the staff preview, Copy image and Save PNG only. Changes apply immediately. The preview now uses the same staff layout and appearance as the exported image.

On **2 Ceremony display**, **Audience screen visibility** controls only the audience preview and HDMI screen. Changes apply immediately without changing countries, elapsed time, pause or blackout. Staff image visibility is unaffected.

Each output independently controls tournament title, contest category, flags and labels, medal labels, three-letter codes, full country names, results table, event hashtag and logos. Hiding flags disables the attached-label controls for that output only. Background and logo artwork continue to be configured through Appearance; their visibility choices are separate.

Both sets of preferences are saved with the current event, historical events and exported tournament files. Opening another event restores its staff preferences while the loaded ceremony keeps its existing audience settings until replaced or explicitly edited.

Older shared preferences are copied to both outputs when schema 1, 2 or 3 files are opened, preserving their appearance. The settings then work independently. Version 0.9 saves schema 4, which earlier apps reject instead of silently dropping the independent settings. Close older versions before launching this build.

The 0.8 behavior for empty startup, per-category countries, event history and country-only Tab navigation is retained. Flag artwork is unchanged from the supplied reference audit. The audit PDF describes the 0.7 flag review; `RELEASE-0.9-checks.txt` records this version's software check count. Physical HDMI rehearsal remains necessary; anthem audio remains deferred.
