---
name: renewal-leads
description: Find companies that use a competitor's product and are coming up for renewal, get the right people to contact, draft renewal-timed outreach, and push the list into the user's sales tools. Use when the user asks who uses a competitor and renews soon, for a competitor's customers, a displacement list, accounts to win from a vendor, renewal leads, or wants competitor customers sent to their contact-data, CRM or email outreach tools.
---

# Renewal leads from RivalPipe

RivalPipe knows which companies use which software vendors, when each started,
and when their contract likely renews. This skill turns that into a contact list
and outreach the user can run today, using the tools already connected to Claude.

## 1. Pin down the ask

From the user's message, get:
- the competitor vendor(s), by product name or website. Several are fine.
- the renewal window, default 90 days;
- filters if given: country (two-letter code), industry, company size;
- how many accounts they want (default 25).

Ask one short question only if the vendor is missing.

## 2. Pull the accounts (RivalPipe tools)

1. `find_vendors` with the vendor name to get its slug. If several match, pick
   the exact name; mention the others in one line.
2. `vendor_overview` for the headline: customers, how many renew in 30/90/180
   days, new accounts this week.
3. `vendor_customers` with `renewing_within_days` and any filters.

Every answer depends on the user's RivalPipe plan:
- **Free:** a 5-account sample from a month ago, renewal month only.
- **Signals:** every account, no dates.
- **Renewals:** exact renewal dates.

If the answer contains `what_you_are_missing`, tell the user plainly what it
says: how many more accounts match, how many renew soon, how many new accounts
appeared this week. Include the upgrade link it gives, once. Never invent
accounts or dates to fill a gap.

## 3. Find the people (the user's own tools)

Look at the other tools connected in this session and use the first that fits:
- **Contact-data tools** (people search or enrichment by company domain and
  job title).
- **The CRM:** existing contacts at those companies first. Avoid re-prospecting
  customers or open deals already in the CRM.

Choose titles from the competitor's category:
- incident management, monitoring, DevOps: VP Engineering, Head of SRE or
  Platform, Director of Infrastructure
- CRM, sales tools, marketing automation: CRO, VP Sales, RevOps, Marketing Ops
- identity, security: CISO, IT Director, Head of Security
- HR and payroll: CHRO, VP People, People Ops
- support and help desk: VP Customer Support, Head of CX
- otherwise: the leader of the team that would use the product, plus one
  operations or procurement owner.

Two or three people per company is plenty. If no contact tool is connected,
list the titles to look for and say which tools would fill them in.

## 4. Write the outreach

One short email per company (under 90 words):
- open on their situation, not the product: the renewal window coming up, or
  growth, or the use case;
- never claim to know their contract terms or price. Say "teams often review
  this around renewal", not "your contract ends on 14 March";
- one concrete reason to look now, one low-friction ask (a 15-minute
  comparison, a migration checklist);
- plain language, no hype.

## 5. Hand it off

Show a table: company, domain, industry, size, renewal (date or month, as the
plan allows), contacts, one-line angle.

Then offer the next step with the tools that are connected:
- **An email sequencing or campaign tool:** add the contacts to a campaign or
  sequence.
- **The CRM:** create or update the companies and contacts, with the renewal
  date on the company.
- **No tools:** give a CSV block they can import.

Always show what will be added and ask before adding anyone to a sequence,
creating CRM records or sending anything. Never send email on the user's behalf
without their explicit yes.

## Good habits

- Accounts with the nearest renewal come first; they are the most time-sensitive.
- If the user tracks the vendor in RivalPipe, they can export the full list
  from the app. Mention it when they want more than one answer can hold.
- Respect plan limits: when RivalPipe says the monthly questions are used up,
  say so and stop.
