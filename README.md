# Before They Renew, by RivalPipe

Ask Claude who uses your competitors and when they renew, then turn those
accounts into contacts and outreach with the tools you already use: your CRM,
contact data and email outreach. No switching between tools.

> "Which companies using my top competitor renew in the next 90 days? Find the
> engineering leaders and add them to my outreach campaign."

Free accounts get 50 questions a month with a sample of 5 accounts per
vendor. Paid plans get full lists, and Renewals adds exact renewal dates.
See https://rivalpipe.com/pricing/.

## Claude Code

```
/plugin marketplace add rivalpipe/before-they-renew
/plugin install before-they-renew@rivalpipe
```

The first time Claude uses RivalPipe it opens a sign-in page: sign in to
RivalPipe and click **Allow**. No API key needed.

## Claude.ai and Claude Desktop

1. **Connect RivalPipe:** Settings → Connectors → Add custom connector →
   name it `RivalPipe`, URL `https://app.rivalpipe.com/mcp` → Add → Connect,
   then sign in and click **Allow**.
2. **Add the skills:** Settings → Capabilities → Skills → Upload skill, once
   for each file: `renewal-leads.zip` and `competitor-watch.zip`
   (from https://rivalpipe.com/claude/).
3. In a chat, ask: *"Who uses my main competitor and renews in the next 60 days?"*

## What's inside

| | |
|---|---|
| `renewal-leads` | Competitor's customers renewing soon → contacts → renewal-timed emails → into your sales tools |
| `competitor-watch` | Weekly briefing: new customers, possible churn, renewals coming up |
| RivalPipe connector | `https://app.rivalpipe.com/mcp` (sign in with RivalPipe) |

Claude always asks before adding anyone to a campaign, creating CRM records
or sending anything.
