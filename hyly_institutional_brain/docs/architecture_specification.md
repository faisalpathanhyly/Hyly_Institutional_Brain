# Architecture Specification

## Hyly Institutional Brain

The Hyly Institutional Brain is the Git-based source of truth for structured institutional knowledge.

S.Academy is the AI-backed learning platform that consumes selected knowledge from the brain.

## Architecture

```text
Hyly Institutional Brain (Git)
        │
        ├── Governance
        ├── Shared Standards
        └── S.Academy
                │
                ├── Multifamily Industry
                ├── Client Intelligence
                ├── AI Intelligence
                ├── Partner Integrations
                └── Competitor Intelligence
```

## Core Decision

The repository uses one Git repo with multiple knowledge domains.

This avoids creating separate repositories too early. Each domain is still structured in a way that allows it to be split later if needed.

## Source of Truth

Git is the brain.

S.Academy consumes the brain.

AI supports delivery, tutoring, evaluation, and retrieval.

## MVP Domains

The active MVP domains are Multifamily Industry, Client Intelligence, and AI Intelligence.

Partner Integrations and Competitor Intelligence are scaffolded for later.
