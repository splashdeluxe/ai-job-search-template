# ATS profile registry

Many application systems let a candidate keep a profile with the company, not just send one form. Teamtailor calls it Connect. JOIN keeps a candidate account. Workday keeps one account per company. A finished profile carries your CV, your consent to be considered for future roles, and job alerts for your function. Recruiters search these profiles when a new seat opens, so an application that only exists as a form submission is easy to miss later.

This file is the registry: what each system offers, what it asks for, and the answers you give. Fill in your own instances as you create them. Your personal answers live in `01-candidate-profile.md` and `02-master-facts-sheet.md`, not here.

## The workflow

1. During the form check in `/apply`, note whether the system, or the company's careers page, offers a candidate profile, a Connect or talent community signup, or job alerts. Write one line in the prep pack.
2. Apply first. Submit exactly once and record the confirmation, as usual. A profile never replaces the application, and creating one never triggers a second submit.
3. After the confirmed submit, create or complete the profile in the same run, with the standing answers below.
4. A profile counts as done only when its dashboard or settings page was seen: values, pitch, consents and alerts checked on screen. Record it in the profile register (step 6).
5. If a profile asks for something with no standing answer, ask the owner once, with a proposed answer. Store the answer in the facts sheet so the next profile does not stall on the same field.
6. Register: copy `tracker/profile-register-template.csv` to `tracker/profile-register.csv` and keep one row per company profile: company, system, date, email used, pitch used, alerts, consent state, status.

## Standing answers

| Field | Answer comes from |
|---|---|
| Name, email, phone, address | `01-candidate-profile.md` |
| Base, relocation, work rights | The facts sheet block for that geography, same answers as the application |
| LinkedIn, portfolio, GitHub | `01-candidate-profile.md` |
| Department or function | The closest match to the role you just applied for |
| Pitch | Written for this role, every time. Role words first, then your strongest matching evidence, then one hands-on example (public code or projects, if you have them). Respect the system's length limit (Teamtailor: 140 characters) |
| CV | The tailored CV built for this application |
| Privacy policy consent | Yes |
| Future job opportunities consent | Yes, always |
| Job alerts | Yes, for this company and this function |
| SMS or phone marketing | No, unless the owner says otherwise |
| Verification links and codes | The agent completes them when the owner has granted that standing permission in setup |
| Passwords | Never invented, never stored in this repo. Where a system forces a password, the owner sets it in their password manager once and the agent reuses that account |

## Per system

| System | What it offers | Login | What the profile asks for |
|---|---|---|---|
| Teamtailor | Connect profile, one per company | Email link, no password | Department, locations, phone, address, a short pitch, CV, job alerts, consents |
| JOIN | One candidate account for all companies on JOIN | Email verification | Profile and CV. Watch the default CV setting: an account can keep one CV as the default for later applications |
| Workday | One candidate account per company | Email and password | Profile, parsed CV, work history, job alerts for that company |
| SmartRecruiters | One candidate account across companies | Email sign-in | Profile fields, CV, job alerts |
| Recruitee | Talent pool signup on some company careers sites | Email form | CV, field of work, consent |
| softgarden | Candidate account | Email and password | Profile, CV, alerts |
| SuccessFactors | Candidate profile, one per company | Email and password | Full profile, CV, alerts |
| Personio | No candidate account | n/a | Form only. Some companies link a separate talent pool from the careers page; check the footer |
| Greenhouse | No candidate account | n/a | Form only. Some boards offer email job alerts; switch those on for your function |
| Ashby | No candidate account | n/a | Form only |
| Lever | No candidate account | n/a | Form only |
| Workable | No candidate profile for applicants | n/a | Form only. The confirmation mail carries your application link |
| Gem | No candidate account | n/a | Form only |

Systems not listed here: check the careers page during the form check, and add a row when a run settles what the system offers. Never guess a row into this table.

## Your instances

| Company | System | Date | Notes |
|---|---|---|---|
| TODO | TODO | TODO | One row per profile you create |
