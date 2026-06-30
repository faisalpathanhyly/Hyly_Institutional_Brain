# Instructions

This file contains the working instructions for the Hyly Institutional Brain repository.

## Naming Standard

Use underscores for all folder and file names.

Correct examples:

```text
hyly_institutional_brain
s_academy
multifamily_industry
client_intelligence
introduction_to_multifamily
quality_standards.md
review_workflow.md
```

Do not use hyphens in folder or file names.

Incorrect examples:

```text
hyly-institutional-brain
s-academy
multifamily-industry
client-intelligence
quality-standards.md
```

## Repository Purpose

Git is the Institutional Brain. It is the long-term structured source of truth for knowledge assets, learning assets, prompts, instructions, and supporting resources.

S.Academy is the AI-backed learning platform that consumes selected knowledge from this brain and delivers it as courses, assessments, AI-guided learning, and other knowledge experiences.

## Active MVP Domains

For the first 30 days, active work should focus on:

1. Multifamily Industry Knowledge
2. Client Intelligence
3. AI Intelligence

Partner Integrations and Competitor Intelligence are scaffolded for future use but should not be deeply populated unless explicitly approved.

## README Rule

There should be only one README file inside the S.Academy section:

```text
s_academy/README.md
```

This README should contain the full repository explanation for teammates and AI agents.

Do not add separate README files inside each course or each knowledge domain unless this rule is changed later.

## History Rule

Every meaningful repository update should be recorded in:

```text
history.md
```

Each entry should capture:

- Date
- Contributor
- Commit or change name
- What changed
- Why it changed
- Affected folders or files

## Editing Rule

Small text updates can be made directly in GitHub using the edit button. The repo does not need to be re-imported as a ZIP for every change.

Large structural changes should be reviewed first because folder decisions affect AI readability, governance, and future scalability.

## Knowledge Asset Rule

Knowledge should be stored once and reused. Courses, assessments, prompts, and learning experiences should reference source knowledge where possible instead of duplicating it.

## AI Agent Rule

AI agents should read this file first, then read `s_academy/README.md`, then inspect the relevant domain or course folder before creating or changing content.
