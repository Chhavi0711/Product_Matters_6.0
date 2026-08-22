# Week 1 - Product Teardown & Feature Innovation

**Product Matters 6.0 · E-Cell IIT Guwahati** - [back to programme overview](../README.md)

Individual assignment: pick an existing digital product, evaluate it as a Product Manager, and propose one scoped feature improvement backed by first-principles reasoning - not a redesign, a single justified fix.

📄 **Brief:** [`Week_1_assignment.pdf`](./Week_1_assignment.pdf)
📄 **Submission:** [`ProductMatters6.0_Assignment1_Final.pdf`](./ProductMatters6.0_Assignment1_Final.pdf)

## Product chosen: LinkedIn

**Life cycle verdict:** Maturity - supported by ~$15B revenue (2023) growing slower than its Growth-phase pace, the 2016 Microsoft acquisition (a classic maturity-stage asset with proven monetization), stable core features with only incremental innovation, and rising competitive pressure from Naukri, Glassdoor, and X for professional discourse.

**Persona:** Abhishek Sharma, 21, final-year engineering student, Kanpur - mobile-first, applies to 50+ roles and hears back from under 10%, and whose core need is transparency: knowing where an application actually stands.

**User flow mapped:** Search Jobs → View Listing → Easy Apply → Confirm Apply → Track Status → *Ghosted*. The critical friction sits at the last two steps: after submission, applicants enter a black box - no SLA, no feedback loop, no recruiter accountability.

## Critique

**Works well:** Easy Apply reduces friction, recruiter visibility into applicant profiles, Skills Assessments add credibility, Job Alerts aid discovery.

**Doesn't work:** zero recruiter accountability after a listing closes, applications stuck on "Under Review" indefinitely, no notification when a listing expires, Easy Apply's low friction creates a quality/volume mismatch, and Premium's InMail promise frequently goes unanswered anyway.

**Core pain point: application ghosting.** When a listing closes, applicants get no notification and their CV is effectively buried, with no SLA on recruiters to act.

## Proposed feature: Application Closure & Feedback System (ACFS)

*When a job listing closes, recruiters must review applications within 7 days — or applicants automatically receive a "Not Proceeding" notification with dignity.*

**First-principles framing:** the core assumption being challenged is "recruiter reviewing applicants is optional." First principle: a job listing is a two-sided contract - both the employer who posted it and the seeker who applied deserve a resolution, not silence.

**Mechanics:** listing expires → 7-day recruiter review window (with a dashboard countdown badge) → recruiter reviews or the system auto-closes → candidate is notified either way, with the option to save their profile for future roles. Recruiters can bulk-reject in one click; compliant companies get an "ACFS Compliant" badge, which is shown to candidates as a signal that boosts application rate.

**Expected impact:** higher trust and re-engagement on the user side (definitive answers instead of indefinite limbo); higher job-seeker DAU/WAU, recruiter accountability, and India-market differentiation from Naukri/Glassdoor on the business side. Tracked via ACFS adoption rate, time-to-resolution, candidate re-engagement rate, and NPS delta.

**Wireframes:** five low-fidelity screens (Job Details → Application Submitted → Status Dashboard → Recruiter Responds / Recruiter Ghosts) included at the end of the submission PDF, hand-sketched per the assignment's accepted-tools list.
