# Hyly Institutional Brain

> **The centralized source of truth for Hyly.AI's institutional knowledge.**

---

# Welcome

Welcome to the **Hyly Institutional Brain**.

The Institutional Brain is the centralized repository where Hyly.AI's knowledge is created, organized, governed, and maintained. It serves as the organization's single source of truth for institutional knowledge and is designed to support both human contributors and AI-powered applications.

Unlike a traditional document repository, the Institutional Brain is built around structured knowledge rather than individual documents. Every piece of information stored within the repository is intended to be reusable, version controlled, and organized according to a common set of standards.

As the organization continues to grow, the Institutional Brain provides a scalable foundation that allows knowledge to evolve while remaining consistent, discoverable, and easy to maintain.

---

# Purpose

The Institutional Brain exists to solve a simple problem.

Knowledge is one of an organization's most valuable assets, yet it is often scattered across documents, meeting notes, presentations, chat conversations, and individual contributors. Over time, this creates duplication, inconsistent information, and makes it increasingly difficult to find trusted answers.

The Institutional Brain addresses this by providing a centralized repository where knowledge is:

* Structured
* Governed
* Version controlled
* Reusable
* AI-readable
* Easy to discover
* Easy to maintain

Rather than treating documents as the primary asset, the Institutional Brain treats **knowledge** as the primary asset.

Everything stored within this repository should contribute to strengthening the organization's institutional knowledge.

---

# Platform Architecture

The Institutional Brain forms the foundation of the Knowledge Management ecosystem.

```text
                           Hyly Institutional Brain
                              (Source of Truth)

                                        │
               ┌────────────────────────┼────────────────────────┐
               │                        │                        │

          Governance               Shared                  S.Academy
                                                               │
                                                       Knowledge Domains
                                                               │
                                                       Knowledge Assets
                                                               │
                                                      AI-backed Learning
                                                               │
                                                            Learners
```

The repository itself acts as the Institutional Brain.

Governance establishes how knowledge is managed.

Shared provides reusable standards and resources used across the repository.

S.Academy consumes institutional knowledge to deliver AI-backed learning experiences.

---

# Core Architecture

The architecture is built around a clear separation of responsibilities.

## Hyly Institutional Brain

The Institutional Brain is the organization's structured source of truth.

It stores institutional knowledge, governs how that knowledge is organized, and provides a consistent foundation that can be consumed by multiple systems over time.

Knowledge should always originate here.

---

## Governance

Governance defines how the repository is managed.

Rather than storing knowledge, this area contains the standards that ensure knowledge remains accurate, consistent, and maintainable.

Examples include ownership, review workflows, quality standards, and lifecycle management.

---

## Shared

The Shared area contains reusable components used throughout the repository.

Rather than duplicating structures or standards across multiple knowledge domains, reusable assets are maintained centrally.

Examples include:

* Schemas
* Templates
* Shared prompts
* Common standards

This ensures consistency across the entire Institutional Brain.

---

## S.Academy

S.Academy is Hyly.AI's AI-backed Learning Management Platform.

It is responsible for transforming institutional knowledge into learning experiences such as courses, assessments, AI tutoring, and future educational experiences.

S.Academy is **not** the source of truth.

Instead, it consumes knowledge from the Institutional Brain while allowing learners to interact with that knowledge through an AI-assisted learning experience.

---

# Repository Structure

```text
hyly_institutional_brain/

│
├── governance/
├── shared/
├── s_academy/
│
├── README.md
├── instructions.md
└── history.md
```

## governance/

Contains repository governance and operational standards.

This area defines how the Institutional Brain is managed and maintained.

Typical documents include:

* Ownership
* Review Workflow
* Knowledge Lifecycle
* Quality Standards

---

## shared/

Contains reusable standards and resources shared across the repository.

Examples include:

* Schemas
* Templates
* Shared prompts
* Reusable components

Any resource intended to be reused across multiple knowledge domains should reside here.

---

## s_academy/

Contains the knowledge that powers the S.Academy platform.

Knowledge is organized into independent knowledge domains while following the standards defined throughout the repository.

---

# Knowledge Domains

Knowledge within S.Academy is organized into dedicated knowledge domains.

Each domain represents a specific area of institutional knowledge while remaining independent from the others.

---

## Multifamily Industry

The Multifamily Industry domain serves as the organization's knowledge base for the multifamily industry.

It contains foundational industry knowledge together with the learning experiences required to educate new employees and future learners.

Examples include:

* Introduction to Multifamily
* Halo Overview
* Industry concepts
* Terminology
* Workflows
* Assessments
* Shared course prompts

This domain establishes the foundational knowledge required to understand the multifamily industry before progressing into product-specific knowledge.

---

## Client Intelligence

The Client Intelligence domain captures reusable knowledge generated through customer interactions.

Its objective is to transform customer knowledge into reusable institutional knowledge.

Examples include:

* Client meeting insights
* Success stories
* Product feedback
* Customer pain points
* Frequently asked questions
* Adoption journeys
* Best practices

Rather than storing isolated meeting notes, this domain focuses on capturing knowledge that can continuously improve learning and decision making.

---

## AI Intelligence

The AI Intelligence domain captures organizational knowledge related to Artificial Intelligence.

Its purpose is to consolidate research, experiments, prompt engineering practices, AI workflows, and emerging technologies into a reusable knowledge base.

Examples include:

* AI research
* Prompt engineering
* LLM evaluations
* AI experiments
* Best practices
* AI implementation patterns

As AI continues to evolve, this domain provides a centralized location for maintaining institutional AI knowledge.

---

## Partner Integrations

The Partner Integrations domain contains knowledge related to third-party systems and integrations.

Examples include:

* Integration documentation
* Partner capabilities
* Integration limitations
* Troubleshooting
* Onboarding guidance

This domain ensures that integration knowledge is maintained consistently and remains reusable across the organization.

---

## Competitor Intelligence

The Competitor Intelligence domain captures knowledge related to market competitors.

Examples include:

* Competitor research
* Product comparisons
* Feature analysis
* Battle cards
* Industry positioning

This knowledge supports strategic decision making while maintaining a centralized repository of competitive intelligence.

---

# Repository Standards

The Institutional Brain follows common standards to ensure consistency across all knowledge domains.

## instructions.md

Provides repository-wide instructions for contributors.

It explains how knowledge should be created, maintained, and organized throughout the repository.

---

## shared/schemas/

Schemas define the standard structure for different types of repository content.

Every document type should follow its corresponding schema to maintain consistency across the Institutional Brain.

Examples include:

* README Schema
* Course Schema
* Knowledge Asset Schema
* Assessment Schema
* Prompt Schema

---

## shared/templates/

Templates provide reusable starting points for creating new repository content.

Templates are based on their corresponding schemas and help contributors maintain consistency while creating new knowledge assets.

---

## history.md

Records significant repository milestones and architectural changes.

Git automatically maintains the technical history of every commit.

The History document exists to capture major repository changes that are meaningful from a business and knowledge management perspective.

---

# Knowledge Flow

Knowledge moves through the platform in a structured manner.

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

Knowledge should always originate within the Institutional Brain before being consumed by S.Academy.

This ensures that all learning experiences remain synchronized with the organization's source of truth.

---

# Repository Growth Strategy

The Institutional Brain has been intentionally designed as a single repository containing multiple knowledge domains.

Maintaining a unified repository provides consistent governance, reusable standards, and centralized knowledge management across the organization.

As individual knowledge domains mature, they can be separated into independent repositories without requiring the overall architecture to be redesigned.

This approach allows the repository to scale while preserving a consistent knowledge management framework.

---

# Contributing

Every contribution should strengthen the Institutional Brain.

Before creating or updating content:

1. Review the repository instructions.
2. Follow the appropriate schema.
3. Use the relevant template whenever available.
4. Organize knowledge within the appropriate knowledge domain.
5. Commit changes using a clear and meaningful commit message.

Following these standards ensures that institutional knowledge remains structured, reusable, and easy to maintain as the repository continues to grow.

---

# Closing Statement

The Hyly Institutional Brain is more than a Git repository.

It is the organization's institutional memory.

Every contribution should improve the quality, reliability, and reusability of organizational knowledge while ensuring that future teammates, AI systems, and learning platforms can continue building upon a trusted foundation.
