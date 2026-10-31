# Judo Ceremony Desk 0.21.4 — compact header on wide screens

On a wide or maximized window, the timer, update timestamp and connection status now sit in the top row between the logo and action buttons. The header uses less vertical space.

Smaller windows keep two rows so all controls remain visible. The layout reserves room for custom seconds, the live countdown and connection labels, keeping normal state changes from repeatedly switching rows. Longer update text keeps its full tooltip.

The same timer remains accessible inside Changes. Rearranging the header does not change its settings, countdown, keyboard focus, requests or loaded audience ceremony.

These changes are included in the [v0.21.4 Preview](https://github.com/YOUNESMAAFI/judo-ceremony-releases/releases/tag/v0.21.4). Close an older copy, extract the complete Windows ZIP and open JudoCeremony.exe. Maximize the window for the single-row header.

The build passed 68 report/timer/layout checks, 31 event-update/workflow checks and 17 category-fetch/header checks. These suites overlap. Coverage includes 1040, 1400, 1720 and 1920 widths, custom seconds, live fetching text, aligned controls, preserved focus and existing timer/report behavior.
