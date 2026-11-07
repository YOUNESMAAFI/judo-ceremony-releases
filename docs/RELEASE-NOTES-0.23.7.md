# Judo Ceremony Desk v0.23.7 Preview — square staff exports

This release includes the changes since the published v0.23.1 preview.

- **Square staff images:** choose **Preparation → Image ratio → Square (1:1)** for a 2400 × 2400 image, or keep **Screen (16:9)** at 2400 × 1350. The preview, Copy image and Save PNG use the selected format, which is saved with the event.
- **Corrected spacing:** two square flags are separated and centred as a pair. Bottom tables follow the flag labels with a consistent gap, and the flags and table are balanced together for each medal preset in both orientations. Footer logos and hashtags retain their space.
- **Table placement:** staff and audience outputs independently offer Top right, Bottom left and Bottom centre. Staff tables can include athlete names; audience output continues to omit them.
- **Background artwork:** Appearance offers Premium judo · Wide, Premium judo · Square and Premium judo · Crimson, with thumbnails. Artwork is bundled for offline use and embedded when selected; darkening and custom artwork remain available.
- **Short podium readiness:** usable gold-and-silver results can be Ready without two bronzes. Final block, remembered social results and country standings share the rule. Pending, disputed and bronze-only results remain unready.

## Install and compatibility

Download **JudoCeremony-0.23.7-win-x64.zip**, close the older app, extract the complete ZIP and open **JudoCeremony.exe**. The Windows x64 runtime, flags, bundled recordings, examples and illustrated guide are included. No separate .NET installation is required.

Event files remain schema 9, compatible with 0.20 and later. Older events default to screen-shaped staff exports. Audience settings remain independent of staff images.

## Validation

- Final v0.23.7: 40 staff-image checks and 292 focused athlete, table-placement and related checks passed; suites overlap in coverage.
- The square exports, including the two-medal crimson example, were rendered and visually reviewed.
- Windows x64 package verification passed native and fresh-session startup, saved-event reopening/autosave, clean shutdown, icon, schema 9, 442 reference-image hashes and 146 anthem hashes. An initial cold-start timeout passed on retry.
- Earlier full regression runs in this release series passed 847 checks for v0.23.4 and 859 for v0.23.5; these are not counts from a final v0.23.7 full run.
- Compilation and self-contained publishing succeeded. NuGet advisory lookup emitted NU1900 while the package service was unavailable.

Published as a preview, consistent with earlier releases. Physical HDMI, mixed display scaling, clipboard paste into the venue's chosen app and venue audio rehearsal remain manual.
