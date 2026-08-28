# Auto-review

Grok Bot can send, publish, and buy. These rules are how you decide when. Settings, General, Auto-review. Narrow is better than poetic.

## Require Approval

- Send or submit any email, LinkedIn message, SMS, or Slack message to an address or account that is not ours
- Publish a post, comment, or reply on X, LinkedIn, or a public site
- Create, edit, or delete a production record in the CRM except a draft note marked draft
- Purchase, place an order, or change billing
- Delete files, users, or campaigns
- Change production configuration, DNS, ads, or access
- Enroll a contact in a sequence or workflow

## Always Allow (only if you need them)

- Read mail, CRM, analytics, and calendars
- Write files under `/workspace`
- Draft in the Bot conversation

If both match, Require Approval wins.

## Description line to keep on every Bot

Grok Bot can send. Do not send, publish, purchase, or delete without explicit approval in this conversation.
