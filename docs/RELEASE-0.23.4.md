# Judo Ceremony Desk v0.23.4 Preview

Preparation now has an **Image ratio** selector above the staff preview:

- **Screen (16:9)** exports at **2400 × 1350**.
- **Square (1:1)** exports at **2400 × 2400**.

The preview, **Copy image** and **Save PNG** all use the selected ratio. Square images arrange the titles, flags, logos, results table and hashtag across the square canvas without cropping or stretching the flags. Select **Image visibility… → Table position → Bottom centre** for a wide results table beneath the flags, including enabled athlete names.

The event remembers the staff image ratio when saved, reopened or restored at startup. Existing events continue to use Screen. Audience output remains independent.

Close the older app and use **Start Judo Ceremony.cmd** or **dist/JudoCeremony-0.23.4/JudoCeremony.exe** for this local preview.

## Validation

- 17 focused checks cover the actual ratio selector, both flag orientations, all three table positions, PNG dimensions, square preview bounds, footer clearance, animation start, audience isolation, saved events, older events and restart recovery.
- Square exports and the actual Preparation UI were rendered and visually reviewed.
- The full regression suite passed all 847 checks, including existing screen exports, audience rendering, persistence and native anthem decoding.
- The self-contained Windows x64 package passed native startup, fresh-session startup, autosave, clean shutdown, embedded icon and bundled flag/anthem hash verification.
