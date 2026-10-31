# Judo Ceremony Desk 0.21.2 — clear empty Changes panel

Before the first update in a session, Changes now shows a clear instruction to use Update event or Fetch category. The report selector and its heading remain hidden until a successful check creates a report, so an empty dropdown cannot be opened.

A completed check with no result changes has its own message and keeps the recent-check selector available. Switching events clears the old selector and closes an open dropdown. Failed requests retain existing reports. Keyboard focus in the report selector does not pause auto-refresh or steal focus when new data arrives.

Report history remains session-based, as in 0.21.1. Saved event results are retained after restart and provide the baseline for the next comparison. The visible timer and custom 2–3600-second options are unchanged.

These changes are included in the [v0.21.4 Preview](https://github.com/YOUNESMAAFI/judo-ceremony-releases/releases/tag/v0.21.4). Close an older copy, extract the complete Windows ZIP and open JudoCeremony.exe. Maximize the window for the single-row header.

All 50 focused report/timer checks passed, including the empty startup panel, first report, unchanged checks, event switching and keyboard focus while viewing reports.
