# Judo Ceremony Desk v0.23.3 Preview

**Table position** now offers **Top right**, **Bottom left** and **Bottom centre** in **Preparation → Image visibility…** and **Ceremony display → Audience screen visibility**.

The medal table and enabled staff athlete names can be centred beneath the flags. Centre placement leaves room for the footer logo and hashtag. Names remain limited to staff images and social posts. Both outputs save their own position; existing bottom-left settings are retained.

Close the older app and use **Start Judo Ceremony.cmd** or **dist/JudoCeremony-0.23.3/JudoCeremony.exe** for this local preview.

## Validation

- 274 focused athlete and placement checks passed, including centre bounds, independent saved positions, original left/right placement, hidden audience names, offscreen animation starts and footer clearance.
- Horizontal and vertical centre exports and a logo/hashtag example were rendered; the footer example was visually reviewed.
- Self-contained Windows x64 build and native startup/autosave/clean-shutdown verification passed, including 442 reference flag hashes and 146 anthem hashes.
- NuGet's online vulnerability metadata check was unavailable in the restricted network (NU1900); compilation and publishing succeeded.
