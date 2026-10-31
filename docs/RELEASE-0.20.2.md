# Judo Ceremony Desk 0.20.2 — clearer results navigation

The former **Results** button selected the results view; pressing it while that view was already selected did not fetch anything. It is now a real **Category results** tab alongside **Ceremony queue**, with the active tab clearly marked.

Use **Update event** in the top bar to fetch new information. The two view tabs switch between the saved category results and ceremony order. Switching views preserves the selected day and category and makes no network request.

Partial results show only the medals currently loaded. A single bronze entry is not treated as a full podium; missing medals or athlete places are never invented.

The automatic top-eight social-post update from 0.20.1 is retained. Event files remain schema 9, and poster files remain format 2.

Close the older running copy and open `dist/JudoCeremony-0.20.2/JudoCeremony.exe`, or **Start Judo Ceremony.cmd**. This is a local review build until explicitly published.
