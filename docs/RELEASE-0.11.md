# Judo Ceremony Desk 0.11 — country filters and IJF event import

Use the **Countries** button at the top of the operator desk, available from every tab. The active scope and visible-country count appear in its label. Filters apply to medal-country suggestions, the ceremony anthem country selector and the anthem testing library.

## Worldwide and continental unions

Choose **Worldwide**, **AJU · Africa**, **JUA · Asia**, **EJU · Europe**, **OJU · Oceania**, **PJC · Panamerica**, or **OTH · Other / unlisted**. Worldwide includes all 255 catalog entries. Union membership comes from an offline snapshot of the official IJF federation pages checked on 28 October 2026. Other / unlisted contains catalog entries not assigned by those five member lists; it is not a claim that they are IJF members.

| Scope | Catalog entries |
| --- | ---: |
| Worldwide | 255 |
| AJU | 54 |
| JUA | 43 |
| EJU | 51 |
| OJU | 20 |
| PJC | 37 |
| Other / unlisted | 50 |

This uses judo membership rather than geographic guesses. Israel and Türkiye are included in EJU; Kazakhstan is included in JUA. IJF aliases SGP, NFI and MNP map to the app's existing SIN, NFK and NMI catalog identities. The app continues to display its existing three-letter codes and flag artwork. Membership does not establish eligibility for a particular event.

## Competition country list

Select **Competition countries…** to edit a draft list. Search countries, filter the editor by region, check individual countries, or use **Add shown / Remove shown**. Changes reach the current event only with **Save changes**; Cancel keeps the existing list.

You can also paste three-letter codes separated by spaces, commas, semicolons or line breaks, for example `TJK FRA GER JPN`, and choose **Replace list with codes**. **Load code list (.txt / .csv)…** accepts a plain code list; CSV files should contain country codes only, with an optional Code/NOC header. Names and other text are rejected rather than guessed. Duplicate codes are combined and supported ISO/IJF aliases are resolved.

Enable **Only countries participating in this competition** in the Countries menu to restrict suggestions to that list. Region and participation filters combine: EJU plus a participant list shows the European-union members on that list. An empty enabled list shows zero choices instead of reverting to Worldwide. **Show all countries** removes both restrictions while preserving the saved participant list.

Changing filters never clears entered medal countries, replaces the loaded podium, changes flag positions or switches the loaded anthem. The menu identifies existing prepared medal countries outside the new scope. Selecting a new category still restores that category's own results as before.

## Import from IJF

Paste an official `https://www.ijf.org/competition/…` link into the participant editor and select **Import from IJF**. Competition overview, results, athlete and nation links are accepted; country/category query filters are removed so the app requests the complete **Nations** list. The importer reads the complete Nations list and the event overview. The preview shows the event name, location, start/end dates and published men’s and women’s weight categories. Choose **Apply event name, location and dates** and/or **Use imported categories**, edit the name or category group if needed, then **Save changes**. Uncheck those options for a country-only import. The imported source URL and time are retained. You can also open this editor with **Import IJF event…** below the tournament name. Imported dates and location appear there as an event summary; they are stored with the event without adding them to ceremony headings.

The editor previews the matched countries and any source codes absent from the flag catalog. Unmatched codes remain in the saved metadata for review and are never substituted with another flag. For example, the current Abu Dhabi fixture contains an IJF delegation code which has no catalog entry. Failed, incomplete, timed-out or cancelled nation downloads keep the editor’s previous list. If only the event overview fails, a warning explains that countries are available; applying event details defaults off so existing details are retained. The source page is read only; no login or account access is used.

Importing requires internet access. Saved participation lists and continental filters work offline. Imports are snapshots, so reimport when the organiser's entry list changes. The app does not continuously synchronize a live event's entries.

## Event history and compatibility

Each event keeps its own region, participation restriction, selected countries, event details and import provenance. Importing details updates the current event; start **New event** first when importing a different tournament. The category presets can be replaced by the imported list while saved category results, the selected category, entered medals and the loaded audience ceremony remain intact. Categories missing from the overview are kept as they are. Review the suggested category group before saving; Senior is the default unless the title identifies Junior or Cadet. Categories within that event share the competition list. A new event starts Worldwide with no participants; reopening a historical event restores its own settings.

Version 0.11 saves **schema 5** so older apps reject the new files instead of silently discarding participation settings. Schema 1–4 files still open, defaulting to Worldwide and no participant restriction. Audio, independent image/audience controls, categories and existing results are retained. Close older versions before launching this build.

## Sources and verification

The membership snapshot is in `Assets/country-regions.json`, with source URLs, original page SHA-256 values and code aliases. `scripts/update-country-regions.py` refreshes the snapshot for review. Sources: [AJU](https://www.ijf.org/countries/aju/members), [JUA](https://www.ijf.org/countries/jua/members), [EJU](https://www.ijf.org/countries/eju/members), [OJU](https://www.ijf.org/countries/oju/members), [PJC](https://www.ijf.org/countries/pjc/members).

Verification covers all region counts and special membership cases, filter intersections, empty lists, legacy migration, schema 5 exports and event history, code aliases, malformed/foreign links, redirects and incomplete responses, actual picker/library propagation, editor Save/Cancel, import failure and existing-result isolation. A live import of the completed Dushanbe competition returned all 19 nations, 14 weight categories, its location and 24–25 October 2026 dates. HTML fixtures retain public country codes, event facts and page structure without athlete data. Checks cover event preview, country-only opt-out, metadata persistence, category selection and audience/result isolation.
