# Judo Ceremony Desk 0.21.3 — timer inside Changes

Open **Changes** beside Update event. Its first section now contains the Auto-refresh checkbox, interval selector, custom seconds and live countdown. The controls remain available in the top bar as well.

Both locations operate one shared timer. Starting, stopping or changing the interval in either location updates the other. The timer remains available while its settings or report selector have keyboard focus; event input editing still defers automatic application.

Connect an IJF event first. Then check Auto-refresh and choose 2, 5, 10 or 30 seconds; 1, 2 or 5 minutes; or Custom for 2–3600 seconds. The timer starts off each session. Requests never overlap and updates do not load or start an audience ceremony.

The empty Changes dropdown fix from 0.21.2 remains included. Event schema 9, social-poster formats, flag artwork and anthem recordings are unchanged.

All 56 focused report/timer checks passed, including controls in the open Changes panel, shared state, custom seconds, keyboard focus, header geometry, countdown operation, failure retention and event switching.

These changes are included in the [v0.21.4 Preview](https://github.com/YOUNESMAAFI/judo-ceremony-releases/releases/tag/v0.21.4). Close an older copy, extract the complete Windows ZIP and open JudoCeremony.exe. Maximize the window for the single-row header.
