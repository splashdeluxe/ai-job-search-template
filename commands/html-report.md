# /html-report

Goal: one offline file that shows the whole search, for owners who want the dashboard outside Muse or as a snapshot.

1. Read the same sources as the dashboard spec (`dashboard/DASHBOARD-SPEC.md`): tracker, shortlist, exclusions.
2. Render one self-contained HTML file: Today KPIs and funnel by track, Pipeline table, feedback coverage, and the world map view if the owner enabled it, under the same no-guessed-location rules.
3. Print the build date on the page and the chain of totals (tracked, submitted, placed, unplaced) wherever a map is shown.
4. Save it as `dashboard/report-YYYY-MM-DD.html`. It is a snapshot. It never overwrites the tracker, and it contains no data that is not in the sources.
