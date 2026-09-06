What finance-service is for

Student-org finance usually dies in a group chat. Someone bought decorations. Someone else has the DJ invoice on their camera roll. The treasurer’s spreadsheet is already the official budget — and nobody wants to open it from a phone at midnight after Diwali.

This service keeps that spreadsheet as the source of truth, and makes it usable from the club’s existing assistant (sms-agent): list what’s on the books, see what a night cost, and file a receipt photo against the right line item — without anyone copying numbers by hand or rewriting planned vs actual.

The problem it solves

Clubs already live in one Google Sheet: events down the page, line items under each header, planned and actual in the columns next to them. That file is what exec and OSIL care about.

What the sheet does not do well is the messy middle:





“What’s left on Garba?” while you’re in Instagram DMs



Matching a photo of a Target run to Food, not the whole event



Proving a purchase happened without dumping images into a Drive folder named receipts FINAL v3

Officers should not need Editor access, a laptop, or to remember the tab named reciepts. They should send a picture and get a link that lands on the right row.

What it actually does

Knows the year at a glance. It reads the live actual tab and returns every event the sheet already has — Involvement Fair through merch — in the order the treasurer laid out. No second calendar. If it’s on the budget, it’s in the list.

Zooms into one event. Ask for Diwali and you get DJ, decor, and the rest, with planned, actual, PR-submitted flag, and notes. Subtotals and the grand TOTAL are skipped so you see purchases, not spreadsheet chrome. Ambiguous names (“Garba food”) resolve to the line item, not a guess at the whole night.

Files a receipt where finance can find it. A photo is stored in Google Drive and a row is appended on the receipts tab: event, line item, clickable Drive link, timestamp, filename. Treasurers reconcile from the sheet they already audit. The budget numbers on actual are never overwritten — attaching a receipt is evidence, not a rewrite of what was spent.

Keeps NJIT in the org. Receipts are visible to people signed in as @njit.edu (the same “NJ Institute of Technology” share you’d pick in Drive). They are not posted for the open internet. The club’s Workspace rules stay intact; the assistant still works.

Safe for concurrent chaos. Two people dumping receipts at once don’t clobber each other. The sheet gets one append at a time.

Why this is useful in practice

The assistant is a finance tool, not a chatbot with a spreadsheet hobby. When someone says they have a receipt for Diwali DJ, the model isn’t inventing a budget — it’s calling this service, which is staring at the same cells the treasurer uses.

That means:





Faster close-out after events (photo in, row on the log, link for whoever does PRs)



Fewer “which Drive folder?” threads



The official budget stays canonical; automation is not a shadow ledger



Exec can answer “what’s on the books for Holi?” without exporting CSV

It does not replace judgment. It will not mark a line paid, change remaining, or invent an event that isn’t a header on actual. It makes the existing process reachable from the channel people already message.

How it fits the club

sms-agent exposes a finance tool: list events, list line items, upload a receipt. This repo is that tool’s backend. Google Sheets and Drive remain the systems of record; finance-service is the disciplined API in front of them — read the budget, prove the purchase, don’t touch the numbers.