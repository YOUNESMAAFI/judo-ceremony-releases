# Judo Ceremony Desk v0.23.5 Preview

Open **Appearance… → Background presets** and select **Premium judo · Square** or **Premium judo · Wide**. Both include thumbnail previews and blue-and-gold artwork of two judoka performing a throw.

For a square staff image, also choose **Image ratio → Square (1:1)** above the Preparation preview. Background darkening and the option to include appearance in staff images continue to apply.

Selecting artwork embeds it in the event file for reopening, copying and backups. The packaged images are available offline. Existing color presets and custom image imports remain available.

Close the older app and launch **Start Judo Ceremony.cmd**, which selects the new local **dist/JudoCeremony-0.23.5/JudoCeremony.exe** build.

## Validation

- 859 regression checks passed; 13 final focused checks cover selection, embedding, save/reopen, image proportions, bundled fallback rendering, darkening, removing artwork and returning to color presets.
- The gallery and square ceremony export were rendered and visually reviewed.
- The self-contained Windows x64 build passed native startup, fresh-session startup, autosave, clean shutdown, embedded icon and bundled asset verification. Both packaged background images match the source hashes.
- Builds completed with no errors. NuGet advisory lookup emitted NU1900 warnings because the package service was unavailable.
