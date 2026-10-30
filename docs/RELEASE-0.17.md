# Judo Ceremony Desk 0.17 — social media exports

This preview adds a separate social poster editor on **Preparation → Social export…**. It starts without athlete photos, as requested, and supports flags, athlete names, the four medal entries and the two 5th/two 7th places.

## Create a poster

1. Prepare a category in the operator desk, then choose **Social export…**. Its medal countries, names, event title, background image and logos seed the editor. You can also open it before choosing a podium and enter or import the results there.
2. At the top of the editor, paste the IJF competition link and choose **Read IJF results**. Select a published category and choose **Use selected results** to fill all eight placings. Fetching alone keeps the current poster. Applying results keeps your chosen event title; a blank title uses the imported title.
3. Review or edit the place, three-letter country code and athlete name in each row. Supported places are **1, 2, 3, 5 and 7**, including ties. Empty unused rows are omitted. Unknown countries and invalid medal counts must be corrected before export; flags are never guessed. Unpublished or conflicting results cannot replace the poster.
4. Choose **Portrait · 1080 × 1350**, **Square · 1080 × 1080** or **Story · 1080 × 1920**. Use **Magenta**, **Navy** or **Teal**, edit the footer/hashtag, and optionally add a background image or logo. **Clear images** removes the poster's embedded background and logos without editing the event.
5. Use **Copy image** or **Save PNG…**. The preview and exported PNG use the selected format's exact pixel dimensions. **Include 5th and 7th places** controls the lower section. No-gold/two-silver and shorter podiums retain the entered medals without inventing a winner.

The layout places silver first, gold next, then the two bronzes, with lower placings below. It uses the app's horizontal flag artwork. Long names fit or use an ellipsis visually; the full text remains editable. No athlete photos are fetched or included.

## Save for offline reuse

**Save poster…** writes a separate `.judo-social.json` project containing results, titles, selected format, theme, optional source/fetch metadata and embedded background/logo images. **Open poster…** restores it without an IJF connection. Files are limited to 25 MB including branding.

Poster projects are separate from tournament files and event backups. They contain athlete names. Keep the poster project alongside your event backup when moving to another PC. It uses poster format 1 and requires the 0.17 app.

## Ceremony behavior

The editor does not apply results to Preparation, alter queue entries, select an anthem or change the loaded audience display. It inherits event artwork as a starting point; changes here belong to the poster. Fifth and seventh places remain outside the ceremony medal list.

The preparation-only athlete-name restriction from 0.16.1 remains active: the ceremony preview and HDMI output omit athlete names. Event files remain schema 8. This release includes the previously local 0.16.1 audience-name restriction.

## Verification

The focused social run passed **197 checks**, including all three PNG resolutions, top-eight parsing, delegation aliases, missing/invalid results, no-gold podiums, saved projects, visible link placement, failed fetch retention and independence from the event and loaded ceremony. Rendered posters and the editor were inspected.

The full regression passed **582 software checks**, including all 146 bundled recordings opening in the native Windows decoder. Build warnings concern the unavailable NuGet vulnerability-data feed; compilation completed with zero errors. The report is `artifacts/checks-0.17/verification.txt`.

A live IJF fetch returned **112 top-eight athlete results across 14 categories**. Reports are in `artifacts/checks-0.17-focused` and `artifacts/checks-0.17-live`. Rehearse venue HDMI and audio separately; poster export does not validate event equipment.

The self-contained Windows package passed native launch, empty startup, schema 8 migration, app icon, all 442 flag-reference hashes and all 146 anthem hashes. Its report is `artifacts/release-audit-0.17/package.json`.
