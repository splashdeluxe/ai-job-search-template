# /outcome

Goal: keep the tracker true, so no role is ever applied to twice or lost, and turn every rejection into feedback the search can learn from.

1. When a reply, rejection, invite or confirmation lands, match it to the tracker row by company and role.
2. Update: status, date, what the mail actually said (quote the reason if one is given), next step and its date.
3. Feedback ask, for every rejection (settings in /setup: on or off, auto-send or approve each, channels, reminder interval):
   - Set the record's feedback status: ASKED, SKIPPED, ANSWERED or BOUNCED.
   - First check what the rejection already says. If it already gives a specific reason (a named gap, or experience or evidence the chosen candidates had more of), do not ask again: that reason is the feedback. Set the status to ANSWERED, quote the reason in the record, and log the skip as feedback already given. Generic lines (a stronger field, other profiles matched more closely) and rejections with no reason are not feedback, the ask below still applies.
   - Where a replyable person or thread exists, send a short reply in that thread asking for the specific reason, in the owner's voice, passing `05-writing-check.md`. Address the person by first name only, and keep the register the process already used: if it ran on first names, stay there (in German that means du, never Sie). Template shape: thank them for the process, name one concrete thing from it, ask what would have made the application stronger, keep the door open in one line.
   - No-reply or automated senders get no mail. If a named recruiter from the process is known, queue the ask for them on LinkedIn instead.
   - One reminder after the owner's interval, then stop. Never argue with a rejection.
   - Log every send, skip, bounce and answer with its date and route.
   - When an answer arrives, record the stated reason in the record and in the rejection groups below.
4. Rejections: group the stated reasons over time (location and rights, fit, stronger field, no reason) and show the owner the pattern when it changes their sourcing. Recurring reasons become proposals (close a gap, add profile evidence, change a track weight, tighten a filter) for the owner to approve, never changes made silently. /upskill is where approved learning proposals land.
5. Move the company in or out of the one-per-week window and record any reapply limit the employer states.
6. File automated confirmations to Job Applications. Keep real person mail in the inbox.
