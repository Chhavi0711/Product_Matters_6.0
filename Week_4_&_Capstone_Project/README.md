# IndusCare+ - Capstone Project

**Product Matters 6.0 · E-Cell IIT Guwahati × IndusInd General Insurance** - [back to programme overview](../README.md)

A mobile-first insurance protection platform for IndusInd Bank customers, built as the programme's final capstone against a brief set by IndusInd General Insurance: reimagine how customers discover, purchase, and manage general insurance across the full lifecycle - discovery, policy management, claims and renewals.

🔗 **Live demo:** https://product-matters-induscare.onrender.com
📄 **Deck:** [`induscare-capstone-deck.pdf`](./IndusCare_Capstone_Deck.pdf) (15 slides)

## The problem

Insurance is bought once and forgotten. Policies are purchased across scattered channels - agents, comparison apps, insurer apps - with no single view of what a customer owns. Coverage is explained in jargon, claims are the most stressful part of the experience at the moment insurance matters most, and renewals are treated as one-time transactions rather than an ongoing relationship, so retention leaks every year.

## The opportunity

India's insurance penetration sits at roughly 4% against a ~7% global average - headroom that is structural rather than competitive. IndusInd's addressable base is ~35M retail and digital banking customers who already trust the bank with their money, while the average insured Indian household holds fewer than three policies spread across unrelated providers with zero cross-visibility.

The thesis: banks sit on income, spending, asset and life-stage data that insurers never see. That data - not distribution alone - is the real moat for a bank-led insurance platform.

**Whitespace:** aggregators compare widely but hold no banking data and stay transactional; insurer apps have product depth but can't unify a portfolio across a single-insurer silo; rival bancassurance still sells and forgets. None own a bank-backed, multi-insurer, lifecycle-first platform.

## Persona

**Rhea Malhotra**, 29, product marketer in Bengaluru. IndusInd salary account holder, owns a two-wheeler and a health policy bought through an agent she's since lost touch with, pays premiums but has never filed a claim. She forgets renewal dates, can't compare her existing cover to alternatives, and dreads the idea of ever filing a claim — while already checking her IndusInd app weekly, making insurance an extension of an existing habit rather than a new one.

> *"I know I'm covered for something. I just don't know for what."*

## Product vision

From a policy you bought once, to a protection layer that works for you every day - built on three pillars: **one view** (every policy across every insurer in one bank app), **proactive not reactive** (renewal nudges, coverage-gap alerts, life-stage recommendations before customers ask), and **effortless claims** (guided, document-light filing with real-time status).

**Scope:** Health, Motor and Home first - chosen for digitisation ease, claim frequency and emotional stakes, and home-loan cross-sell respectively. Travel, pet, cyber and rental become Phase 2 modules once the core lifecycle engine is proven.

## Prototype

Four screens carry the experience, and all four are clickable in the demo:

| Screen | What it does |
|---|---|
| **Home** | Coverage snapshot plus one proactive nudge, styled to sit inside the existing IndusInd app |
| **My Policies** | Every policy, every insurer, one scroll - status, premium and renewal date at a glance |
| **Compare & Buy** | Plain-language plan cards side by side with a single primary CTA, KYC auto-filled from the bank profile |
| **File a Claim** | Step-based form with progress indicator, photo upload, AI pre-check, and a live status timeline |

## North Star metric

**Active Protected Customers** - customers with 2+ active policies *and* at least one app session in the last 30 days. Supported by adoption (% of banking customers with 1+ policy), cross-sell (attach rate), retention (renewal rate, 30-day lapse), engagement (claim NPS, dashboard MAU), efficiency (claim resolution time, % claims filed unassisted) and growth (in-app premium volume vs traditional channels).

## Go-to-market

Four phases: soft launch to existing app users via in-app banner and relationship-manager outreach → cross-sell nudges triggered off real banking events (home loan disbursal → home insurance) → retention loop through renewal campaigns and loyalty ties → category expansion once engagement and claim-satisfaction metrics hold.

## Risks and assumptions

Assumes insurer partners will expose APIs for real-time policy and claim data, that customers trust their bank to manage insurance in-app, and that KYC/DigiLocker integration removes most purchase friction. Key risks: IRDAI bancassurance and data-sharing compliance across tie-ups, low early claims volume making AI pre-check hard to trust, and cannibalising branch and agent-led sales without a clear channel strategy.

## Tech

- Plain HTML, CSS and JavaScript — no framework, no bundler, no backend
- All state simulated in-browser; resets on refresh
- Hosted on [Render](https://render.com) as a static site (no build command)

## Running locally

Open `index.html` directly, or serve it:

```bash
python3 -m http.server 8000
```
