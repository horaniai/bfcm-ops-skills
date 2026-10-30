# SMS Rules

- **Save SMS for time-sensitive moments**: early access, launch, a cart nudge inside 48 hours, last chance
- **Frequency**: one SMS per day at most on peak days, and roughly one SMS per flow within a 48-hour window. A peak day replaces the monthly allowance rather than adding to it — see the monthly caps in the `bfcm-schedule` and `bfcm-messaging` skills
- **Quiet hours**: hold promotional sends inside 8am–9pm recipient local time. This is a federal floor, not a suggestion: 47 CFR 64.1200(c)(1) bars telephone solicitations outside those hours in the recipient's timezone, and 64.1200(e) applies the same rule to text messages. Several states are stricter (Florida closes at 8pm) and some cap message frequency, so apply state law on top. In Klaviyo, campaign quiet hours can follow profile location, but flow quiet hours follow the phone number's area code
- **Consent**: confirm terms, privacy policy, and opt-in language are compliant. Carrier review is stricter at peak
- **Spend**: forecast SMS credit usage and enable auto-upgrade so sends don't stall mid-sale
- **Throughput**: plan for slow delivery at peak. Carriers cap messages per second per sending number, not per ESP — a standard toll-free number sends at roughly 3 messages/second, so a 300,000-message send takes many hours, not minutes. Schedule earlier in the day. Toll-free numbers have had unreliable MMS during past BFCM peaks, so check Klaviyo's current guidance and default to text-only on toll-free numbers
- **SMS form**: run an SMS-only sign-up form for known email subscribers (see `forms-and-flows.md`)

These rules assume US sending. For deeper compliance work, use the `bfcm-messaging` skill.
