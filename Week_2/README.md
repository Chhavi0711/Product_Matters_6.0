# Week 2 - TrustFix: Concept, Personas, MVP & GTM

**Product Matters 6.0 · E-Cell IIT Guwahati** - [back to programme overview](../README.md)

The assignment: design TrustFix, a trusted home-services marketplace, from a one-paragraph market problem - no existing product to critique this time, a 0-to-1 concept instead. This deck and its decisions are what [Week 3's prototype](../Week_3) builds directly on top of.

📄 **Brief:** [`Week_2_assignment.pdf`](./Week_2_assignment.pdf)
📄 **Submission:** [`ProductMatters6.0_Assignment2_Final.pdf`](./ProductMatters6.0_Assignment2_Final.pdf)

## The problem: a marketplace double-bind

Core message: TrustFix isn't just a discovery engine, it's trust infrastructure. The primary barrier to growth in home services isn't a shortage of professionals or customers - it's asymmetric information causing mutual anxiety on both sides.

- **Customer problems:** unsure whether a professional is genuine, no standard pricing, late arrivals, fake reviews, poor post-service support, hard to compare providers
- **Provider problems:** irregular work, difficult to build credibility, forced to compete on price alone, no long-term customer relationship

**Key insight:** customers don't struggle to *find* plumbers - they struggle to *trust* them. That becomes the product vision.

## Personas

**Riya Sharma** (the anxious customer) - 29, software engineer, Kanpur, mobile-first and highly digitally literate. Fears unverified people entering her apartment, anxiety over arbitrary post-service price hikes, wastes hours waiting for professionals who delay without notice. Needs: total pricing transparency, verified professional identity.

**Rajesh Kumar** (the stressed professional) - 38, electrician, Kanpur, 8 years' experience, low tech-fluency, relies on WhatsApp/calls. Depends on word-of-mouth, inconsistent income, no digital track record to justify premium rates. Needs: a simplistic, low-text interface to secure consistent local jobs without administrative overhead.

## Product vision: "Making Trust Measurable"

Unlike existing marketplaces, TrustFix helps users make confident booking decisions through transparency and accountability. Core principles: **Verified Professionals · Transparent Pricing · Real-time Tracking · Trust Score · Service Guarantee.**

## Proposed solution - three pillars

1. **The Predictable Pricing Engine** - standardized, upfront rate cards per task (e.g. "AC Cleaning – Base Rate ₹X"), eliminating haggling entirely
2. **Verified Credential Layer** - multi-step background check (identity + basic skill validation) surfaced via simple badges, building customer psychological safety
3. **Low-Friction Bridge** - an optimized customer booking flow paired with an ultra-simple one-tap accept/reject flow for professionals, built around low digital literacy

Core features: Trust Score™, government-verified professionals, transparent price estimates, live tracking, arrival guarantee, digital job card, before/after photos, easy rebooking.

## MVP prioritization (value vs. complexity)

Prioritized ruthlessly given limited engineering resources:

| Feature | Targeted user | MVP? | Why |
|---|---|---|---|
| Upfront Standardized Pricing | Customer | Yes | Directly solves the "predictable pricing" pain point |
| OTP-Verified Job Start & End | Both | Yes | Low-cost feature ensuring accountability and safety |
| One-Tap Job Acceptance Flow | Professional | Yes | Essential given low digital literacy |
| In-App Real-Time Chat | Both | **No** | High complexity — fallback to direct call masking for MVP |
| AI-Driven Dynamic Surge Pricing | Platform | **No** | High complexity — static rates suffice for launch |

## User journey

**Discovery** → customer selects a category, sees fixed base pricing, taps book. **Matching** → system pings the nearest verified professional, who gets a clear big-button prompt showing location and payout. **Execution** → professional arrives, customer shares an Arrival OTP, work completes, Completion OTP entered. **Settlement** → cashless payment collected, two-way binary rating (thumbs up/down, for speed).

## Go-to-market: solving liquidity

**Cold start:** constrain constraints - launch in one specific city (e.g. Bangalore) with only two high-frequency categories (Electricians, AC Repair) to concentrate liquidity from day one.

**Supply-side (the anchor):** direct offline onboarding at hardware wholesale markets and local hubs, backed by a Guaranteed Minimum Daily Payout for the first 30 days to de-risk trying a new platform.

**Demand-side:** geo-targeted hyper-local digital ads focused entirely on safety and price guarantees, plus physical flyers in target residential complexes.

## North Star Metric

**Completed, OTP-verified bookings per week, per city.**

*(Sourced from Week 3's recap slide, which states this metric as "unchanged" from Week 2 - the submitted Week 2 deck available in this folder ends at the GTM section above, and the metrics/risks/wireframes portions of the brief aren't present in that file. If a separate metrics/risks slide or wireframe link exists outside this PDF, it belongs here.)*
