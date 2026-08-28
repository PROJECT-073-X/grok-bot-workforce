---
name: icp-research-draft
description: Research accounts against the ICP, score fit, write email and LinkedIn drafts. Never send.
when-to-use: Weekday morning or on-demand account research for outbound. Stop if the list is empty. Stop before send.
---

# ICP research and draft

## Inputs

- The current account list named by the user (sheet, CRM view, or `/workspace/outbound/list.md`)
- The written ICP in `/workspace/outbound/icp.md`

## Steps

1. Open the named list. If it is missing, or it has no account rows (header only counts as empty), stop. Say the list is empty. Do not invent companies.
2. For each account: company site, one recent public page, one registry or news source if available.
3. Score fit: yes / no / unknown. Unknown if a required ICP field has no source, or if `icp.md` still has unfilled brackets.
4. For yes: one email draft and one LinkedIn draft in the account's language. No merge-field theatre. Name one specific fact with a link.
5. Write `/workspace/outbound/review-YYYY-MM-DD.md` and paste the table in this conversation.

## Output columns

account | fit | evidence links | email draft | linkedin draft | legal note

Legal note for DE/AT/CH: draft only; send needs a documented legal basis.

## Rules

- Do not send. Do not enroll a contact in a sequence. Do not open a compose window that submits. Do not send or enroll unless the user releases that exact action in this conversation.
- Do not invent companies, metrics, hires, or funding rounds. If you cannot link it, leave it out.
- Stale-data: if the list or ICP file is older than seven days, say so at the top and still run, unless the user told you to stop. An empty list is a stop, not a stale run.
