# Judo Ceremony Desk 0.16 — athlete names and anthem beta warning

This preview adds optional athlete names to the results table and a visible beta notice on the ceremony page and anthem testing panel.

## Anthem notice

The ceremony page and **4 Anthem testing** now display:

> BETA FEATURE. We accept no responsibility for anthem accuracy or playback. Verify the recording with event officials before use.

The notice stays on the operator desk. It is not drawn on staff images or the audience screen. Anthem selection, separate/linked transport and existing playback guards continue to work as before.

## Import and review athlete names

Use the IJF competition link in **Import IJF medal results**, then **Read results**. The preview shows the published athlete beside each medal and country. Applying a category imports its names as well as its medal countries. Loading a full event and refreshing published results retains names in the final-block plan; preparing or loading a queued podium carries them into that ceremony.

On **Preparation**, expand **Athlete names · optional** below the medal countries to review, correct or enter the four names. New categories start blank. Returning to an entered category restores its own names. Changing one country clears that entry's name so a previous athlete is not attributed to another nation. Names are limited to 160 characters on one line. Missing names stay blank; names are never guessed from a country's other athletes.

Names are attached to individual medal rows. Two athletes from the same nation remain separate. Unresolved names do not prevent importing readable country results; conflicting duplicate results still require review.

## Choose where names appear

Names are **hidden by default**.

- **Preparation → Image visibility… → Athlete names in table** controls the staff preview, copied image and exported PNG.
- **Ceremony display → Audience screen visibility → Athlete names in table** controls the audience output independently.

Enable **Results table** for names to appear. They are an additional table column; flag labels retain their existing controls. With no fetched or entered name, the table uses a dash. Long names fit within the table and may be shortened visually with an ellipsis; the complete saved name remains available in Preparation.

Editing preparation does not rewrite the loaded ceremony. Reload the approved podium to present corrected names. Finished queue entries preserve the names actually loaded and presented, even if preparation or subsequently fetched results change.

## Event compatibility

Event files saved by this build use **schema 8**. They retain athlete names in preparation, saved categories, final-block medals and completed queue podiums, plus the separate image/audience visibility choices. Portable backups retain the same data.

Schema 1–7 events still open; missing name fields become blank and the two name visibility options start off. Events and backups saved by 0.16 require **0.16 or newer**. Older apps reject schema 8 instead of silently dropping athlete data.

Physical HDMI and venue-audio checks remain part of event rehearsal.

## Verification

The full regression passed **543 software checks**, including native decoding of all 146 bundled recordings. The focused athlete-name run passed **171 checks**, including repeated nations, Unicode names, missing/ambiguous names, per-category persistence, independent image/audience settings, immutable loaded/completed podiums, backups and schema migration. The beta warning leaves anthem transport, volume and sound testing visible at the normal board size.

A live IJF fetch of competition 3353 returned all **56 medal athlete names across 14 categories**. Rendered horizontal and vertical tables and the ceremony controls were inspected. Reports are under `artifacts/checks-0.16-final`, `artifacts/checks-0.16-focused` and `artifacts/checks-0.16-live`. Build warnings concern an unavailable NuGet vulnerability-data feed; compilation completed with zero errors.

The self-contained Windows package passed native launch, empty startup, schema 8 migration, embedded icon, all 442 flag-reference hashes and all 146 anthem hashes. Its report is `artifacts/release-audit-0.16/package.json`.
