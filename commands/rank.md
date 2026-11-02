# /rank

Goal: a shortlist the owner can decide on in minutes.

1. For each surviving posting, run the eligibility gate and the language gate again on the full job description text. A failed gate is a drop with a one line reason, reported once.
2. Score the rest per track (see `00-tracks.md`). Best track wins, ties within 5 points are both shown.
3. Write `feeds/shortlist.json`: company, role, track, fit score, location verdict, posting URL, gap in one line.
4. Present in this shape: Brief, the wide set grouped by track, Converge with a real recommendation and the non-obvious pick marked, traps listed separately, Focus on the top items.
5. The owner decides per role: queue for /apply, fill the gap first, or drop. Drops go to the exclusions.
