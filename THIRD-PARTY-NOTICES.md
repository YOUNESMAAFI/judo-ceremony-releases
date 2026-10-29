# Asset sources and notices

## Country flags

Base national flag artwork is imported from [hampusborgos/country-flags](https://github.com/hampusborgos/country-flags), whose README identifies the national flag artwork as public domain and describes its Wikimedia Commons origins. The application bundles locally rendered PNGs. No flag download is needed at runtime.

The upstream flag-source README is the reference for the artwork's provenance. Source SVGs are rendered using `@napi-rs/canvas` only during development; that tool is not shipped with the application.

Country codes follow the IJF reference for the 205 covered catalog entries. Other entries use three-letter IOC codes where supplied by the country-code dataset, with ISO alpha-3 fallbacks for territories without an IOC entry. Kosovo uses KOS; the constituent British-country entries use ENG, SCO, WAL, and NIR. This catalog is not a list of eligibility for any particular event.

Both orientations use 205 country-specific flag illustrations from the [IJF Flag Reference Manual, April 2026](https://78884ca60822a34fb0e6-082b8fd5551e97bc65e327988b444396.ssl.cf3.rackcdn.com/up/2026/04/IJF_Flag_Manual_-_01_04_2026_--1776074839.pdf). Its copyright notice credits the International Judo Federation, 2024. Only the country flag illustrations are bundled; the manual's pages, prose, federation logos and layout are not redistributed. Attribution is retained here. The illustrations use the manual's event proportions and its available raster resolution. Chinese Taipei's horizontal event flag is also taken from this reference, replacing the generic Taiwan national flag.

Source page numbers, horizontal and vertical asset hashes, and 50 entries outside this manual's coverage are recorded in `Assets/vertical-reference.json`. Sixteen of those countries use the flag illustrations embedded in the supplied FlagChecking v1.5e workbook for both views; `Assets/excel-reference.json` records their original shape names, image hashes and the workbook hash. The workbook and its macros are not distributed. The remaining 34 entries use the base artwork and rotation fallback and are marked for organizer review in both modes. See `docs/RELEASE-AUDIT.md` for the full comparison, intentional reference differences and gaps. No IJF endorsement is implied.

## Country names and code mappings

Country names come from the flag catalog, with selected English display-name adjustments. IOC and ISO mappings are imported from [datasets/country-codes](https://github.com/datasets/country-codes). The upstream data package supplies its licensing and source details. Country data is bundled in `Assets/countries.json`.

## Continental-union membership and competition countries

Version 0.11 bundles a country-to-union snapshot from the official [IJF federation directory](https://www.ijf.org/countries), checked on 28 October 2026. `Assets/country-regions.json` records the five source URLs, source-page SHA-256 values, catalog identities and IJF code aliases. Other / unlisted is the remainder of this app's catalog, not a list of IJF membership. The data is used as a selection aid and does not establish competition eligibility.

When requested by the operator, the competition importer reads country codes and the title of the public IJF Nations page. It does not import athlete details, sign in or modify the IJF service. Imported country lists remain local to the saved event. See `docs/RELEASE-0.11.md` for sources, snapshot behavior and unmatched codes.

## Category definitions

Senior, junior, cadet and veterans weight-category definitions are checked against the [IJF Sport and Organisation Rules, 14 August 2026](https://www.ijf.org/ijf/documents/26), sections 2.2.1 and A1.4–A1.5. Veterans divisions M1–M9 and F1–F9 are included. Masters, open, and team labels are editable convenience presets. The medal order matches section 8.10 for a standard gold/silver/two-bronze ceremony. Organizers can adjust the catalog for their event; no federation endorsement is implied.

## Anthem recordings

The 0.10 offline library includes selected instrumental U.S. Navy Band performances documented on individual Wikimedia Commons file pages. Only sources whose individual file metadata identifies a public-domain Navy performance are selected. `Assets/Anthems/catalog.json` retains each country code, original file/page, performer, source license description and URL, audio URL, retrieval date and SHA-256. Some files use Commons' MP3 derivative; others are converted from the original using FFmpeg/libmp3lame at 192 kbit/s, without trimming or musical edits. Where a local conversion is made, the original file hash is also retained. For remaining tracks unavailable from the media host, the public-domain `open-assets-hub/national-anthems` mirror is used only when its original-file provenance matches the reviewed Commons file identity; `MirrorUrl` and `Acquisition` identify these files. The USA recording uses the original Navy source preserved by Internet Archive and linked on its Commons page.

The original file pages describe the performance and composition rights and their jurisdictions. This source metadata is retained as provenance, rather than a claim that every recording has been approved by IJF or the event organiser. Coverage, deliberate omissions and corrected country mappings are listed in `docs/ANTHEM-LIBRARY.md`. Organisers can replace any recording with their preferred MP3/WAV. Locally imported recordings remain the organiser's materials and are not uploaded or included in tournament exports.

Country candidates were discovered with the `open-assets-hub/national-anthems` index, but its country mappings are not accepted without review. The application uses an explicit reviewed mapping in `scripts/anthem-sources.json`. Incorrect USA/Hungary, Oman/Romania and Dominica/Dominican Republic mappings were corrected before inclusion. The UWW download pack is not bundled.

FFmpeg and imageio-ffmpeg are development-only conversion tools and are not shipped with the Windows application. Playback uses Windows WPF MediaPlayer and requires no downloaded codec library.

## Microsoft .NET runtime

Self-contained builds include Microsoft .NET and WPF components. Their license and third-party notices are included in the distribution when supplied by the .NET publish tooling. See [dotnet/runtime](https://github.com/dotnet/runtime) and [dotnet/wpf](https://github.com/dotnet/wpf).
