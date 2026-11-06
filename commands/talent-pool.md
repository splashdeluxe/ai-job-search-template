# /talent-pool

Goal: join talent pools cheaply and keep them tracked, so a pool turns into a real application when a live seat opens. A pool join is not an application. All standing rules in `AGENTS.md` apply unless this file says otherwise.

## What counts as a pool
- The posting says career pool, talent pool, talent community, speculative application, or the German Initiativbewerbung.
- There is no single seated role: no named client, team or start date, just future projects or future openings.
- If a posting has a real seat, it is not a pool. Run `/apply` instead.

## Detect
- During `/scrape` and `/rank`, tag pool postings POOL and list them separately from ranked roles.
- Pools skip fit ranking against a JD. There is no real JD to score against.

## Qualify (three checks, nothing more)
1. Engagement type is truthful for the owner: the contract form the posting states (freelance, fixed term, permanent) is one the owner accepts, per `01-candidate-profile.md`.
2. Geography is truthful: the owner could actually work the engagement from a base in the facts sheet, or relocate to it.
3. The field and level roughly match one of the owner's tracks in `00-tracks.md`.

A pool that fails a check is dropped with a one line reason in `tracker/exclusions.txt`, like any other role.

## Join
1. Reopen the live posting. Confirm it is still open.
2. Duplicate check: the pool register and the tracker. Never join the same pool twice.
3. Accounts: many pool platforms hide the form behind a sign-in (JOIN does). Create the account once, with the owner's approval, save the login in the owner's password manager, and reuse it for every pool on that platform. Note the platform in the register.
4. Form check, adapted: pool forms often start with a CV upload and only show later steps after it. Upload the pool CV (step 5), then read every later step before submitting. A required field with no truthful answer still drops the pool.
5. Pool CV: one variant per track, built to `03-cv-standard.md` with a consultant or generalist headline for that track. Reuse it for every pool in the track. Refresh it monthly, or when the record changes. Do not build a per-company CV for a pool.
6. Answers come from the pool block in `02-master-facts-sheet.md` (day rate band, contract types, availability). Research a missing figure once, show the owner the figure and basis, then store it in the pool block so the next pool does not stall on the same question.
7. Submit once. Record the confirmation wording in the register.

## Track
- One row per pool in the pool register (`tracker/pool-register-template.csv`, copied to `tracker/pool-register.csv` during setup): company, role, platform, date joined, engagement type, status.
- Pool joins never count in the application tally and never use the one-application-per-company-per-week slot. A later application to a live role at the same company is a normal application, not a duplicate.
- Status values: joined, invited, seat-live, closed, stale.

## Activate
- Check the register monthly: pool mail, platform messages, and the company board, looking for a live seat that matches.
- When a seat opens, run the normal `/apply` flow for it. The pool join is context, the application is new work.
- A pool with no signal for a quarter goes stale: close it in the register, or re-check it once and then close it.

## Worked shape (fictional)
A consultancy posts "Senior Product Manager / Consultant [Career Pool]", freelance, six month contracts, remote in the owner's country. Qualify passes. The platform needs an account, created once. The form starts with a CV upload, then asks availability, yearly compensation and language level, all covered by the pool block. One submit, one register row, status joined. Two months later the platform mails about a client project: status invited, and the live project goes through `/apply`.
