# /gmail-sync

Goal: turn mail signals into tracker truth, with the owner's approval on every change. Works with any connected mailbox; Gmail is the common case.

1. Read the tracker rows that are still open.
2. Search the mailbox for mail matching those companies and roles since the last sync: interview invites, assessment links, status updates, offers, rejections.
3. Propose updates, one per application: current status, what the mail says (quote the key line), proposed new status.
4. The owner approves or corrects each proposal. Nothing changes on a guess, and a mail about a different role at the same company is never merged in.
5. Apply approved updates through /outcome, including feedback asks for new rejections.
6. Report: matched, updated, unmatched mail that looked relevant but fit no tracker row.
