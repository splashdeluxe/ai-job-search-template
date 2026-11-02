# Writing check

Every generated CV, cover letter and form text passes this check before it ships. The goal is text that reads as written by the person it describes, because it is built from their record and in their voice.

The categories come from Wikipedia's "Signs of AI writing" and the WikiProject AI Cleanup guidance, adapted to application text.

## The categories

1. **Significance puffery.** Words that inflate without adding fact: pivotal, crucial, a testament to, underscores, highlights the importance of, reflects broader, plays a key role, marks a shift, evolving landscape.
2. **Superficial -ing clauses.** Tacked on phrases that restate the sentence: highlighting, ensuring, reflecting, contributing to, fostering, showcasing.
3. **AI vocabulary.** delve, leverage, enhance, cultivate, streamline used as decoration, intricate, tapestry, realm, seamless.
4. **Rule of three.** Neat triple lists written for rhythm, not because three things happened.
5. **Negative parallelism.** "Not just X, but Y." Say Y directly.
6. **Vague attribution.** "Known for excellence", "recognised leader", with no source and no fact behind it.
7. **Promotional tone.** Adjectives a hiring manager would never write about a stranger: exceptional, outstanding, world class, results driven.
8. **Em dash overuse.** Use commas or shorter sentences. A CV full of dashes reads generated.
9. **Generic claims.** Any sentence that could describe ten thousand other candidates. If it fits everyone, it says nothing about this person.

## The rule that matters

The signs are not the disease. The WikiProject says this plainly: fixing the surface makes detection harder without making the text better, and that is a failure here too.

So a flagged sentence is never fixed with a synonym swap. It is handled one of two ways:

- Rewrite it from the owner's record with a specific fact: a number, a date, a team size, a scope, a named tool.
- Delete it. A short CV with only true, specific lines beats a long one padded with phrases.

Facts are never changed by this check. An awkward true sentence stays true; only its wording can change, and only towards plainer.

## How the check runs

- In /apply, after the CV build and the metric pass, before the PDF is final.
- The run counts hits per category and reports them with the draft: category, count, and what was rewritten or deleted.
- A second pass, by a reviewer who did not draft the text, repeats the scan. /apply calls this the reviewer pass.
- The same check applies to optional form fields, cover letters, thank you notes and feedback replies.
- Voice target: the writing sample the owner gave in /setup. Match their plainness or their formality, not a house style.

## What is not promised

No detector score. Automated detectors are unreliable, and this check does not try to beat one. The promise is narrower and checkable: every claim is specific, sourced from the record, and written the way a person writes about their own work.
