# Release audit - Judo Ceremony Desk 0.7

Audit date: 27 October 2026. Reference policy confirmed by the organizer: use the newer April 2026 IJF manual and document differences from Excel.

## Assessment

Ready for management review. 149 software checks pass with zero build warnings/errors. The published Windows x64 EXE starts and closes with isolated test data; embedded icon and packaged reference hashes pass. Event use remains conditional on a physical HDMI rehearsal and review of the reference gaps below. This is a local functional/source audit, not IJF certification, a penetration test or an independent external audit.

## Display controls

The Ceremony display tab keeps monitor selection, Load, Play/Pause, Restart, Reset, Black screen, elapsed time and seconds controls visible. Nine checkboxes control tournament title, contest category, flags/labels, medal labels, three-letter codes, full country names, results table, hashtag and logos. Choices apply immediately to the loaded audience scene and preparation, are saved with tournament files, and do not change countries, elapsed time, paused state or blackout. Hiding flags hides their attached labels; the table independently retains three-letter codes. Keyboard Space remains available to focused checkboxes. Existing tournament files receive the previous visible defaults.

## Complete flag comparison

- 255 catalog entries x two orientations = 510 app views examined.
- 205 catalog entries use the April 2026 IJF manual in both views; hashes and page mappings are pinned.
- 16 more catalog entries use workbook-only artwork in both views (32 supplemental images).
- 34 catalog entries have no illustration in either reference and retain base artwork / rotation fallback, with an organizer-review reminder in the interface.
- Excel supplies 433 comparable views; 77 app views have no corresponding Excel picture.
- After correction: 421 close comparisons, 8 material differences in four countries, and 4 presentation/ratio reviews in two countries. These 12 remaining comparisons follow the newer manual by the organizer's instruction.
- Before correction: 220 close, 116 review and 97 material comparisons. Pixel scores are screening measurements, not federation approval.
- All 11 final comparison sheets were visually reviewed, including the six exceptions at larger size. Each appendix shows Excel/App for horizontal and vertical views. Country codes, full names, image labels, comparison statuses and scores are selectable, searchable PDF text; flags are separate images.

## Documented Excel differences

| Code | Manual page | Finding and disposition |
| --- | --- | --- |
| SWZ | 31 | Excel's SWZ-v picture depicts Sint Maarten, not Eswatini. Horizontal colours and emblem details also differ. The app uses Eswatini from the manual in both views. |
| NCL | 49 | Excel overlays a French tricolour on the Kanak artwork in both views. The app follows the single Kanak flag illustration in the newer manual. |
| PRK | 29 | Emblem placement, scale, colours and aspect ratio differ. The manual records design/colour updates in August 2025 and a ratio update in April 2026. The app follows its April 2026 illustration. |
| NMI | 51 | Excel calls this MNP. Blue tone, emblem scale and proportions differ. The app uses the NMI code and illustrations in the manual. |
| NEP | 49 | Both nonrectangular pennants remain intact. The manual's white rectangular image canvas differs from the workbook's transparent surrounding area. The source canvas is retained; review its appearance on a dark background. |
| NIU | 51 | The manual uses event proportions and a different canton scale from Excel. Both orientations retain the newer manual artwork. |

The PDF includes a side-by-side table on page 3 for all six countries above, showing the original Excel and current IJF/app flags in both orientations alongside the finding and decision.

For these country illustrations, page numbers are printed manual numbers; PDF viewer page numbers are four higher.

## Workbook source defects

The source was inspected as a ZIP/XML package without running Excel or VBA. Seven misnamed pictures were recovered by their worksheet country cell and orientation column. Existing correctly named pictures were never replaced by ambiguous duplicates.

| Source shape | Recovered as |
| --- | --- |
| Image 52 / Image 53 | BOT horizontal / vertical |
| ERIC-v | ERI vertical |
| Image 206 | LAT vertical |
| LBA-c | LBA vertical |
| Image 214 | LCA vertical |
| SFM-h | FSM horizontal |

The workbook contains 449 media objects and 455 drawing picture records, including duplicate/unused images. Its embedded pictures are identical to those in the downloaded v1.5e copy; this is a source-version difference, not evidence of a user edit.

## Coverage requiring organizer attention

Excel supplements: ANT, BER, DMA, ENG, ERI, GRN, MDV, FSM, OMA, SKN, VIN, SCO, TKL, TUV, IVB, WAL.

Outside both references: AIA, ATA, BVT, IOT, AHO, CXR, CCK, EUR, FLK, FGU, ATF, GIB, GRL, GGY, HMD, VAT, IMN, JEY, MRT, MAY, MNT, NIR, PCN, BLM, HEL, MAF, SPM, SGS, SJM, TKS, UMI, WAF, ESH, ALA.

The workbook country selector has AIN, COR, IJF, RJF and ZAN entries that the app does not offer. COR is also present in the manual but is not in this app catalog. The Excel AIN horizontal picture is a World Judo Tour banner; it must not be assumed to be an approved neutral-athlete flag. BAD, FUR and IRT are additional embedded placeholder/legacy images, not automatically added as countries. MNP is mapped to NMI and SFM-h to FSM. Check the participating delegation list before event use; events requiring unsupported entries need an approved addition.

## Verification and deployment limits

- PASS: 149 checks covering country codes/search, reference file hashes, all flag decoding, normal/reduced/no-gold medals, ties, snapshot isolation, timing, restart/pause/blackout, shortcuts, JSON compatibility/validation, image embedding, backgrounds/logos, visibility rendering, real XAML bindings, minimum window size and session locking.
- PASS: published native EXE launch/close using a separate data directory; Windows app icon extraction; published horizontal/vertical reference hashes.
- REVIEW: physical HDMI Extend mode, monitor selection, mixed DPI/resolution, audience distance/readability, cable removal/reconnection, clipboard paste into staff's target app, and the final event branding/delegations.
- Not included: anthem audio playback (previously deferred), automatic results import, unsupported delegation entries, installer or code signing. An unsigned app may show Windows reputation prompts.
- Rendering retains source colours, event proportions, emblems and source resolution, which can differ from generic national flag graphics. Resizing does not add detail; check sharpness on the actual screen, especially 4K. Nepal retains the manual's white canvas.
- Close older releases before launching 0.7; old releases do not implement the saved-session lock. Normal use is offline and has no third-party NuGet dependencies.

## Handover rehearsal

1. Extract the entire Windows x64 ZIP to a local folder; keep Assets, Notices, examples and docs together. Launch JudoCeremony.exe.
2. Open the supplied sample tournament or enter the real tournament name once. Select each actual category and delegation; resolve every reference reminder or unsupported delegation.
3. On Ceremony display, choose the HDMI monitor, load the prepared ceremony, and check the nine visibility options. Compare both flag orientations and the recap with the approved podium list.
4. Rehearse Play, Pause/Resume, Restart, Black screen/Restore and Reset. Rehearse no-gold and reduced-medal cases if applicable. Confirm that preparing the next category does not replace the loaded ceremony.
5. Paste a staff image into the chosen Windows app and inspect it. Test reconnecting HDMI on the actual event computer. Keep a backup of the .judo.json setup.

## Evidence and reproducibility

[Full visual report](audit/Release-Audit.pdf), [510-view comparison CSV](audit/flag-comparison.csv), [source picture/hash evidence](audit/flag-evidence.json), [software check result](audit/software-checks.txt), and [native package checks](audit/package-checks.json).

[IJF April 2026 manual](https://78884ca60822a34fb0e6-082b8fd5551e97bc65e327988b444396.ssl.cf3.rackcdn.com/up/2026/04/IJF_Flag_Manual_-_01_04_2026_--1776074839.pdf); current listing: https://www.ijf.org/documents . Source SHA-256: `411186e50c34b433f72bf56fb24e61604149cfe8a51caf0c5757db8aea5a607d`.

Original workbook: FlagChecking_v1.5e.xlsm. SHA-256: `55532532434054311d6346a4b9ddeb0daa0a300c1f57742d1e592a7f44542046`. Original workbook unchanged; workbook/macros and full manual pages are not shipped.

The comparison normalizes horizontal pictures to 144x96 and vertical pictures to 96x144, excludes a 0.6% raster border and measures mean absolute RGB error against a white background. Close <= 0.04; review <= 0.10; material > 0.10. Native aspect ratios, alternate rotations/reflections, source names, hashes and image dimensions are recorded separately. This method may overlook small details; final artwork follows the declared source policy, with visual review as additional evidence.

Use scripts/audit-excel-flags.py, scripts/import-audited-flags.py and scripts/create-release-audit.py as documented in README.md. Baseline comparison reproduces the v0.6 asset choices; after comparison uses the v0.7 runtime asset selection.
