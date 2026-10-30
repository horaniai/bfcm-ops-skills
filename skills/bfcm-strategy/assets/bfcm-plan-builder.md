# BFCM Plan Template Builder

Use this to build the one-page BFCM plan for a brand. Fill every section from the discovery answers and the reference files. Leave a field as `[TBD — owner]` if the answer isn't known yet and list it under Open Items. Don't invent numbers.

## Creative swap calendar

Site, forms, flows, and campaigns should change together. Fill one row per phase with a date and owner for every swap.

| Phase | Site banner | Popup + teaser | Flow banner (universal block) | Campaign header | SMS form | Date | Owner |
|---|---|---|---|---|---|---|---|
| **Teaser** | "Something's coming" | Early access signup | Early access | Teaser | Early access | | |
| **Early access** | VIP live | "Unlock early access" | Early access live | VIP | Early access | | |
| **Black Friday** | BF sale | Sale offer | BF | BF | Sale alerts | | |
| **Cyber Monday** | CM angle | CM offer | CM | CM | Sale alerts | | |
| **Last chance** | Ends tonight | Ends tonight | Last chance | Last chance | — | | |
| **Shipping cutoff** | Order by [date] | Gift / gift card | Shipping cutoff | Gift guide | — | | |
| **Revert** | Evergreen | Evergreen welcome | Evergreen | Evergreen | Evergreen | | |

## Plan template

```
BFCM PLAN — [BRAND]

Sale window: [dates] | VIP early access: [dates]
Offer: [offer] | Cyber Monday angle: [angle]
Baseline (last BFCM): RPR [$] | Click [%] | Revenue [$]

DELIVERABILITY RAMP
- Current cadence: [X/week] → Peak cadence: [X/week]
- Ramp: [week-by-week segment expansion]
- Auth status: [SPF / DKIM / DMARC]

SEGMENTS, TIERS + EXCLUSIONS
- [Segment]: [treatment]
- Send tiers: [which tiers get which sends]
- Excluded: [list]

FORMS + POPUPS
| Phase | Offer | Live from | Reverts |

FLOW CHANGES
| Flow | Logic change | Creative change | Live from | Reverts |

CREATIVE SWAP CALENDAR
| Phase | Site | Popup | Flow banner | Campaign | Date | Owner |

CAMPAIGN SENDS
| Date | Channel | Tier / segment | Message | Goal |

OFFERS
- [Offer structure, thresholds, loyalty, auto-apply links]

SMS
- Cap: [X/day] | Quiet hours: [window] | Number type: [type]

MONITORING TRIGGERS
- [Metric]: [threshold] → [action]

POST-BFCM + REVERT
- [Retention moves with dates]
- Revert date: [date]

OPEN ITEMS
1. [Item] — [owner]
```
