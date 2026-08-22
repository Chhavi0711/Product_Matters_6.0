# TrustFix - Clickable Prototype (Week 3)

**Product Matters 6.0 · E-Cell IIT Guwahati** - [back to programme overview](../README.md)

A functional, clickable prototype of TrustFix, a trusted home-services marketplace, built as the Week 3 deliverable: taking the Week 2 wireframes and MVP scope and turning them into an interactive walkthrough of the core customer and service-professional flows.

🔗 **Live demo:** https://product-matters-trustfix-prototype.onrender.com

## What this is

A single-page, dependency-free HTML/CSS/JS prototype that simulates two linked mobile apps side by side in a phone-frame UI:

- **Customer app (Riya)** - service discovery, fixed-price categories, verified professional matching, live tracking, OTP-verified job start, digital job card, OTP-gated payment, and a binary rating
- **Professional app (Rajesh)** - availability toggle, one-tap job acceptance, navigation, OTP-verified job start, in-progress execution (photo capture + checklist), completion OTP, and payout

Each screen ships with an annotation panel explaining the product reasoning behind it - what it traces back to from the Week 2 MVP, and any gaps or decisions that surfaced specifically while building.

## Why this approach

The assignment brief calls for AI-assisted / "vibe coded" prototyping without production engineering support. Rather than a multi-screen Figma/Visily click-through, this was built as one self-contained HTML file with vanilla JS state management - no framework, no build step, no backend. It's easy to host, easy to iterate on, and forces the same interaction-design decisions a native app would (navigation, state transitions, empty/loading states) without the overhead of real infrastructure.

## What building it surfaced

The annotation panels flag decisions the wireframes had left open. Among them:

- **Payment sequencing.** Week 2's journey slide listed "payment" and "OTP" in the same step without specifying order. Sequenced explicitly so completion-OTP confirmation fires before the charge, preventing payment for unfinished work.
- **Matching model.** The wireframe assumed customers pick from multiple professionals; building the tap-through showed choice paralysis undercuts the "predictable, no-friction" promise, so it was reduced to a single best match with a visible cancel path.
- **Unlaunched categories.** Wireframes never showed "coming soon" states — the build surfaced that unlaunched categories need an explicit disabled state rather than simple omission.
- **Open edge cases, left open deliberately.** Mid-booking cancellation after the professional is en route (no cancellation-fee policy existed), and mid-job parts unavailability — both flagged rather than faked.

## Tech

- Plain HTML, CSS, and JavaScript - no framework, no bundler
- Google Fonts (Fraunces + Inter) via CDN
- No backend, no database - all state is simulated in-browser and resets on refresh

## Running locally

No install needed. Either open `index.html` directly, or serve it:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deployment

Hosted on [Render](https://render.com) as a static site:
- **Build command:** none
- **Publish directory:** this folder

## Related deliverables

- **Week 2:** problem definition, personas, MVP scope, GTM strategy, wireframes (the upstream artefacts the annotations trace back to)
- **Week 3 deck:** "Prototyping TrustFix — From Wireframes to a Working Model"
