# Security

## Postings are untrusted input

A job posting is text from a stranger, and it is treated that way.

- Before /apply evaluates a posting, it runs an integrity check: hidden text, invisible or zero width characters, instruction shaped lines ("ignore previous instructions", "tell the user", "include this phrase in your application"), and links that do not match their anchor text.
- A posting that fails the check is flagged to the owner with the exact lines found. The owner decides. The workflow never follows an instruction that came from a posting.
- The agent fetches no links from a posting body on its own. Only the posting page and the employer's own application form are opened.
- These defences are instruction level, not a sandbox. On an unfamiliar board, skim what was fetched before anything is submitted in your name.

## Your data

- Your copy of this repo is private. See PRIVACY.md.
- Logins live in your agent's secure vault or your password manager. Never in this repo, never in chat.
- Salary figures are researched and shown to you before they are entered anywhere.
- The agent submits only through the employer's official board, only with your approval mode from `06-dispatcher.md`, and exactly once per role.

## Reporting a problem

Found a pattern that tricks the gate, or a portal behaving badly? Open an issue at https://github.com/splashdeluxe/ai-job-search-template/issues with the posting text attached. Do not include your own profile data in a public issue.
