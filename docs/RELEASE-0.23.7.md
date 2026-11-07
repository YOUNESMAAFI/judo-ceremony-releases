# Judo Ceremony Desk v0.23.7 Preview

Square staff images now centre a two-flag pair with a clear horizontal gap, fixing the overlap between the larger portrait flags.

A bottom results table follows the actual flag and label bounds instead of remaining pinned near the bottom edge. The flags and table are centred together within the square body, keeping a compact gap for one, two, three and four medals, both flag orientations and the two-silver layout. Footer artwork and hashtags retain their own space.

Close the older app and use **Start Judo Ceremony.cmd**, which selects **dist/JudoCeremony-0.23.7/JudoCeremony.exe**.

## Validation

- All 40 staff-image checks passed, including pixel bounds for the flag gap, the distance from labels to the table, centring, each medal preset in both orientations, footer clearance, export dimensions and saved settings.
- All 292 focused athlete and existing table-placement checks passed.
- The two-medal crimson export was rendered and visually reviewed.
- The Windows x64 package passed native startup, fresh-session startup, autosave, clean shutdown, icon and bundled asset verification after an initial cold-start timeout.
