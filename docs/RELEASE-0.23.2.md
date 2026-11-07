# Judo Ceremony Desk v0.23.2 Preview

- In **Preparation → Image visibility…**, enable **Results table**, **Athlete names in table** and **Table at bottom left** to place the named medal table in the lower-left corner. Clear the position option to restore the top-right table.
- The audience screen has its own **Table at bottom left** option. Athlete names remain exclusive to staff images and social posts.
- Both table positions save with the event. Flags leave space above a bottom-left table; the hashtag and bottom logo retain their footer positions.
- Categories with usable gold and silver medals now show **Ready**, even with zero or one bronze. Four-medal exceptional layouts remain supported. Bronze-only, pending, disputed and unresolved results remain unready. Final block, social category readiness and country standings share this rule.
- Existing schema 9 event files remain compatible. Events without the new position option keep the original top-right placement.

This is a local preview build. Close the older app and use **Start Judo Ceremony.cmd** or open **dist/JudoCeremony-0.23.2/JudoCeremony.exe**.

## Validation

- 269 focused athlete and placement checks passed, including saved positions, independent outputs, hidden audience athlete names, bottom-left pixel bounds and flags remaining offscreen before animation.
- 265 focused remembered-result checks passed, including green gold-and-silver-only rows in Final block and Social posts. These overlap with the athlete suite.
- 56 country standings checks passed.
- Vertical and horizontal staff exports were visually reviewed.
- Native package verification passed fresh startup, saved-event reopening/autosave, clean shutdown, embedded icon, schema 9, 442 reference-flag hashes and 146 anthem hashes.
- Build and self-contained Windows x64 publish succeeded. NuGet's online vulnerability metadata check was unavailable in this network-restricted environment (NU1900).
