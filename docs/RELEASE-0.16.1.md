# Judo Ceremony Desk 0.16.1 — athlete names in preparation images only

Athlete names are now limited to the **Preparation staff image**, including **Copy image** and **Save PNG**. Enable **Image visibility… → Results table → Athlete names in table** to include them. Imported names, manual correction, category history and completed queue records remain available on the operator desk.

The ceremony page no longer has an athlete-name checkbox. Audience previews and HDMI output always omit names, including when an event saved by 0.16 had enabled them. Loading or saving that event clears its audience name setting while preserving the staff-image setting and all names. A rendering guard also prevents old enabled settings from drawing names on the audience screen.

The anthem beta notice remains on the ceremony operator page and anthem testing panel. Event files remain schema 8; names and existing events are retained. Files saved by this build require 0.16 or newer for schema support, and 0.16.1 or newer applies the preparation-only display restriction.

This correction is included in the 0.17 release.

The focused run passed **176 checks**, including old enabled settings, image-only name rendering, preserved athlete data, ordinary snapshot identity, queue completion, backups and the removed ceremony control. The Windows build completed with zero errors. Reports are in `artifacts/checks-0.16.1-focused`; native package results are in `artifacts/release-audit-0.16.1`.
