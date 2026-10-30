# Judo Ceremony Desk 0.18.1 — visible social editor entry

Use the teal **Create social post…** button in the main top bar, beside the version button. It stays visible on every workspace, so the editor can be opened without finding the smaller button below the preparation preview. **Preparation → Social export…** remains available as well.

The poster window shows **Podium cards**, **Compact results**, **Flag grid** and **Winner spotlight** above its preview. No prepared podium is required to open it; enter results or use the IJF link in the editor.

Open `dist/JudoCeremony-0.18.1/JudoCeremony.exe`, or use **Start Judo Ceremony.cmd** to select this newest local build. Check that the title/version button shows **v0.18.1**. The public download remains 0.17 until a newer release is explicitly published.

Focused checks verified the top-bar button at minimum window width on Preparation and Ceremony display, and clicking it opened the actual social editor. Existing layout, project persistence and event-independence checks passed. Reports and a screenshot are in `artifacts/checks-0.18.1-focused`. Event files remain schema 8 and saved poster projects remain format 2, requiring 0.18 or newer.
