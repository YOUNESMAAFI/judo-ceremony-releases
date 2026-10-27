# Asset sources and notices

## Country flags

Base national flag artwork is imported from [hampusborgos/country-flags](https://github.com/hampusborgos/country-flags), whose README identifies the national flag artwork as public domain and describes its Wikimedia Commons origins. The application bundles locally rendered PNGs. No flag download is needed at runtime.

The upstream flag-source README is the reference for the artwork's provenance. Source SVGs are rendered using `@napi-rs/canvas` only during development; that tool is not shipped with the application.

Country codes follow the IJF reference for the 205 covered catalog entries. Other entries use three-letter IOC codes where supplied by the country-code dataset, with ISO alpha-3 fallbacks for territories without an IOC entry. Kosovo uses KOS; the constituent British-country entries use ENG, SCO, WAL, and NIR. This catalog is not a list of eligibility for any particular event.

Both orientations use 205 country-specific flag illustrations from the [IJF Flag Reference Manual, April 2026](https://78884ca60822a34fb0e6-082b8fd5551e97bc65e327988b444396.ssl.cf3.rackcdn.com/up/2026/04/IJF_Flag_Manual_-_01_04_2026_--1776074839.pdf). Its copyright notice credits the International Judo Federation, 2024. Only the country flag illustrations are bundled; the manual's pages, prose, federation logos and layout are not redistributed. Attribution is retained here. The illustrations use the manual's event proportions and its available raster resolution. Chinese Taipei's horizontal event flag is also taken from this reference, replacing the generic Taiwan national flag.

Source page numbers, horizontal and vertical asset hashes, and 50 entries outside this manual's coverage are recorded in `Assets/vertical-reference.json`. Sixteen of those countries use the flag illustrations embedded in the supplied FlagChecking v1.5e workbook for both views; `Assets/excel-reference.json` records their original shape names, image hashes and the workbook hash. The workbook and its macros are not distributed. The remaining 34 entries use the base artwork and rotation fallback and are marked for organizer review in both modes. See `docs/RELEASE-AUDIT.md` for the full comparison, intentional reference differences and gaps. No IJF endorsement is implied.

## Country names and code mappings

Country names come from the flag catalog, with selected English display-name adjustments. IOC and ISO mappings are imported from [datasets/country-codes](https://github.com/datasets/country-codes). The upstream data package supplies its licensing and source details. Country data is bundled in `Assets/countries.json`.

## Category presets

Senior, junior, cadet and veterans weight-category definitions are checked against the [IJF Sport and Organisation Rules, 14 August 2026](https://www.ijf.org/ijf/documents/26), sections 2.2.1 and A1.4–A1.5. Veterans divisions M1–M9 and F1–F9 are included. Masters, open, and team labels are editable convenience presets. The medal order matches section 8.10 for a standard gold/silver/two-bronze ceremony. Organizers can adjust the catalog for their event; no federation endorsement is implied.

## Microsoft .NET

Self-contained builds include Microsoft .NET and WPF components. Their license and third-party notices are included in the distribution when supplied by the .NET publish tooling. See [dotnet/runtime](https://github.com/dotnet/runtime) and [dotnet/wpf](https://github.com/dotnet/wpf).
