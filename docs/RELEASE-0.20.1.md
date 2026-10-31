# Judo Ceremony Desk 0.20.1 — automatic top-eight social results

**Update event** now refreshes remembered social posts automatically. There is no second **Use event results** step. When IJF publishes the full top eight, posts receive 1st, 2nd, both 3rd places, both 5th places and both 7th places.

The correction covers both causes of four-athlete posts: a selected preparation podium supplying only four medallists, and a remembered post taking precedence over the updated event snapshot. New posts now use the shared published results first. Existing posts keep their layout, dimensions, palette, branding, footer and custom heading while their athlete rows refresh.

An editor already open while an update completes refreshes too. The refreshed post is remembered and survives reopening/restarting. Failed, pending or conflicting published results do not invent missing athletes or replace a valid poster with unusable rows. A source with fewer than eight published results remains visibly incomplete; the preview shows its athlete count out of eight.

Close the older running copy and open `dist/JudoCeremony-0.20.1/JudoCeremony.exe`, or **Start Judo Ceremony.cmd**. Click **Update event**, then open **Create social post**. Check that **Include 5th and 7th places** is enabled when you want those places visible on the image.

Event files remain schema 9 (0.20 or newer); poster projects remain format 2. This is a local review build until explicitly published.
