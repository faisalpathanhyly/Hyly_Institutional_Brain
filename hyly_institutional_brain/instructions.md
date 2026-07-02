# Instructions

This file contains the working instructions for the Hyly Institutional Brain repository.

---

## Naming Standard

Use underscores for all folder and file names.

Correct examples:

```text
hyly_institutional_brain
s_academy
multifamily_industry_intelligence
client_intelligence
partner_integrations_intelligence
onboarding_intelligence
introduction_to_multifamily
quality_standards.md
review_workflow.md
```

Do not use hyphens in folder or file names.

Incorrect examples:

```text
hyly-institutional-brain
s-academy
multifamily-industry-intelligence
client-intelligence
partner-integrations-intelligence
onboarding-intelligence
quality-standards.md
```

---

## Repository Purpose

Git is the Institutional Brain. It is the long-term structured source of truth for knowledge assets, learning assets, prompts, instructions, schemas, and supporting resources.

S.Academy is the AI-backed learning platform that consumes selected knowledge from this brain and delivers it as courses, assessments, AI-guided learning, and other knowledge experiences.

Onboarding Intelligence uses S.Academy as the learning delivery platform, but it is not directly mapped as an S.Academy knowledge domain.

---

## Current Repository Areas

The repository currently includes these main areas:

```text
governance/
shared/
s_academy/
onboarding_intelligence/
```

### governance/

Stores repository rules, quality standards, lifecycle standards, and schemas for repeatable learning assets.

Governance may include:

```text
ownership.md
review_workflow.md
knowledge_lifecycle.md
quality_standards.md
schemas/
```

Current governance schemas include:

```text
governance/schemas/course_schema.md
governance/schemas/quiz_schema.md
governance/schemas/video_schema.md
```

These schemas define how repeatable S.Academy learning assets should be structured.

Actual learning content should not live in `governance/`.

### shared/

Stores reusable resources that may apply across multiple repository areas.

Examples include shared templates, prompts, standards, and reusable components.

### s_academy/

Stores the knowledge assets that power S.Academy learning experiences.

S.Academy contains intelligence domains such as:

```text
multifamily_industry_intelligence/
client_intelligence/
ai_intelligence/
partner_integrations_intelligence/
competitor_intelligence/
```

### onboarding_intelligence/

Stores onboarding structure, training plans, product intelligence references, evaluation assets, mindmaps, checklists, and performance tracking assets for new recruits and teams.

This brain supports employee onboarding, training, evaluation, performance refinement, and goal tracking.

It should use S.Academy learning material where relevant, but it should not duplicate full S.Academy course content.

---

## Active MVP Domains

For the current MVP, active work should focus on:

1. `multifamily_industry_intelligence`
2. `client_intelligence`
3. `ai_intelligence`
4. `onboarding_intelligence`

`partner_integrations_intelligence` is active for coordination with the CSM team and future integration-related courses.

`competitor_intelligence` is scaffolded for future use and should not be deeply populated unless explicitly approved.

---

## S.Academy Domain Rules

Each S.Academy intelligence domain should remain focused on its own knowledge category.

### multifamily_industry_intelligence/

Use this domain for foundational multifamily learning and structured courses.

Current course work includes:

```text
introduction_to_multifamily
halo_overview
```

Future work may include more courses categorized by department and cohort, along with assessments, quizzes, and evaluations to measure Hylee performance and knowledge.

### client_intelligence/

Use this domain for reusable client-based learning and client knowledge assets.

Current structures include:

```text
client_proof_stories/
pre_pilot_client_knowledge_assets/
```

Client Proof Stories should explain how Hyly solved real client problems.

Pre-Pilot Client Knowledge Assets should capture early client intelligence before or during pilot readiness and should be organized by product:

```text
hayley/
halo/
helix/
```

Client Intelligence should not duplicate Marketing testimonials. Marketing testimonials may be used as supporting proof, but Client Proof Stories should focus on problem, bottleneck, Hyly diagnosis, solution, outcome, and reusable learning.

### ai_intelligence/

Use this domain for AI-related knowledge such as AI Pulse content, AI workflows, prompt practices, AI experiments, LLM usage learnings, and future AI training modules.

AI Pulse content should be categorized by domain when added.

### partner_integrations_intelligence/

Use this domain for third-party integration knowledge, partner capabilities, integration limitations, onboarding guidance, and troubleshooting.

Future work should coordinate with the CSM team to develop integration-related courses and learning assets.

### competitor_intelligence/

Use this domain for competitor research, product comparisons, positioning notes, battle cards, and market intelligence.

Populate this area only when approved.

---

## Onboarding Intelligence Rules

`onboarding_intelligence/` is a separate brain at the repository level.

It is not directly mapped as an S.Academy knowledge domain.

It uses S.Academy as the learning delivery platform.

### Purpose

The purpose of `onboarding_intelligence/` is to provide a seamless structure for onboarding, training, evaluation, and performance refinement.

It should help Hyly:

```text
train new recruits
evaluate knowledge and readiness
refine performance gaps
track onboarding goals
reduce unclear onboarding
reduce repeated hiring and firing cycles by identifying gaps earlier
```

### Current Structure

```text
onboarding_intelligence/
├── README.md
├── onboarding_intelligence_schema.md
├── training_plans/
├── product_intelligence/
│   ├── hayley/
│   ├── halo/
│   ├── helix/
│   └── general_cohort/
├── evaluation_assets/
├── mindmaps/
├── checklists/
└── performance_tracking/
```

### Folder Rules

Use `training_plans/` for role-based or cohort-based training plans.

Use `product_intelligence/` for product-related onboarding knowledge assets, learning references, videos, and links to S.Academy material.

Use `evaluation_assets/` for evaluation plans, scorecards, readiness checks, and assessment assets.

Use `mindmaps/` for visual or structured learning maps for new recruits.

Use `checklists/` for onboarding checklists.

Use `performance_tracking/` for tracking onboarding progress, goals, gaps, and refinement plans.

### Placeholder Rule

If a folder is empty, use a visible `meta.json` file instead of `.gitkeep`.

The `meta.json` file should briefly explain the folder purpose and keep the folder visible in GitHub.

Standard placeholder format:

```json
{
  "folder": "",
  "purpose": "",
  "status": "placeholder",
  "notes": "This JSON file keeps the folder visible in GitHub until content assets are added."
}
```

---

## Schema Rules

Schemas define the standard structure for repeatable content.

Use governance-level schemas when the structure applies broadly across S.Academy learning assets.

Use domain-level schemas when the structure applies only to one domain.

Current governance-level schemas:

```text
governance/schemas/course_schema.md
governance/schemas/quiz_schema.md
governance/schemas/video_schema.md
```

Current domain-level schemas:

```text
s_academy/client_intelligence/client_intelligence_schema.md
s_academy/client_intelligence/client_proof_stories/client_proof_story_schema.md
s_academy/client_intelligence/pre_pilot_client_knowledge_assets/pre_pilot_client_knowledge_schema.md
onboarding_intelligence/onboarding_intelligence_schema.md
```

When creating or updating an asset, follow the relevant schema first.

---

## Course Rule

Courses should follow the course schema.

The course schema lives at:

```text
governance/schemas/course_schema.md
```

Courses should preserve approved source content as closely as Markdown allows.

Do not rewrite, summarize, expand, or compress approved course content during migration.

Course content should include, where applicable:

```text
meta.json
initial_message.md
table_of_contents.md
chapters/
questions_and_answers/question_bank.md
media links
knowledge checks
chapter assessments
```

---

## Quiz and Assessment Rule

Quizzes, knowledge checks, chapter assessments, and course assessments should follow:

```text
governance/schemas/quiz_schema.md
```

Quiz content should be aligned with approved learning content.

Do not invent questions, answers, outcomes, or examples that are not supported by the approved source material.

---

## Video Rule

Learning videos should follow:

```text
governance/schemas/video_schema.md
```

Videos may be acquired from the Growth team.

Videos should be uploaded to:

```text
Cloudinary
Google Drive
```

Git should store the video metadata, context, key takeaways, related asset path, and video link.

Do not upload large video files directly into Git.

---

## README Rule

There should be one main README file inside the S.Academy section:

```text
s_academy/README.md
```

This README should contain the S.Academy explanation for teammates and AI agents.

Do not add separate README files inside each course or S.Academy knowledge domain unless this rule is changed later.

The repository root may also contain a short root README that acts as the entry point and points readers to the main project folder.

`onboarding_intelligence/README.md` is allowed because `onboarding_intelligence/` is a separate repository-level brain and not an S.Academy knowledge domain.

---

## History Rule

Every meaningful repository update should be recorded in:

```text
history.md
```

Each entry should capture:

```text
Date
Contributor
Change Name
Change Type
What Changed
Why It Changed
Affected Location
Notes
```

Update `history.md` for major milestones such as:

```text
new brain added
domain renamed
schema added
course migration completed
client intelligence structure updated
onboarding intelligence added
governance schema added
README architecture updated
```

---

## Editing Rule

Small text updates can be made directly in GitHub using the edit button.

The repo does not need to be re-imported as a ZIP for every change.

Large structural changes should be reviewed first because folder decisions affect AI readability, governance, and future scalability.

If GitHub upload hides empty folders, use visible `meta.json` placeholder files instead of hidden `.gitkeep` files.

---

## Knowledge Asset Rule

Knowledge should be stored once and reused.

Courses, assessments, prompts, onboarding plans, videos, and learning experiences should reference source knowledge where possible instead of duplicating it.

If a course already exists in S.Academy, `onboarding_intelligence/` should link to it rather than duplicating the full course content.

---

## Media Rule

Videos, images, carousels, visuals, and recordings should be stored in Cloudinary or Google Drive.

Git should store:

```text
media title
media type
media link
purpose
learning context
related asset
key takeaways
review notes
```

Do not upload large media files directly into Git unless a future repository rule allows it.

---

## AI Agent Rule

AI agents should read files in this order before creating or changing content:

```text
1. instructions.md
2. README.md
3. s_academy/README.md, if the work is S.Academy-related
4. relevant governance schema
5. relevant domain schema
6. relevant domain or asset folder
```

For `onboarding_intelligence/` work, AI agents should read:

```text
1. instructions.md
2. README.md
3. onboarding_intelligence/README.md
4. onboarding_intelligence/onboarding_intelligence_schema.md
5. relevant onboarding folder
```

AI agents should not invent missing content. If the source is incomplete, they should state the gap clearly.
