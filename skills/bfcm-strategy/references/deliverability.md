# Deliverability Ramp

Inbox providers tighten their filters exactly when everyone sends more. The reliable way to land in spam is to point a daily cadence at a cold list.

## Technical check (do first)
- SPF, DKIM, and DMARC configured on a branded sending domain
- One-click unsubscribe in place and tested
- Gmail classifies a **bulk sender** as a From domain sending 5,000+ messages/day to Gmail accounts, transactional included. At that volume DMARC `p=none`, From-domain alignment, one-click unsubscribe, and a spam rate under 0.3% become mandatory. SPF **or** DKIM, valid PTR records, and TLS apply to every sender regardless of volume. Enforcement interrupts sending and there is no holiday carve-out
- Google Postmaster Tools connected if it isn't already

## Volume rules
- Step frequency up from October into November. Do not jump from 2–3 sends a week to daily in one move
- Ceiling to aim for: roughly 2x your normal cadence during BFCM week, and only if the ramp happened beforehand
- Route the additional volume to your most engaged subscribers before anyone else

## Engaged-first expansion
- Suppress anyone with no opens, clicks, or site activity in 180 days once they have received 15+ emails
- Begin with the 14 or 30-day engaged segment; widen to 60, then 90 days, only while engagement holds
- Keep the full list off the launch send. Hold the broadest send for the final day of the sale
- Opens are a weak signal now: Apple Mail Privacy Protection pre-loads tracking pixels, and Gmail's image proxying changes when a fetch is recorded, so a reported open is often not a human read. Judge health on clicks, conversions, unsubs, and spam complaints

For a full deliverability audit, use the `bfcm-inbox` skill.
