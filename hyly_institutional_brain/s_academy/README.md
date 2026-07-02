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

The `governance/` area defines how the repository is managed, reviewed, structured, and kept reliable.

It does not store learning content or domain knowledge. It stores the standards that help knowledge remain accurate, consistent, and maintainable.

Typical governance documents may include:

- ownership standards
- review workflows
- knowledge lifecycle rules
- quality standards
- contribution expectations
- schemas for repeatable learning assets

Governance schemas define the standard structure for reusable S.Academy asset types such as courses, quizzes, and videos.

Current governance schema structure:

```text
governance/
└── schemas/
    ├── course_schema.md
    ├── quiz_schema.md
    └── video_schema.md
```

Actual learning content should remain inside the relevant S.Academy knowledge domain. Governance stores the standards for how those assets should be created, reviewed, and maintained.

---

## shared/

The `shared/` area contains reusable standards and resources that can apply across multiple areas of the repository.

Examples include:

- reusable templates
- common prompts
- shared standards
- reusable components

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
│   └── schemas/
│       ├── course_schema.md
│       ├── quiz_schema.md
│       └── video_schema.md
├── shared/
└── s_academy/
    ├── README.md
    ├── meta.json
    ├── multifamily_industry_intelligence/
    ├── client_intelligence/
    ├── ai_intelligence/
    ├── partner_integrations_intelligence/
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
├── multifamily_industry_intelligence/
│   └── courses/
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
├── partner_integrations_intelligence/
└── competitor_intelligence/
```

---

# Knowledge Domains

Knowledge inside S.Academy is organized into dedicated intelligence domains.

Each domain represents a specific area of institutional knowledge and should remain focused on its defined purpose.

Each intelligence domain has a current focus and future scope.

The current focus explains what is being worked on or maintained today.

The future scope explains how the domain can grow as the Institutional Brain and S.Academy mature.

---

## Multifamily Industry Intelligence

The `multifamily_industry_intelligence/` domain stores foundational learning content related to the multifamily industry, property management context, and Hyly product learning.

This domain helps learners understand the industry before moving into product-specific or client-specific knowledge.

### Current Focus

The current focus is on developing and maintaining structured S.Academy courses.

Current work includes:

- migrated course content from approved Notion sources
- course metadata
- initial learner messages
- table of contents
- chapter files
- media links
- knowledge checks
- question banks
- assessment material

Current courses include:

```text
introduction_to_multifamily
halo_overview
```

Courses are stored under:

```text
s_academy/multifamily_industry_intelligence/courses/
```

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

The governance-level course schema is stored at:

```text
governance/schemas/course_schema.md
```

The schema defines the standard format for courses regardless of topic. It covers course metadata, learner opening messages, table of contents, chapter files, media placeholders, key takeaways, knowledge checks, chapter assessments, question banks, and migration rules.

The Git version should preserve approved source content as closely as Markdown allows. Course migration should not rewrite, summarize, expand, or compress approved course content.

### Future Scope

The future scope of this domain includes:

- development and addition of more S.Academy courses
- categorization of courses by department
- categorization of courses by cohort
- assessments, quizzes, and evaluations to measure real-time Hylee performance
- tracking learner understanding across chapters, topics, and courses
- supporting onboarding and role-based learning paths for Hylees

The goal is to make this domain the foundation for structured multifamily learning and measurable learner readiness.

---

## Client Intelligence

The `client_intelligence/` domain captures reusable knowledge generated from client interactions, client problems, product discussions, pilot readiness, and validated client outcomes.

This domain is not meant to store raw meeting notes or duplicate Marketing testimonials. It exists to turn client knowledge into structured learning assets that help Hyly teams understand client needs, prepare for pilots, explain product value, and reuse proven problem-solution patterns.

### Current Focus

The current focus is on building two types of client knowledge assets:

```text
1. Client Proof Stories
2. Pre-Pilot Client Knowledge Assets
```

Client Proof Stories explain how Hyly solved real client problems.

They answer:

```text
Have we solved a problem like this before?
```

Pre-Pilot Client Knowledge Assets capture early client intelligence before or during pilot readiness.

They answer:

```text
What do we know about this client before the pilot, and what do we need to validate?
```

Current work includes:

- defining the Client Intelligence structure
- creating schemas for Client Proof Stories
- creating schemas for Pre-Pilot Client Knowledge Assets
- separating Client Proof Stories from Marketing testimonials
- organizing pre-pilot knowledge by Hayley, Halo, and Helix
- preparing the domain for CSM-requested client knowledge assets

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

### Client Proof Stories

Client Proof Stories are story-based learning assets that explain how Hyly solved real client problems.

They should explain:

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

Marketing testimonials may be used as supporting proof, but Client Proof Stories should not copy the testimonial format. The testimonial is evidence. The Client Proof Story is the problem-solving breakdown.

### Pre-Pilot Client Knowledge Assets

Pre-Pilot Client Knowledge Assets capture early client intelligence before or during pilot readiness.

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

### Future Scope

The future scope of this domain includes:

- adding more CSM-requested knowledge assets
- adding videos for current clients
- adding videos for pre-pilot clients
- developing a content library based on client requirements
- converting repeated client problems into reusable learning assets
- supporting Sales, CSM, Product, Product Marketing, L&D, and Onboarding teams
- using client knowledge to support future pilot readiness and client conversations

The goal is to make this domain the central place for structured client learning, client proof, and client-specific knowledge reuse.

---

## AI Intelligence

The `ai_intelligence/` domain captures organizational knowledge related to Artificial Intelligence.

This domain supports AI learning, AI research, AI workflows, prompt practices, and future AI-backed use cases inside Hyly.

### Current Focus

The current focus is to create a structured space for AI-related knowledge that can be reused across teams.

This may include:

- AI research
- AI workflows
- prompt practices
- AI experiments
- LLM usage learnings
- AI implementation notes

### Future Scope

The future scope of this domain includes:

- addition of AI Pulse content
- categorization of AI Pulse content by domain
- development of AI training modules
- organizing AI learnings into reusable knowledge assets
- supporting internal AI education for Hylees
- helping teams understand how AI can support workflows, learning, and decision-making

The goal is to make this domain the central place for AI learning, AI updates, and reusable AI knowledge inside the Institutional Brain.

---

## Partner Integrations Intelligence

The `partner_integrations_intelligence/` domain contains knowledge related to third-party systems, integration partners, onboarding workflows, integration limitations, and troubleshooting.

This domain supports teams that need to understand how Hyly works with integration partners and what is required during onboarding or implementation.

### Current Focus

The current focus is to organize integration-related knowledge into a structured learning area.

This may include:

- integration documentation
- partner capabilities
- integration limitations
- troubleshooting notes
- onboarding guidance
- implementation-related knowledge

### Future Scope

The future scope of this domain includes:

- coordinating with the CSM team to develop integration-related courses
- creating learning assets for partner-specific onboarding
- documenting integration limitations and common troubleshooting scenarios
- supporting CSM, implementation, onboarding, and client-facing teams
- turning partner integration knowledge into structured S.Academy learning content

The goal is to make this domain the trusted place for integration learning and partner-specific operational knowledge.

---

## Competitor Intelligence

The `competitor_intelligence/` domain captures knowledge related to market competitors.

This domain supports strategic decision-making, product positioning, and sales enablement by keeping competitive knowledge organized in one place.

### Current Focus

The current focus is to create a structured place for competitor-related knowledge.

This may include:

- competitor research
- product comparisons
- feature analysis
- battle cards
- positioning notes

### Future Scope

The future scope of this domain includes:

- developing competitor comparison assets
- supporting Sales with competitive positioning
- supporting Product Marketing with market research
- creating battle cards and objection-handling material
- organizing competitor insights into reusable knowledge assets

The goal is to make this domain the central place for competitive intelligence that can support strategy, positioning, and enablement.

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

Governance-level schemas apply to repeatable learning asset types.

Current governance-level schemas include:

```text
governance/schemas/course_schema.md
governance/schemas/quiz_schema.md
governance/schemas/video_schema.md
```

Domain-level schemas may also exist when the standard applies to a specific knowledge area.

Current domain-level schemas include:

```text
s_academy/client_intelligence/client_intelligence_schema.md
s_academy/client_intelligence/client_proof_stories/client_proof_story_schema.md
s_academy/client_intelligence/pre_pilot_client_knowledge_assets/pre_pilot_client_knowledge_schema.md
```

Use governance-level schemas when the structure applies broadly across S.Academy learning assets.

Use domain-level schemas when the structure applies only to one specific intelligence domain.

---

## Media Rules

Videos, images, carousels, visuals, and recordings should not be uploaded directly into Git unless a future repository rule says otherwise.

Media should be uploaded to:

```text
Cloudinary
Google Drive
```

The Git file should store the media link, context, and related learning asset.

This applies to course videos, Growth team videos, Client Proof Story media, and other learning media used by S.Academy.

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
