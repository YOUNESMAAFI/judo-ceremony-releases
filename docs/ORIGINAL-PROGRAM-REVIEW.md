# Original FlagChecking v1.5e review

Inspected `FlagChecking_v1.5e.xlsm` from the user's `OneDrive/Desktop/Corina/FlagChecking` folder on 26 October 2026. The workbook was read as a ZIP/XML package, and VBA source was extracted for inspection. Excel and its macros were not executed; the source workbook was not changed or copied into this repository.

The workbook contains Flag Checker, Horizontal Printout, Vertical Printout, and Flags sheets. Its footer identifies v1.5e and the August 2025 IJF flag reference book. The VBA forms select countries and contest categories and generate horizontal or vertical static flag printouts from embedded worksheet images. One label supports an exceptional two-silver outcome. The new application added that outcome in version 0.4, along with reduced-medal presets and manual medal assignments; see `SPECIAL-MEDAL-LAYOUTS.md`.

No playback keyboard bindings or play/pause/restart handlers were found in the extracted VBA source. The new application's ceremony shortcuts therefore control its existing timed animation. They do not invoke the workbook or its macros. The new application continues to use its audited April 2026 vertical flag assets.

Version 0.3 adds shared shortcuts for the operator and audience windows, immediate restart of the loaded ceremony, background color/image controls, and top-left, top-right, and bottom-center logos. Images are embedded in tournament files. Prepared appearance changes are isolated from the active audience ceremony.
