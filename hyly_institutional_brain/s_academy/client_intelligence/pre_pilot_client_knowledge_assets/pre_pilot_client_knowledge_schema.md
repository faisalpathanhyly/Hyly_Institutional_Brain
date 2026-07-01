# Pre-Pilot Client Knowledge Schema

## Purpose

Pre-Pilot Client Knowledge Assets capture early client intelligence before or during pilot readiness.

These assets help Hyly teams understand client needs, prepare for pilots, connect client problems to the right product direction, and define what needs to be validated.

They are not Client Proof Stories yet because the solution and outcome may not be fully validated.

---

## Standard Location

```text
s_academy/client_intelligence/pre_pilot_client_knowledge_assets/
```

Assets should be organized by product:

```text
pre_pilot_client_knowledge_assets/
├── hayley/
├── halo/
└── helix/
```

---

## Product Folder Direction

### hayley/

Use for client knowledge related to Hayley, including lead engagement, automation, chat, email, voice, follow-up, leasing team support, and prospect communication workflows.

### halo/

Use for client knowledge related to Halo, including reporting, attribution, owner visibility, data intelligence, spend visibility, performance reporting, and connected data workflows.

### helix/

Use for client knowledge related to Helix, including ad audits, alerts, recommendations, campaign diagnostics, QA workflows, and optimization intelligence.

---

## File Naming Format

```text
client_name_problem_area.md
```

### Examples

```text
sample_client_reporting_visibility.md
sample_client_lead_follow_up_automation.md
sample_client_ad_audit_readiness.md
```

---

## When To Create A Pre-Pilot Asset

Create a Pre-Pilot Client Knowledge Asset when Hyly has early client information but still needs to validate the solution, fit, pilot scope, success criteria, or outcome.

Use this asset when the team needs to answer:

```text
What do we know about this client before the pilot?
What do we still need to validate?
How does this map to Hayley, Halo, or Helix?
What should the pilot prove?
```

---

## Standard Asset Format

Use this format for every pre-pilot asset:

```markdown
# Pre-Pilot Client Knowledge Asset: [Client Name] — [Problem Area]

## Client Context

[Who the client is and what situation they are in]

## Product Area

**Product:** [Hayley / Halo / Helix]

## Client-Stated Problem

[What the client said they are struggling with]

## Pain Points

- [Pain point]
- [Pain point]
- [Pain point]

## Possible Bottlenecks

- [Possible bottleneck]
- [Possible bottleneck]

## What Hyly Needs To Validate

- [Validation point]
- [Validation point]
- [Validation point]

## Product Fit Hypothesis

[Why this product may help this client]

## Proposed Solution Direction

[What Hyly may recommend, configure, test, or observe during the pilot]

## Pilot Success Criteria

- [What should improve, reduce, clarify, automate, or prove]
- [Success indicator]

## Risks / Open Questions

- [Risk or unknown]
- [Risk or unknown]

## Source

**Source Type:** [Client call / Sales note / Research call / Demo / Internal discussion]  
**Source Link:** [Link if available]  
**Date:** [Date]

## Media / Supporting Material

**Media Type:** [Video / Recording / Carousel / Notes / Deck]  
**Media Link:** [Cloudinary or Google Drive link]

## Internal Notes

[Internal-only context]
```

---

## Asset Maturity

A Pre-Pilot Client Knowledge Asset can become a Client Proof Story after the pilot or implementation produces enough validated learning.

Lifecycle:

```text
Pre-Pilot Client Knowledge Asset
↓
Pilot Learning
↓
Validated Outcome
↓
Client Proof Story
```

Do not move an asset into Client Proof Stories until the problem, solution, and outcome are clear enough to create a reusable story.

---

## Writing Rules

Keep the asset focused on pilot readiness and validation.

Do:

```text
Capture what the client said
Separate known facts from assumptions
Identify what Hyly needs to validate
Map the problem to the relevant product
Define pilot success criteria
Add source links when available
```

Do not:

```text
Claim the solution has worked before it is validated
Invent outcomes
Turn the asset into a testimonial
Add unrelated product details
Mix multiple clients in one file
```

---

## Completion Checklist

Before saving a Pre-Pilot Client Knowledge Asset, confirm:

```text
[ ] Product folder is correct
[ ] Client-stated problem is clear
[ ] Pain points are captured
[ ] Possible bottlenecks are listed
[ ] Validation points are included
[ ] Product fit hypothesis is explained
[ ] Pilot success criteria are defined
[ ] Risks or open questions are included
[ ] Source details are included where available
[ ] Media link is added if available
[ ] No unvalidated outcomes are claimed
```
