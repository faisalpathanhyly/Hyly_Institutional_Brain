# Hyly Institutional Brain and S.Academy Repository Guide

## Purpose

This repository is the first structured version of the Hyly Institutional Brain.

The Institutional Brain is the Git-based source of truth for knowledge assets, learning assets, prompts, instructions, governance rules, and supporting resources that can be used by humans, AI agents, and S.Academy.

S.Academy is Hyly.AI's AI-backed learning platform. It is similar to an LMS, but instead of being built fully inside a third-party LMS, it uses structured knowledge, Git, LLMs, and supporting tools to deliver courses, assessments, AI-guided learning, and other knowledge experiences.

The key distinction is:

```text
Git = Brain and source of truth
S.Academy = AI-backed learning platform
LLM = Intelligence layer
Learners = End users who consume the knowledge
```

## Core Architecture

```text
hyly_institutional_brain/
│
├── instructions.md
├── history.md
├── docs/
├── governance/
├── shared/
├── exports/
└── s_academy/
    ├── README.md
    ├── multifamily_industry/
    ├── client_intelligence/
    ├── ai_intelligence/
    ├── partner_integrations/
    └── competitor_intelligence/
```

## Why This Repository Exists

The organization needs a structured place where knowledge can be organized, version controlled, reused, and accessed by AI systems.

Notion has been useful for creating and drafting knowledge, but the long-term direction is to treat Git as the structured Institutional Brain.

The repository is designed so that knowledge does not remain trapped inside courses, isolated documents, or individual team members' heads. Instead, knowledge becomes a reusable asset that can support learning, AI agents, client intelligence, product understanding, and future knowledge systems.

## S.Academy

S.Academy sits inside the Institutional Brain because it is the main learning platform that will consume this knowledge.

S.Academy should not be treated as the source of truth. The source of truth is the Git-based Institutional Brain.

S.Academy uses selected knowledge from the brain to deliver:

- Courses
- Assessments
- AI tutor experiences
- Knowledge assets
- Future learning experiences

## Knowledge Domains

The repository contains five knowledge domains under S.Academy.

```text
s_academy/
├── multifamily_industry/
├── client_intelligence/
├── ai_intelligence/
├── partner_integrations/
└── competitor_intelligence/
```

### Multifamily Industry Knowledge

This domain contains knowledge about the multifamily industry, including terminology, concepts, workflows, personas, regulations, industry context, and related learning assets.

For the MVP, this domain includes course folders for:

```text
introduction_to_multifamily
halo_overview
```

These courses were identified from the Hyly.AI Knowledge Brain in Notion and are being placed under Multifamily Industry Knowledge because they support foundational multifamily and Halo learning.

### Client Intelligence

This domain contains structured customer and client knowledge.

It can include:

- Client meeting insights
- Product feedback
- Pain points
- Adoption challenges
- Success stories
- Business impact narratives
- Videos and supporting references

Videos should generally be stored as links inside Markdown files rather than uploaded directly into Git, unless the team decides otherwise.

### AI Intelligence

This domain contains AI-related knowledge.

It can include:

- AI trends
- AI tools
- Internal AI experiments
- Claude notes
- DeepSeek research
- Prompt practices
- Provider-neutral AI considerations

### Partner Integrations

This domain is scaffolded for future use.

It will later contain partner and integration knowledge such as PMS, CRM, onboarding processes, dependencies, risks, limitations, and troubleshooting.

### Competitor Intelligence

This domain is scaffolded for future use.

It will later contain competitor knowledge, differentiators, positioning, comparison notes, and battlecard-style assets.

## MVP Focus

For the first 30 days, the active focus is:

```text
multifamily_industry
client_intelligence
ai_intelligence
```

The other two domains exist so the repository can scale without needing to be redesigned later.

## Naming Standard

Use underscores in all folder and file names.

Correct:

```text
multifamily_industry
client_intelligence
introduction_to_multifamily
review_workflow.md
quality_standards.md
```

Incorrect:

```text
multifamily-industry
client-intelligence
introduction-to-multifamily
review-workflow.md
quality-standards.md
```

## Single README Rule

This file is the single README for the S.Academy repository area.

Do not add separate README files inside each course, domain, or subfolder unless the repository standard changes.

Use `instructions.md` for instructions and `history.md` for change tracking.

## How to Add a Knowledge Asset

To add a knowledge asset, first identify the correct knowledge domain.

For example, a client success story should go under:

```text
s_academy/client_intelligence/knowledge_assets/
```

A new AI experiment should go under:

```text
s_academy/ai_intelligence/experiments/
```

A multifamily concept should go under:

```text
s_academy/multifamily_industry/knowledge_assets/
```

The asset should be written in Markdown and should include enough context for both a human and an AI agent to understand it.

## How to Add a Video

Videos should usually be added as links inside Markdown files.

Example:

```markdown
# Halo Pre Pilot Explainer

## Video Link

https://example.com/video

## Summary

This video explains...

## Key Takeaways

...
```

This keeps Git focused on knowledge structure while the video itself remains hosted in the correct video platform.

## How to Update a Course Rule

Small updates can be made directly in GitHub.

Open the relevant file, click edit, make the text change, and commit.

There is no need to upload a new ZIP for every change.

## Change Tracking

All meaningful changes should be recorded in:

```text
history.md
```

This keeps a readable record of what changed, when it changed, why it changed, and which files were affected.
