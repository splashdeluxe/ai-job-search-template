# Dispatcher

Status: TEMPLATE. /setup fills this file with the owner's choices and then creates the scheduled jobs in Muse. Nothing runs on a schedule before the owner has approved this file and seen one pilot application complete.

## Owner choices (filled in /setup)

- Timezone: TODO
- Morning shortlist time: TODO (default 08:30 local)
- Daily briefing time: TODO (default 08:30 local, can be the same run as the shortlist delivery)
- Dispatch interval: TODO (default every 5 hours) or "no automatic applying"
- Quiet hours: TODO (default 22:00 to 07:00, no deliveries, runs may still prepare)
- Approval mode: TODO, one of "blanket per batch" or "ask per role". Never assumed.

## The three jobs

1. **Dispatcher.** On the interval above: run /scrape, then /rank, then /apply for the roles the approval mode covers. Each application runs in its own chat. Submit exactly once per role. A run that finds nothing worth applying to ends quietly.
2. **Morning shortlist.** Daily at the shortlist time: the top ranked roles from the latest /rank, with fit, track, gap in one line, and a keep or drop call per role.
3. **Daily briefing.** Daily at the briefing time, covering yesterday in the owner's timezone: jobs found (verified on official boards, with form check drops counted), applied (confirmed submissions only, company and role; unconfirmed submits reported separately, never counted), rejections received, open applications with no reply from yesterday's cohort, and every rejection's stated reason grouped: location and rights, stated fit, stronger field, no reason given. One closing line: the pattern, if one is forming.

## Rules for every scheduled run

- All standing rules in AGENTS.md apply, including the integrity gate and submit exactly once.
- Reports go to the owner's main chat. Zero result days get one line, not a padded briefing.
- Token discipline: prefer text over screenshots, batch form fields, never re-read the whole tracker when a summary exists.
- The dashboard and, if enabled, the world map refresh after the briefing run.

## Stop rule

The owner says stop, in any chat, and every job in this file halts in the same turn. The agent reports what was done, what was not done, and what is mid-flight, and resumes nothing until the owner says go again.
