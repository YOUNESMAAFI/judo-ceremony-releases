# Judo Ceremony Desk 0.18 — social export layouts

Open **Preparation → Social export…** and choose a layout above the preview. All four work with portrait **1080 × 1350**, square **1080 × 1080** and story **1080 × 1920** exports, every palette, event artwork, custom background/logo images and the optional fifth/seventh-place section.

| Layout | Design |
| --- | --- |
| Podium cards | The original raised medal cards: silver, gold, then the two bronzes. |
| Compact results | A ranked list with places, flags, athlete names and country codes. |
| Flag grid | Medal tiles arranged in two columns, with lower places below. |
| Winner spotlight | A large gold-medallist panel and a list of the remaining results. |

Choosing a layout updates the preview and the image used by **Copy image** and **Save PNG**. It preserves results, selected format, theme, branding, footer and source metadata. Reading and applying IJF results preserves the chosen layout. The editor remains separate from event preparation, queue entries, anthems and the loaded ceremony.

Winner spotlight uses the actual gold medal only. A no-gold podium shows **NO GOLD AWARDED** and its medal results instead of selecting an athlete as winner. Two silvers, shorter podiums and long names are supported. Athlete photos remain outside this version.

## Saved posters

Layout selection is saved in `.judo-social.json` projects using **poster format 2**. The 0.18 app opens existing format-1 projects in **Podium cards**, preserving the original design. Saving a poster upgrades it to format 2; **0.18 or newer** is needed to reopen that saved poster. Version 0.17 rejects the newer format rather than silently losing its layout choice.

Event files remain schema 8 and the audience output continues to omit athlete names. The public download remains 0.17 until this local build is explicitly published.

## Verification

The focused social run passed **255 checks**, including all 12 layout/format combinations and saved PNG decoding, distinct designs, no-gold cases, short podiums, long names, lower-place visibility, layout persistence, older project migration, future-version file protection, editor selection and imported-result retention. Visual checks include portrait, square and story layouts and the no-gold spotlight. Reports and PNG examples are under `artifacts/checks-0.18-focused`.

The native Windows package passed launch, empty startup, schema 8 migration, embedded icon, all 442 flag-reference hashes and all 146 anthem hashes. Its report is `artifacts/release-audit-0.18/package.json`. Build warnings concern an unavailable NuGet vulnerability-data feed; compilation completed with zero errors.
