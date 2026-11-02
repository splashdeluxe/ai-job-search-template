# /scrape

Goal: find new live roles that could fit, from official sources only.

1. Read the profile, tracks and exclusions first. If `seen_jobs.json` does not exist yet (first run on a fresh copy), create it as an empty list before anything else. It stays local, it is gitignored on purpose.
2. Sweep the remote boards in `04-sources.md` and the ATS watchlist companies' own careers pages.
3. For each hit, keep: company, role title, official posting URL, location as posted, date found.
4. Drop anything in `tracker/exclusions.txt`, anything already in `seen_jobs.json`, and anything that fails the eligibility or language gate on its face.
5. Add new finds to `seen_jobs.json` with the date. Save the job description text for the survivors, one file per role under `applications/`, so /rank and /interview work from the real text later.
6. Report counts only: found, dropped per reason, surviving. No padding to hit a number.
