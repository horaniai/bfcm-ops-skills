# Sign-up Forms, Popups, and Flows

Transactional emails are out of scope.

## Sign-up forms and popups

BFCM brings the year's highest-intent traffic. An evergreen popup spends it on the wrong offer. Forms should move with each phase and show what the site is showing.

### Swap the offer by phase

| Phase | Form offer |
|---|---|
| **Pre-sale (Oct – early access)** | "Get early access" to the BFCM sale instead of the standard welcome discount |
| **Early access live** | "Unlock early access now" |
| **Sale live** | The sale itself. Don't stack a welcome code on top of the sale unless that's deliberate |
| **Post-sale** | Revert to the evergreen welcome offer |

### Rules
- **Mirror the site.** Popup image, headline, colors, and offer name match the site's current hero and banner. The popup changes the same day the site does
- **Update the teaser too.** The teaser (the tab that appears after someone closes the form) should hint at the current offer
- **Schedule variants by date** with Klaviyo's form scheduler so swaps happen automatically and revert on time
- **Success page** links to the early access or sale collection, with UTMs on the link
- **Run an SMS-only form for known email subscribers** so they only see the phone number step
- **Hide forms** from existing subscribers, and never show them on cart or checkout
- **Optional banner form** for the sale announcement or shipping cutoffs
- **Keep forms and flows in sync.** Each form feeds the right list, and the welcome or early access flow delivers exactly what the form promised
- **Track submit rate** per variant. ~3%+ is a healthy popup benchmark

## Flows

Audit every flow that could fire during the sale. Flows carry more volume than campaigns at peak, and evergreen messaging that contradicts the live sale costs conversions.

### Logic
- **Cut abandonment delays.** Reduce cart and browse abandonment first-message delays to about 30 minutes for the sale window
- **Turn off Smart Sending on key flows** (welcome, abandoned cart, browse, post-purchase) during the sale window so they still fire alongside campaign sends. Keep Smart Sending on for campaigns
- **Use flow scheduling.** Build sale versions of flows, schedule them Live for the sale window, and schedule the evergreen versions back on after. No late-night manual switching
- **Fix discount conflicts first.** Any flow that hands out a code needs a decision: pause it, swap it, or route around it
- **Check sale cutoffs.** A delayed message can land after the sale ends and promise a discount that no longer exists. Add a date-based filter or split so nothing sends a dead offer

| Flow | Change for the sale window | Revert |
|---|---|---|
| **Welcome** | New signups go into a BFCM early access path instead of the standard welcome discount. Once the sale is live, swap in a BFCM banner pointing to the sale. Route everyone through the non-discount path | Bring the welcome discount back the day after the sale ends |
| **Abandoned cart** | 30-minute first send. Swap discount emails for no-discount versions that point to the sale | Day after cutoff |
| **Abandoned checkout** | Same as cart: no-discount versions pointing to the sale | Day after cutoff |
| **Browse abandonment** | 30-minute first send, sale messaging | Day after cutoff |
| **Price drop** | Set to Draft if the brand's sale uses price changes. Otherwise every sale item triggers it | Back on after the sale |
| **Post-purchase** | Shorten the upsell window while the sale is live ("people who bought this also picked up"). Tag first-time BFCM buyers into their own segment | Normal timing after the sale |
| **Winback** | Pause for the sale window. A winback discount on top of the sale trains people to wait | Day after cutoff |
| **Sunset** | Pause during ramp so you don't lose subscribers right before peak | Restart in December |

### Creative
- **Add a BFCM banner to every customer-facing flow** (welcome, cart, browse, checkout, post-purchase). Build it as a universal content block so one edit updates every flow at each phase change
- **Update subject lines and preview text** in abandonment flows to reference the sale
- **Remove copy that contradicts the sale**: "10% off your first order", old free-shipping thresholds, evergreen urgency lines
- **Check product blocks show the right price** for both code-based and price-change sales
- **Countdown timers only where the flow can't send after cutoff**
- **December swap**: shipping cutoff banner, gift wrap, and extended returns messaging in post-purchase

### QA checklist (October, not Black Friday morning)
- [ ] Filters and trigger logic correct on every live flow
- [ ] Discount codes apply (or are correctly removed)
- [ ] Smart Sending settings match the plan
- [ ] Flow schedules set with correct start/end times and timezone
- [ ] No message can send a dead offer after cutoff
- [ ] Banners and universal blocks show the right phase
- [ ] Test sends reviewed on mobile

For deeper abandonment flow builds or welcome flow redesigns, use a dedicated flow skill. That work sits outside this pack.
