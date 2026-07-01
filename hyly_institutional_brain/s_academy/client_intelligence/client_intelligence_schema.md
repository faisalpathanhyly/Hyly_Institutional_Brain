# Client Intelligence Schema

## Purpose

Client Intelligence is the S.Academy knowledge area for capturing client-based learning that can help Hyly teams understand client problems, prepare for pilots, and reuse validated problem-solution examples.

This section is not a marketing testimonial library. It is an internal learning and intelligence system built from client context, problems, pain points, bottlenecks, product fit, pilot learnings, and reusable solution patterns.

---

## Scope

Client Intelligence currently includes two asset types:

```text
1. Client Proof Stories
2. Pre-Pilot Client Knowledge Assets
```

### Client Proof Stories

Client Proof Stories are validated problem-solution learning assets.

They answer:

```text
Have we solved a problem like this before?
```

They should be used when Hyly has enough context to explain the client problem, the bottleneck, the Hyly diagnosis, the product solution, the outcome or impact, and the reusable lesson for future clients.

### Pre-Pilot Client Knowledge Assets

Pre-Pilot Client Knowledge Assets capture early client intelligence before or during pilot readiness.

They answer:

```text
What do we know, what do we need to validate, and how should we prepare for this client pilot?
```

They should be used before the client example becomes validated proof.

---

## Standard Folder Structure

```text
s_academy/
└── client_intelligence/
    ├── client_intelligence_schema.md
    ├── client_proof_stories/
    │   ├── client_proof_story_schema.md
    │   └── stories/
    └── pre_pilot_client_knowledge_assets/
        ├── pre_pilot_client_knowledge_schema.md
        ├── hayley/
        ├── halo/
        └── helix/
```

---

## Asset Direction

Client Intelligence should support the full client learning lifecycle:

```text
Pre-pilot signal
↓
Pilot readiness
↓
Pilot learning
↓
Validated outcome
↓
Client proof story
```

A pre-pilot asset may later become a Client Proof Story only after Hyly has enough evidence to explain what was solved and why the solution worked.

---

## What Belongs Here

Client Intelligence should include assets that help teams understand or reuse client learnings.

Examples:

```text
Client-stated problems
Pain points
Bottlenecks
Product fit hypotheses
Pilot success criteria
Validation questions
Real problem-solution examples
Reusable solution patterns
Internal client learning notes
```

---

## What Does Not Belong Here

Avoid adding content that is only promotional or too raw to be useful.

Do not use this section for:

```text
Generic praise
Standalone client quotes
Website testimonial copy
Raw meeting transcripts without structure
Unverified outcome claims
Bug reports
Feature request lists without client context
```

If a client quote is useful, it can support a story, but it should not become the full asset.

---

## Naming Rules

Use lowercase folder and file names with underscores.

### File Naming Format

```text
client_name_problem_area.md
```

### Examples

```text
sample_client_reporting_visibility.md
sample_client_lead_follow_up_automation.md
sample_client_ad_audit_readiness.md
```

Do not use spaces or hyphens in file names.

---

## Media Rules

Videos, carousels, screen recordings, visuals, and supporting files should be uploaded to Cloudinary or Google Drive.

Git should only store the media link inside the relevant asset.

### Media Placeholder

```markdown
## Media / Supporting Material

**Media Type:** [Video / Carousel / Screen Recording / Visual / Notes / Deck]  
**Media Link:** [Cloudinary or Google Drive link]
```

The structured Git file remains the source of truth. Media supports the learning experience but should not replace the written asset.

---

## Quality Standard

A Client Intelligence asset is complete when it clearly answers:

```text
What client problem are we capturing?
Why does it matter?
Which product area does it connect to?
What has been validated or still needs validation?
How can this help future client conversations or internal learning?
```

If the asset does not answer those questions, it should be refined before it is treated as useful client intelligence.
