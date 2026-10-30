# Live Monitoring, Post-BFCM Retention, and Revert

## Live monitoring

Check daily during BFCM week and know in advance which numbers trigger a change. Decide the threshold before the sale, not while you're watching the dashboard:

| Metric | Action if it moves the wrong way |
|---|---|
| Revenue per recipient | Tighten segment, swap creative |
| Click rate | Shrink audience to a higher send tier |
| Unsubscribe rate | Cut frequency for that tier |
| Spam complaints | Stop expanding audience immediately |
| SMS opt-out rate | Cut SMS frequency |
| Form submit rate | Check the popup matches the site and the offer is clear |
| Support ticket volume | Check exclusions and flow messaging |

## Post-BFCM retention

What happens in the two to three weeks after BFCM decides whether the new buyers come back.

- **First-time BFCM buyer welcome**: separate post-purchase path for this cohort
- **Review requests** 7–10 days after delivery
- **Loyalty enrollment push** in early December for first-time buyers, framed around gifting
- **30-day read**: new customer conversion, repeat purchase rate, retention of BFCM cohort, email vs SMS contribution
- **List clean-up** in December using the engagement data BFCM generated

## Revert checklist (day after the sale ends)
- [ ] Every popup, teaser, and banner form back to evergreen
- [ ] Every flow banner and universal block back to evergreen
- [ ] Welcome discount path restored
- [ ] Abandonment flows back to normal delays and discount logic
- [ ] Smart Sending back on for flows
- [ ] Winback, price drop, and sunset flows back on
- [ ] No live links point to expired sale pages
- [ ] Expired codes disabled in Shopify

## BFCM postmortem and learning

Write the postmortem in two passes. The **48–72 hour read** captures execution lessons while they're fresh; the **30-day read** adds customer quality and retention. Compare against the plan, the prior BFCM period, and a normal non-promotional baseline where available. Label missing or directional data as such, and do not invent attribution or benchmarks.

### 48–72 hour read

| Area | Review | Decision it should inform |
|---|---|---|
| **Revenue** | Total revenue, email/SMS attributed revenue, revenue per recipient, AOV, conversion rate | Which sends, audiences, and offers should return next year |
| **Customer mix** | New vs repeat-buyer revenue, VIP revenue, first-time customer count | How much to prioritize acquisition, repeat buyers, and VIP early access |
| **Campaigns** | Revenue and clicks by send, segment, message angle, send time, and device | What to repeat, retire, or test |
| **Offers** | Redemption, AOV, units per order, gross margin where available | Whether tiers, bundles, GWP, loyalty, or a flat discount performed best |
| **Email health** | Clicks, unsubscribes, spam complaints, bounces, and engagement by send tier | Where frequency or audience expansion became too aggressive |
| **SMS** | Revenue per recipient, click rate, opt-out rate, delivery failures, and credit use | Which moments deserve SMS and which should remain email-only |
| **Flows and forms** | Flow revenue, abandonment recovery, welcome conversion, form submit rate, and SMS capture | Which automated changes materially contributed |
| **Operations** | Broken links, code failures, inventory issues, late swaps, support tickets | What needs an owner, QA step, or earlier deadline next year |

Platform-attributed revenue is not the same as incremental revenue. Without a holdout or another incrementality test, report attribution as directional.

### 30-day read

- First-time BFCM buyers who placed a second order
- Repeat purchase rate and time to second purchase for the BFCM cohort
- Refund, cancellation, and return rates by offer and customer type
- Contribution margin or gross margin after discounts, gifts, shipping, and returns when available
- List growth retained after unsubscribes and suppressions
- SMS subscriber growth retained after opt-outs
- Performance of the first-time-buyer post-purchase path

Compare the BFCM cohort with the prior year's BFCM cohort and a comparable non-BFCM acquisition cohort when the data exists.

### Postmortem output

```text
BFCM POSTMORTEM — [BRAND] — [YEAR]

OUTCOME VS PLAN
- Revenue: [actual] vs [plan] ([variance])
- Email/SMS attributed revenue: [actual] vs [plan]
- AOV: [actual] vs [baseline]
- New vs repeat-buyer revenue: [split]
- Margin: [actual or unavailable]

WHAT WORKED
1. [Finding] — [evidence] — Repeat: [action]

WHAT DID NOT
1. [Finding] — [evidence] — Change: [action]

CUSTOMER QUALITY — 30-DAY UPDATE
- Second-order rate: [result]
- Returns/refunds: [result]
- Cohort comparison: [result]

NEXT BFCM
- Repeat: [items]
- Stop: [items]
- Test: [items with hypothesis and success metric]
- Infrastructure fixes: [item — owner — due date]

OPEN DATA GAPS
- [Missing data and how to capture it next time]
```

Every recommendation should cite the result that supports it. Separate proven findings from hypotheses that need testing next year.
