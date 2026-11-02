# Privacy

This system only works if it knows true things about you: work rights, salary anchors, what you cannot do yet. That is exactly the data that should never be public.

- **Your copy stays private.** If you use GitHub, create your copy as a private repository. The public template is the empty system, not your filled version.
- **The live tracker stays local.** `tracker/job_search_tracker.csv` and `seen_jobs.json` are in `.gitignore` on purpose. They list everywhere you applied, when, and what came back.
- **No passwords, ever.** Not in the repo, not in chat with your agent, not in the profile. Use your agent's secure vault or your password manager.
- **Dates of birth and home addresses** belong in the facts sheet only if your market's forms regularly require them, and you can keep that block in a local file outside the repo instead. The profile template marks those fields optional for a reason.
- **Sharing a filled repo** with a coach or a friend means sharing your salary anchors and rejection history too. Export the parts you mean to share instead.
- **Review before you publish anything derived from this template.** Search your copy for your name, email, phone and salary figures before a repository changes visibility. One command does it: `grep -rn "your-name-or-email" .` with your own details filled in.
