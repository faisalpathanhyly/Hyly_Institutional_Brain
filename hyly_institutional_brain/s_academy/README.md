# Hyly Institutional Brain

> **The centralized source of truth for Hyly.AI's institutional knowledge.**

---

# Welcome

Welcome to the **Hyly Institutional Brain**.

The Institutional Brain is the centralized repository where Hyly.AI's knowledge is created, organized, governed, and maintained. It serves as the organization's single source of truth for institutional knowledge and supports both human contributors and AI-powered applications.

Unlike a traditional document repository, the Institutional Brain is built around structured knowledge rather than standalone documents. Every piece of information stored here should be reusable, version controlled, discoverable, and organized according to a shared standard.

As Hyly.AI grows, this repository provides a scalable foundation for maintaining trusted knowledge across teams, products, learning experiences, and future AI-backed workflows.

---

# Purpose

The Institutional Brain exists to solve one core problem: important organizational knowledge often becomes scattered across Notion pages, meeting notes, presentations, chats, training material, and individual memory.

When knowledge is scattered, teams face:

- duplicated information
- inconsistent answers
- outdated references
- unclear ownership
- slower onboarding
- weaker decision-making
- difficulty reusing past learning

The Institutional Brain addresses this by giving Hyly.AI a single place where knowledge is:

- structured
- governed
- version controlled
- reusable
- AI-readable
- easy to review
- easy to maintain

The repository treats **knowledge** as the primary asset.

Every contribution should make Hyly's institutional knowledge clearer, more reliable, and easier to reuse.

---

# Platform Architecture

The Institutional Brain forms the foundation of Hyly.AI's Knowledge Management ecosystem.

```text
                           Hyly Institutional Brain
                              (Source of Truth)

                                        │
               ┌────────────────────────┼────────────────────────┐
               │                        │                        │

          Governance                 Shared                  S.Academy
                                                               │
                                                       Knowledge Domains
                                                               │
                                                       Knowledge Assets
                                                               │
                                                      AI-backed Learning
                                                               │
                                                            Learners
```

The repository acts as the source of truth.

Governance defines how knowledge is managed.

Shared contains reusable standards and resources.

S.Academy consumes institutional knowledge and turns it into AI-backed learning experiences.

---

# Core Architecture

The repository is organized around a clear separation of responsibilities.

## Hyly Institutional Brain

The Institutional Brain is the organization's structured source of truth.

It stores institutional knowledge, governs how that knowledge is organized, and provides a consistent foundation that can be consumed by S.Academy and future systems.

Knowledge should originate here before being converted into learning, enablement, or AI-backed experiences.

---

## governance/

The `governance/` area defines how the repository is managed.

It does not store learning content or domain knowledge. It stores the standards that help knowledge remain accurate, consistent, and maintainable.

Typical governance documents may include:

- ownership standards
- review workflows
- knowledge lifecycle rules
- quality standards
- contribution expectations

---

## shared/

The `shared/` area contains reusable standards and resources that can apply across multiple areas of the repository.

Examples include:

- shared schemas
- reusable templates
- common prompts
- shared standards

Resources should live in `shared/` when they are meant to be reused across multiple knowledge domains.

---

## s_academy/

The `s_academy/` area contains the knowledge that powers S.Academy.

S.Academy is Hyly.AI's AI-backed learning platform. It transforms institutional knowledge into learning experiences such as courses, assessments, story-based learning assets, client intelligence assets, and future educational formats.

S.Academy is not separate from the Institutional Brain. It is the learning layer inside the Institutional Brain.

---

# Repository Structure

```text
hyly_institutional_brain/
├── README.md
├── instructions.md
├── history.md
├── governance/
├── shared/
└── s_academy/
    ├── README.md
    ├── meta.json
    ├── multifamily_industry/
    ├── client_intelligence/
    ├── ai_intelligence/
    ├── partner_integrations/
    └── competitor_intelligence/
```

---

# S.Academy Structure

S.Academy is organized into knowledge domains.

Each domain contains knowledge assets that support a specific learning or intelligence purpose.

Current structure:

```text
s_academy/
├── README.md
├── meta.json
├── multifamily_industry/
│   └── courses/
│       ├── course_schema.md
│       ├── introduction_to_multifamily/
│       └── halo_overview/
├── client_intelligence/
│   ├── client_intelligence_schema.md
│   ├── client_proof_stories/
│   │   ├── client_proof_story_schema.md
│   │   └── stories/
│   └── pre_pilot_client_knowledge_assets/
│       ├── pre_pilot_client_knowledge_schema.md
│       ├── hayley/
│       ├── halo/
│       └── helix/
├── ai_intelligence/
├── partner_integrations/
└── competitor_intelligence/
```

---

# Knowledge Domains

Knowledge inside S.Academy is organized into dedicated knowledge domains.

Each domain represents a specific area of institutional knowledge and should remain focused on its defined purpose.

---

## Multifamily Industry

The `multifamily_industry/` domain stores foundational learning content related to the multifamily industry and Hyly product context.

This domain currently includes structured S.Academy courses migrated from approved Notion course sources into Git.

Current courses:

```text
s_academy/multifamily_industry/courses/
├── course_schema.md
├── introduction_to_multifamily/
└── halo_overview/
```

### Purpose

The purpose of this domain is to help learners understand:

- multifamily industry fundamentals
- property management context
- prospect and resident journeys
- reporting and data concepts
- Hyly product relevance inside multifamily workflows

### Course Structure

Each course should follow the standard course structure:

```text
course_name/
├── meta.json
├── initial_message.md
├── table_of_contents.md
├── chapters/
└── questions_and_answers/
    └── question_bank.md
```

The course schema is stored at:

```text
s_academy/multifamily_industry/courses/course_schema.md
```

The schema defines the standard format for courses regardless of topic. It covers course metadata, learner opening messages, table of contents, chapter files, media placeholders, key takeaways, knowledge checks, chapter assessments, question banks, and migration rules.

### Current Course Assets

The current migrated courses include:

- course metadata
- initial learner messages
- table of contents
- chapter content
- Cloudinary media links
- knowledge checks
- correct answers
- question banks
- assessment material

The Git version should preserve approved source content as closely as Markdown allows. Course migration should not rewrite, summarize, expand, or compress approved course content.

---

## Client Intelligence

The `client_intelligence/` domain captures reusable knowledge generated from client interactions, client problems, product discussions, pilot readiness, and validated client outcomes.

This domain is not meant to store raw meeting notes or duplicate Marketing testimonials. Its purpose is to turn client knowledge into structured learning assets that help Hyly teams understand client needs, prepare for pilots, explain product value, and reuse proven problem-solution patterns.

Current structure:

```text
s_academy/client_intelligence/
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

### Purpose

Client Intelligence supports:

- sales enablement
- client success conversations
- pilot preparation
- product learning
- onboarding
- L&D assets
- product marketing inputs
- reusable client problem patterns

It helps Hyly teams move from generic product claims to specific problem-solution proof.

---

### Client Proof Stories

Client Proof Stories are story-based learning assets that explain how Hyly solved real client problems.

They answer:

```text
Have we solved a problem like this before?
```

Client Proof Stories should explain:

- client context
- client problem
- pain points
- bottlenecks
- what Hyly identified
- product solution
- how the solution worked
- why the solution worked
- outcome or impact
- reusable pattern for future clients
- internal notes

Client Proof Stories are written for the multifamily and PMC audience. They should help future clients and internal teams recognize similar operational problems inside multifamily environments.

They are different from Marketing testimonials.

Marketing testimonials capture what clients say about Hyly. Client Proof Stories explain what Hyly solved, how the solution worked, and how that learning can help future multifamily or PMC clients.

Client Proof Stories are stored under:

```text
s_academy/client_intelligence/client_proof_stories/
```

The schema is stored at:

```text
s_academy/client_intelligence/client_proof_stories/client_proof_story_schema.md
```

Marketing testimonials may be used as supporting proof, but Client Proof Stories should not copy the testimonial format. The testimonial is evidence. The Client Proof Story is the problem-solving breakdown.

---

### Pre-Pilot Client Knowledge Assets

Pre-Pilot Client Knowledge Assets capture early client intelligence before or during pilot readiness.

They answer:

```text
What do we know about this client before the pilot, and what do we need to validate?
```

These assets help teams understand:

- who the client is
- what product area they are evaluating
- what problem they want solved
- what pain points they have shared
- what bottlenecks may block success
- what assumptions need validation
- what the pilot should prove
- what would count as success

Pre-Pilot Client Knowledge Assets are organized by product:

```text
s_academy/client_intelligence/pre_pilot_client_knowledge_assets/
├── hayley/
├── halo/
└── helix/
```

The schema is stored at:

```text
s_academy/client_intelligence/pre_pilot_client_knowledge_assets/pre_pilot_client_knowledge_schema.md
```

This section captures early-stage client knowledge. A successful pre-pilot asset may later become a Client Proof Story once the problem, solution, and outcome are validated.

The intended lifecycle is:

```text
Pre-Pilot Knowledge Asset
        │
        ▼
Pilot Learnings
        │
        ▼
Validated Outcome
        │
        ▼
Client Proof Story
```

---

## AI Intelligence

The `ai_intelligence/` domain captures organizational knowledge related to Artificial Intelligence.

Its purpose is to consolidate AI-related research, workflows, experiments, prompt engineering practices, and implementation learnings into a reusable knowledge area.

Examples may include:

- AI research
- prompt engineering
- LLM evaluations
- AI experiments
- AI workflows
- AI implementation patterns

---

## Partner Integrations

The `partner_integrations/` domain contains knowledge related to third-party systems and integrations.

Examples may include:

- integration documentation
- partner capabilities
- integration limitations
- troubleshooting notes
- onboarding guidance

This domain supports consistent understanding of Hyly's integration partners and related onboarding workflows.

---

## Competitor Intelligence

The `competitor_intelligence/` domain captures knowledge related to market competitors.

Examples may include:

- competitor research
- product comparisons
- feature analysis
- battle cards
- positioning notes

This domain supports strategic decision-making and keeps competitive knowledge centralized.

---

# Repository Standards

The Institutional Brain follows common standards so knowledge remains consistent across domains.

---

## instructions.md

The `instructions.md` file provides repository-wide instructions for contributors.

It explains how knowledge should be created, organized, updated, reviewed, and maintained.

---

## history.md

The `history.md` file records significant repository milestones and architectural changes.

Git automatically tracks technical commit history. The history file exists to capture major business and knowledge-management changes in a human-readable format.

History entries should follow the standard entry format:

```text
Date:
Contributor:
Change Name:
Change Type:
What Changed:
Why It Changed:
Affected Location:
Notes:
```

---

## Schemas

Schemas define the standard structure for different types of repository content.

Some schemas live in `shared/` when they apply broadly across the repository. Other schemas live inside the domain or folder they govern.

Current domain-level schemas include:

```text
s_academy/multifamily_industry/courses/course_schema.md
s_academy/client_intelligence/client_intelligence_schema.md
s_academy/client_intelligence/client_proof_stories/client_proof_story_schema.md
s_academy/client_intelligence/pre_pilot_client_knowledge_assets/pre_pilot_client_knowledge_schema.md
```

Domain-level schemas should be used when the standard applies to a specific knowledge area rather than the entire repository.

---

# Knowledge Flow

Knowledge should move through the platform in a structured way.

```text
Knowledge Created
        │
        ▼
Knowledge Domain
        │
        ▼
Knowledge Asset
        │
        ▼
Institutional Brain
        │
        ▼
S.Academy
        │
        ▼
AI-backed Learning
        │
        ▼
Learners
```

Knowledge should be captured in the right domain before it is reused in learning, enablement, product, or AI-backed experiences.

---

# Repository Growth Strategy

The Institutional Brain is currently designed as one repository containing multiple knowledge domains.

This keeps governance, standards, and knowledge management centralized while the repository is still maturing.

As individual domains mature, they can later be separated into independent repositories if needed without redesigning the overall knowledge architecture.

---

# Contributing

Every contribution should strengthen the Institutional Brain.

Before creating or updating content:

1. Review `instructions.md`.
2. Place the asset in the correct knowledge domain.
3. Follow the relevant schema.
4. Preserve approved source content where migration is involved.
5. Use clear file and folder names with underscores.
6. Update `history.md` for major milestones or architecture changes.
7. Commit changes with a clear message.

Following these standards helps keep institutional knowledge structured, reusable, and easy to maintain.

---

# Closing Statement

The Hyly Institutional Brain is more than a Git repository.

It is Hyly.AI's institutional memory.

Every contribution should improve the quality, reliability, and reusability of organizational knowledge so future teammates, AI systems, and learning platforms can continue building on a trusted foundation.
