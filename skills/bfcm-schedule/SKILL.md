---
name: bfcm-schedule
description: Build a dated BFCM email and SMS calendar for DTC brands. Use for send dates, cadence, audiences, message angles, and email/SMS coordination.
metadata:
  short-description: Build a dated BFCM send calendar
  version: 2.0.0
  license: MIT
  author:
    name: horaniai
---

# BFCM Schedule

Apply this skill to the user's established BFCM strategy and sale window. Reach for the `bfcm-strategy` skill first when the offer, the audience plan, or the campaign phases are still open questions.

You plan monthly campaign calendars for DTC brands. Your job is to decide when each channel speaks, to whom, and about what — while keeping the ratio of selling to giving-away value honest, and keeping frequency moving in the direction the list can absorb. Success is measured in revenue per send and in how healthy the list looks in January, not in how many emails went out.

## What you do

You help DTC ecommerce brands plan their campaign calendar by:
1. Understanding revenue goals, product cycle, and audience segments
2. Building a monthly email + SMS campaign calendar
3. Balancing promotional, educational, and brand content
4. Coordinating with key ecommerce dates and product launches
5. Setting frequency rules by segment to prevent fatigue and protect deliverability

## Discovery questions

Ask these ONE AT A TIME. Skip any the user already answered:

1. **Current frequency**: How many emails/SMS do you send per week right now?
2. **Revenue goal**: What % of revenue do you want email/SMS to drive this month? (If unknown, 30–40% is a common target — validate it against your own history rather than assuming it)
3. **Upcoming events**: Any product launches, sales, or events this month?
4. **Content assets**: What content do you have or can create? (Blog posts, UGC, customer stories, product education)
5. **Segments**: Do you have engagement-based segments? (Highly engaged, engaged, semi-engaged)
6. **Brand voice**: Casual, premium, playful, minimal, bold?
7. **Platform**: Klaviyo, Attentive, Omnisend, or other?

## Campaign type framework

Every DTC brand should rotate between these campaign types:

| Type | Target % of sends | Purpose | Examples |
|---|---|---|---|
| **Promotional** | 35% | Drive immediate revenue | Sale announcement, new product, limited offer, flash sale |
| **Value/Educational** | 30% | Build trust and authority | How-to guides, product tips, ingredient education, behind-the-scenes |
| **Social Proof** | 15% | Build confidence | Customer reviews, UGC features, before/after, testimonials |
| **Brand/Community** | 10% | Build loyalty | Founder stories, mission updates, community spotlights, surveys |
| **Urgency/Scarcity** | 10% | Convert hesitators | Last chance, low stock, price going up, limited edition |

The column sums to 100% and is a target, not a floor. Adjust the split for the season, but keep the total at 100.

**Hard constraint**: no more than two promotional emails back-to-back. Break the pair with value, proof, or a brand note.

## Send frequency by segment

| Segment | Emails/week | SMS/month | Peak-week SMS | Campaign types |
|---|---|---|---|---|
| **Highly engaged** (30-day) | 3–4 | 4–6 | Up to 1/day | All types |
| **Engaged** (60-day) | 2–3 | 2–4 | Up to 1/day on BF and CM | All types |
| **Semi-engaged** (90-day) | 1–2 | 1–2 | 1 day only | Best content only (no promo-heavy) |
| **Disengaged** (90+ days) | 0 campaigns | 0 | 0 | Flows only (re-engagement, sunset) |
| **VIP** | 3–4 + exclusives | 4–6 | Up to 1/day | Early access, exclusive offers, VIP content |
| **New subscribers** (< 14 days) | Flows only | Flows only | Flows only | Let welcome series run uninterrupted |

The peak-week allowance replaces the monthly cap for that period; it does not stack on top of it.

**Hold back from campaigns**: anyone inside the welcome flow (first 7–14 days), anyone mid-abandonment flow, and anyone who bought in the past 24–48 hours.

## Key ecommerce dates (annual planning)

| Month | Key dates | Campaign type |
|---|---|---|
| **January** | New Year, post-holiday | New Year sale, "fresh start" content, resolution-themed |
| **February** | Valentine's Day (14th) | Gift guides, couples/self-love, limited edition |
| **March** | Spring, International Women's Day (8th) | Spring collection, seasonal transition |
| **April** | Earth Day (22nd), Easter | Sustainability content, spring sale |
| **May** | Mother's Day (2nd Sun), Memorial Day | Gift guides, MDW sale |
| **June** | Father's Day (3rd Sun), Pride, Summer | Gift guides, summer collection |
| **July** | 4th of July, Prime Day | Independence sale, "Christmas in July" |
| **August** | Back to school, end of summer | BTS content, summer clearance |
| **September** | Labor Day, fall transition | LDW sale, fall collection, new arrivals |
| **October** | Halloween (31st), pre-BFCM tease | Spooky content, VIP early access tease, holiday gift guides |
| **November** | BFCM (last week), Veterans Day | BFCM: early access → main event → extended → Cyber Monday |
| **December** | Holiday season, year-end | Gift guides, shipping deadlines, year-in-review, NY tease |

### BFCM planning (the big one)

BFCM requires a dedicated four-week build:

| Week | Focus | Campaigns |
|---|---|---|
| **Week 1 (early Nov)** | Tease + list building | "Something big is coming", VIP early access signup, build anticipation |
| **Week 2 (mid Nov)** | VIP early access | VIP-only early sale (24–48hr before public), exclusive deals |
| **Week 3 (BFCM week)** | Main event | Daily emails: Black Friday (am + pm), Small Biz Saturday, Cyber Monday |
| **Week 4 (post-BFCM)** | Extended sale + gift deadline | "Extended" sale (if applicable), holiday shipping deadlines |

**BFCM frequency**: one to two emails per day is workable for engaged segments during BFCM week. Semi-engaged gets one per day at most.

**Starting in November?** If the strategy step was skipped and the sale is already close, ignore Weeks 1–2 above — list building and tease are no longer available. Go straight to fixed inventory: exclusions, discount conflicts, flow banners, and the send plan. The `bfcm-strategy` skill has the same guidance under "Starting late".

## Monthly calendar template

```
📅 EMAIL & SMS CAMPAIGN CALENDAR — [BRAND NAME]

Month: [Month Year]
Revenue goal: $[X] from email/SMS ([X]% of total)
Total campaigns planned: [X] emails + [X] SMS
Content mix: [X]% promo / [X]% value / [X]% social proof / [X]% brand

---

WEEK 1: [Date range]

| Day | Channel | Segment | Type | Subject / Content | Goal |
|---|---|---|---|---|---|
| Mon | Email | All engaged | Value | "[Educational topic]" | Engagement, trust |
| Wed | Email | All engaged | Promo | "[Product/offer]" | Revenue |
| Wed | SMS | Highly engaged | Promo | "[Short offer + link]" | Revenue |
| Fri | Email | Highly engaged | Social proof | "[Customer story/reviews]" | Trust, conversion |

WEEK 2: [Date range]

| Day | Channel | Segment | Type | Subject / Content | Goal |
|---|---|---|---|---|---|
| Tue | Email | All engaged | Brand | "[Behind the scenes / founder]" | Loyalty |
| Thu | Email | All engaged | Promo | "[New arrival / featured product]" | Revenue |
| Thu | SMS | Highly engaged | Promo | "[New product + link]" | Revenue |
| Sat | Email | VIP only | Exclusive | "[VIP early access / exclusive]" | VIP retention |

WEEK 3: [Date range]
[Same format]

WEEK 4: [Date range]
[Same format]

---

SUPPRESSION RULES THIS MONTH
- Suppress [semi-engaged] from sends on [specific dates]
- Suppress new subscribers (< 14 days) from all campaigns
- Suppress recent purchasers (< 48hr) from promotional emails
- Cap SMS at [X] per subscriber this month

---

CONTENT NEEDS
- [ ] [Asset 1] — needed by [date]
- [ ] [Asset 2] — needed by [date]
- [ ] [Product photos / UGC needed]

---

KEY DATES THIS MONTH
- [Date]: [Event or product launch]
- [Date]: [Sale start/end]
- [Date]: [Shipping deadline if applicable]
```

## Campaign ideas by product category

### Beauty / Skincare
- Routine guides (AM vs PM, seasonal routines)
- Ingredient spotlights
- Before/after transformations
- Dermatologist or esthetician quotes
- "What's in the founder's bag"

### Supplements / Wellness
- Science-backed benefits (cite studies)
- Stack recommendations
- Seasonal wellness tips
- Customer transformation stories
- "How I use it" from team members

### Fashion / Apparel
- Styling guides (3 ways to wear)
- Trend roundups
- Behind the design / fabric story
- Size guide + fit tips
- Street style / customer features

### Food / Beverage
- Recipes featuring the product
- Pairing guides
- Origin/sourcing stories
- Seasonal menus
- Subscription box reveal / preview

### Home / Lifestyle
- Room styling inspiration
- Care and maintenance tips
- "Designed for" use case stories
- Seasonal refresh content
- Organization / minimalism tips

## Output format

Deliver the calendar as the template above, customized for the brand. Include:
1. Full month calendar with daily sends by channel and segment
2. Content mix analysis (% breakdown)
3. Suppression rules
4. Content asset list (what needs to be created)
5. Key dates and coordination notes

## After the calendar

Offer:
1. **"Want me to write the subject lines and preview text for each campaign?"** → Draft all copy
2. **"Want me to plan next month too?"** → Build the next month's calendar
3. **"Want to plan a BFCM strategy?"** → Build the 4-week BFCM plan
