# Week 3 - TrustFix: Clickable Prototype

**Product Matters 6.0 · E-Cell IIT Guwahati** - [back to programme overview](../README.md) · builds directly on [Week 2](../Week_2)

A functional, clickable prototype of TrustFix, built as the Week 3 deliverable: taking Week 2's wireframes and MVP scope and turning them into an interactive walkthrough of the core customer and service-professional flows.

🔗 **Live demo:** https://product-matters-trustfix-prototype.onrender.com
📄 **Brief:** [`Week_3_assignment.pdf`](./Week_3_assignment.pdf)
📄 **Updated deck:** [`ProductMatters6.0_Assignment3_Final.pdf`](./ProductMatters6.0_Assignment3_Final.pdf) - *"TrustFix: From Wireframes to a Working Model"*

## What this is

A single-page, dependency-free HTML/CSS/JS prototype simulating two linked mobile apps side by side in a phone-frame UI:

- **Customer app (Riya)** - service discovery, fixed-price categories, verified professional matching, live tracking, OTP-verified job start, digital job card, OTP-gated payment, and a binary rating
- **Professional app (Rajesh)** - availability toggle, one-tap job acceptance, navigation, OTP-verified job start, in-progress execution (photo capture + checklist), completion OTP, and payout

Every screen ships with an annotation panel naming the Week 2 artefact it traces back to, and flagging any gap surfaced specifically while building.

## Tools & approach

Built with **Claude** as the AI-assisted / "vibe coding" tool - describing each screen's intent and letting the assistant translate the Week 2 wireframes and user journey directly into working markup, rather than hand-writing it. Delivered as one self-contained HTML file with vanilla JS state management: no framework, no build step, no backend, two toggleable app frames (Customer/Professional) in a single shareable prototype, each screen carrying a built-in rationale panel.

**By the numbers:** 2 end-to-end flows prototyped (customer booking + professional job acceptance), 15 screens wired into one clickable prototype (8 customer + 7 professional), 5 concrete product decisions resolved that Week 2 had left implicit.

**Held constant from Week 2:** both personas, the three pillars, the MVP scope, and the cold-start GTM - nothing here changed. What sharpened were the interaction details underneath them.

## What building it surfaced

- **Payment sequencing.** Week 2's journey slide listed "payment" and "OTP" in the same step without specifying order. Sequenced explicitly so completion-OTP confirmation fires before the charge, preventing payment for unfinished work.
- **Matching model.** The wireframe assumed customers pick from multiple professionals; the tap-through showed choice paralysis undercuts the "predictable, no-friction" promise, so it was reduced to a single best match with a visible cancel path.
- **Unlaunched categories.** Wireframes never showed "coming soon" states - the build surfaced that unlaunched categories need an explicit disabled state rather than simple omission.
- **Payout timing.** Split into two explicit events: completion code shown → customer confirms → payout releases, rather than a vague "job marked complete."

## Updated success metrics & risks

**North Star Metric - unchanged:** Completed, OTP-verified bookings per week, per city. Reinforced by the prototype's booking-to-confirmed-match rate, arrival-OTP share rate (a proxy for trust in the safety flow), rebooking rate, and professional accept-rate within 45 seconds.

**New risks surfaced while prototyping:**
- **No cancellation-fee policy** - customers can cancel post-match at zero cost today; needs a rule before pilot launch
- **No mid-job parts-unavailable flow** - a professional has no defined path if a job can't be finished as booked
- **OTP-sharing friction** - two separate 4-digit codes per job may confuse first-time, low-literacy users; flagged for usability testing
- **No visible fallback on single-match design** - if the nearest verified professional doesn't respond, the customer currently sees no re-match state

## Tech

- Plain HTML, CSS, and JavaScript - no framework, no bundler
- Google Fonts (Fraunces + Inter) via CDN
- No backend, no database - all state is simulated in-browser and resets on refresh

## Running locally

```bash
python3 -m http.server 8000
```

## Deployment

Hosted on [Render](https://render.com) as a static site - build command: none, publish directory: this folder.
