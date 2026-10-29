# Special medal layouts

Version 0.4 adds a Medal layout selector and a medal selector for each of four country entries. The same results drive preparation, staff PNG/clipboard output, the audience display and restart. Editing a prepared result never changes an already loaded ceremony.

## Available presets

| Preset | Awarded medals |
| --- | --- |
| Standard | Gold, silver, bronze A, bronze B |
| No gold - two silver | Silver A, silver B, bronze A, bronze B |
| One bronze | Gold, silver, one bronze |
| Gold and silver only | Gold, silver |
| Gold only | Gold |

The no-gold preset uses five hanging positions from the audience's left: silver A, silver B, an empty gold position, bronze A and bronze B. Only four flags are drawn. Both silver flags finish at the same silver height; the bronze flags finish at the same lower height. The five-position layout uses slightly smaller flags to keep every flag within the screen.

Reduced-medal presets are tools for entering approved results, not automatic decisions based on the number of entrants. For a missing bronze B, choose Not awarded on the fourth entry. For a missing bronze A, choose Not awarded on the third entry instead. The other awarded country remains in the result. Not awarded entries are hidden in exports and on the audience screen, and their country is not required. Their prepared country selection is retained so switching back does not erase it.

## Manual results

Each entry can be Gold, Silver, Bronze or Not awarded. Editing these selectors automatically identifies custom layouts. Use this for a missing silver, missing bronze medals, no gold with fewer bronze medals, or other official medal-withholding decisions. There must be at least one awarded medal and a selected country for every awarded entry. The editor supports at most one gold, two silvers and two bronzes within four awarded entries. It does not support multiple gold medals or more than four medallists.

Medals determine the hanging order and height. Within a tie, entry order determines A/B order; choosing the same country more than once is supported. A missing gold keeps its hanging position empty. No placeholder flag, medal label or country code is drawn there.

## Rule basis

Checked against the IJF Sport and Organisation Rules, version 14 August 2026, on 26 October 2026. [Official IJF documents](https://www.ijf.org/documents), [official SOR PDF](https://78884ca60822a34fb0e6-082b8fd5551e97bc65e327988b444396.ssl.cf3.rackcdn.com/up/2026/08/IJF_Sport_and_Organisation_Rul-1787430903.pdf).

- Section 8.10, page 98: the normal order is silver, gold, bronze A, bronze B. For the double hansoku-make final case, the order includes both silvers followed by an empty gold position and both bronzes.
- Article 18.3.1, page 194: an indirect double hansoku-make in the final gives both finalists second place. In a bronze contest both receive fifth place, so that contest produces no bronze medallist.
- Article 18.3.2, page 194: consequences of direct double hansoku-make are decided by the IJF Ad Hoc Commission. The app therefore provides manual medal entry and does not infer those consequences.
- Section 2.5, page 37: normal medal allocation has exceptions for low numbers. Use the result approved for the applicable competition system.

The app is a ceremony presentation tool. It does not adjudicate matches, recalculate brackets or promote another athlete when a medal is withheld.

## Saved tournaments

Earlier schema 1 files open with the standard layout when medal settings are absent. Version 0.4 saves schema 2 files, including the four medal assignments and any appearance settings. Earlier app versions reject these files instead of silently presenting an exceptional silver medal as gold. Keep a copy of an older tournament if you still need to use it with an earlier app.
