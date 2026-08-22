# Product Matters 6.0 - E-Cell, IIT Guwahati

A four-week product management programme run by E-Cell, IIT Guwahati, culminating in a capstone project set by **IndusInd General Insurance**. This repository collects the two build deliverables I produced during the programme, in the order they were made.

**By:** Chhavi Tanwar · **Programme:** Product Matters 6.0 (individual participation) · **Jun - Jul 2026**

---

## The two projects

| | **TrustFix** (Week 3) | **IndusCare+** (Capstone) |
|---|---|---|
| **What** | Clickable prototype of a trust-first home-services marketplace | Product case + prototype for a bank-led insurance platform |
| **Brief** | Turn Week 2's personas, MVP scope and wireframes into an interactive, annotated walkthrough | Reimagine how customers discover, buy, manage, claim and renew general insurance |
| **Set by** | Programme curriculum | IndusInd General Insurance (real corporate brief) |
| **Emphasis** | Interaction design, two-sided flows, trust mechanics | Market sizing, prioritisation, metrics, GTM, roadmap |
| **Deliverables** | Clickable prototype + rationale annotations | 15-slide deck + clickable prototype |
| **Folder** | [`trustfix-week3-prototype/`](./trustfix-week3-prototype) | [`induscare-capstone/`](./induscare-capstone) |
| **Live demo** | https://product-matters-trustfix-prototype.onrender.com | https://product-matters-induscare.onrender.com |

---

## How the two fit together

The programme ran weekly modules (product strategy, root-cause analysis, guesstimates, product design and improvement, behavioural interviewing, SQL), each assessed by a quiz and a submission-based assignment. Two of those submissions were builds rather than write-ups, and they sit at opposite ends of the product craft:

**TrustFix (Week 3)** works bottom-up from an interface. The brief called for AI-assisted prototyping without engineering support, so the deliverable is a two-sided walkthrough - a customer app and a professional app - where every screen carries an annotation panel naming the Week 2 artefact it traces back to, and flagging the decisions the wireframes had left unresolved. Building it was the point: sequencing questions that a static wireframe can defer (who enters which OTP, when payment fires relative to completion, what happens on a mid-booking cancellation) have to be answered once the flow is clickable.

**IndusCare+ (Capstone)** works top-down from a market. It opens on penetration and addressable base, positions against aggregators, insurer apps and rival bancassurance, commits to a single persona, then narrows through scope justification and MoSCoW prioritisation to a North Star metric, a phased GTM and a four-quarter roadmap. The prototype here is supporting evidence for the strategy rather than the centre of it.

Read together: one project shows the ability to resolve a product down to the interaction, the other to reason up from a market to a roadmap.

---

## Skills demonstrated across both

- **Discovery & framing** - persona definition, pain-point articulation, problem statements
- **Prioritisation** - MoSCoW, explicit scope cuts, deliberate "won't have (v1)" calls
- **Metrics** - North Star definition, adoption / engagement / retention metric trees
- **Strategy** - market sizing, competitor positioning, whitespace identification, phased GTM, roadmapping
- **Interaction design** - two-sided marketplace flows, trust and verification mechanics, edge-case handling, low-digital-literacy constraints
- **Prototyping** - dependency-free HTML/CSS/JS prototypes, deployed as static sites

---

## Repository structure

```
.
├── README.md
├── trustfix-week3-prototype/
│   ├── README.md
│   └── index.html                      # the entire prototype, single file
└── induscare-capstone/
    ├── README.md
    ├── index.html                      # clickable prototype
    └── induscare-capstone-deck.pdf     # 15-slide submitted deck
```

Each project folder has its own README with full detail. Both prototypes are dependency-free single files - no build step, no backend.
