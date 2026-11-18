---
name: competitor-watch
description: A short briefing on what changed for the user's competitors in RivalPipe, with new customers, possible churn and renewals coming up, and what to do about it. Use when the user asks "what changed this week", "competitor update", "new customers of <vendor>", "who left <vendor>", "weekly competitor briefing", or "what's happening with my competitors".
---

# Competitor watch

1. `my_workspace`: get the tracked vendors and the plan. If nothing is tracked,
   ask which competitors to look at and use `find_vendors`.
2. For each competitor (at most 5):
   - `vendor_overview`: customers, renewals in the next 30 and 90 days, new
     accounts today and this week;
   - `vendor_signals` with `type: "new"`, then `type: "churn"`, since 7 days ago.
3. Write the briefing, one short block per competitor:
   - **New this week:** the count, plus up to 5 notable companies (biggest or
     best fit first). Free plans see counts only; say so once.
   - **Possible churn:** companies that stopped showing the vendor. Each is an
     opening to reach out.
   - **Renewing soon:** how many in 30 and 90 days, if the plan includes dates.
4. End with three concrete next steps, e.g. "Reach out to the 12 accounts
   renewing in 30 days", "Ask me for renewal leads for <vendor>" (the
   renewal-leads skill), "Push churned accounts to my CRM".

When an answer includes `what_you_are_missing`, pass on what it says, once, with
its link. Keep the whole briefing under 250 words unless the user asks for more.
