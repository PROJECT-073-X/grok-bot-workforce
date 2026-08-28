---
name: icp-research-draft
description: Research accounts against the ICP, score fit, write email and LinkedIn drafts. Send only after explicit release.
when-to-use: Weekday morning or on-demand account research for outbound. Stop if the list is empty. Do not send unless the user released that exact action.
---

# ICP research and draft

Grok Bot can send. This skill waits for release. Auto-review is the setting that enforces that if you leave it on.

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

Legal note for DE/AT/CH: send needs a documented legal basis. Auto-review on send is the setting.

## Rules

- Grok Bot can send. Do not send or enroll unless the user releases that exact action in this conversation. Do not open a compose window that submits.
- Do not invent companies, metrics, hires, or funding rounds. If you cannot link it, leave it out.
- Stale-data: if the list or ICP file is older than seven days, say so at the top and still run, unless the user told you to stop. An empty list is a stop, not a stale run.
