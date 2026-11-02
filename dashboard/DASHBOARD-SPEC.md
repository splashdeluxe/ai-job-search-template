# Dashboard spec

What the agent builds for the owner in Muse at the end of /setup, and refreshes after every briefing run. The same spec renders as `/html-report` for owners who want an offline file.

## Data sources

- `tracker/job_search_tracker.csv` - every application and its status. The system of record.
- `feeds/shortlist.json` - the latest ranked shortlist.
- `tracker/exclusions.txt` - dropped roles and why.

No number appears on the dashboard that is not in one of these files.

## Views

**Today**
- KPI strip: tracked, applied, interviews, rejections, follow ups due.
- Focus first: the three things that need the owner today (a reply owed, a follow up due, a shortlist decision waiting).
- Funnel by track: sourced, ranked, applied, replied, interview, rejected, per track.
- Feedback coverage: asks sent and answers received across all rejections, as a bar.

**Explore**
- The current shortlist as cards: company, role, track, fit, gap in one line, posting link.
- Sourcing counts per portal, from the latest /scrape.

**Pipeline**
- Every tracked application: company, role, status, fit, date applied, next step and its date.
- Rejections grouped by stated reason, matching the daily briefing's groups.

**World map (optional, owner chooses in /setup)**
- Countries shaded by application volume, count badge per country. Selecting a country lists its companies and their statuses.
- Location comes from the posting or the tracker record only.
- Work model split: on site, hybrid, remote worldwide, remote one country, remote one region.
- Remote and multi-country roles form their own category. Roles with no recorded location form a "location not recorded" category. Neither is pinned to a guessed country.
- Reconciliation: the map total must equal the pipeline's submitted total. The page states the chain (tracked, submitted, placed, unplaced) whenever a gap exists.

## Refresh rule

- Rebuild after every daily briefing run, and on demand when the owner asks.
- The dashboard shows the data as of its build time, printed on the page. It never presents stale numbers as live.
