# Judo Ceremony Desk 0.21.1 — visible and custom refresh timer

Auto-refresh is directly in the top bar, with its checkbox, interval selector and countdown visible on every workspace. The Changes panel is reserved for reviewing the recent update reports.

Choose 2, 5, 10 or 30 seconds; 1, 2 or 5 minutes; or Custom to enter any whole number from 2 to 3600 seconds. Invalid custom values pause network requests and display the allowed range. The timer defaults to off and a one-minute interval each session.

The selected interval starts after a request completes. Slow requests do not overlap. Timer controls can keep keyboard focus without blocking refresh; typing in event inputs still defers automatic application. Event data, preparation and audience isolation follow the [0.21 update workflow](RELEASE-0.21.md).

Close an older running copy, extract the complete v0.21.1 Windows ZIP and open `JudoCeremony.exe`. Check that the version button says v0.21.1. The existing workspace launcher also selects the latest local build.

Event schema 9, poster formats and bundled flag/audio assets are unchanged.
