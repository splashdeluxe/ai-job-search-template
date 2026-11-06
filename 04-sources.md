# Sources

## Rules
- Official careers boards only for applying. Aggregators and reposts can be leads, never the submit route.
- A lead from anywhere gets verified on the employer's own board before it is ranked or applied to.
- Check name variants of excluded companies. A parent brand and its product brands count as the same company.

## Portals (starter set, adapted in /setup)

Remote boards: Himalayas, Remotive, Remote OK, We Work Remotely, Arbeitnow, Jobicy, Working Nomads.
Regional boards: Arbeitsagentur (Germany, public API), MyCareersFuture (Singapore), Jobstreet / SEEK (Singapore, Malaysia, Philippines, Indonesia — use the bare sg. / my. / ph. / id. hosts, the www. hosts serve the wrong market), Welcome to the Jungle, JustJoin.it, Landing.jobs (EU).
General boards: LinkedIn Jobs, Indeed, Glassdoor, StepStone.
Not usable as a feed: Glints — its search API ignores the search term outside a browser session, so it stays a manual look only.
Startup boards: Wellfound, Work at a Startup (YC).
ATS platforms (the company's own application pages): Greenhouse, Ashby, Lever, Workable, SmartRecruiters, Recruitee, Teamtailor, Personio, Breezy, Workday, SAP SuccessFactors.
Plus: the employer's own careers page, which is the source of truth for every role.

In /setup, add your local boards, your public job service and the niche boards of your field, and delete portals you do not use.

## ATS direct watchlist
- TODO in /setup: companies in your tracks on the ATS platforms above.
- Start with 20 to 30 companies you actually want. Grow it from /scrape results, not from guesses.

## Exclusions
- Live list: `tracker/exclusions.txt`
- Already applied (inside the one-per-week window), dropped by the owner, failed a hard gate, or a form with no truthful answer: all go in the exclusions with a one line reason and a date.
- A dropped role stays dropped until the owner reopens it.

## Talent pool platforms
Some platforms host career pools for many companies at once. One account per platform covers every pool on it.
- JOIN (join.com): company pools, form starts with a CV upload after an email sign-in.
- TODO in /setup: the pool platforms of your field.

Pools found anywhere still follow the rules above: verify on the employer's own page before joining.
