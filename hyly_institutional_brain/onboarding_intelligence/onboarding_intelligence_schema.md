# onboarding_intelligence_schema

## Purpose

This schema defines the standard structure for assets stored inside `onboarding_intelligence`.

`onboarding_intelligence` supports employee onboarding, training, evaluation, and performance refinement.

It should organize onboarding knowledge in a way that helps Hyly train new recruits, evaluate their readiness, identify performance gaps, and refine learning outcomes.

---

## Standard Folder Structure

```text
onboarding_intelligence/
├── README.md
├── onboarding_intelligence_schema.md
├── training_plans/
├── product_intelligence/
├── evaluation_assets/
├── mindmaps/
├── checklists/
└── performance_tracking/
```

---

## Folder Placeholder Rule

Each empty folder should include a visible `meta.json` file until real content assets are added.

The placeholder JSON keeps the folder visible in GitHub and briefly explains the folder purpose.

### Standard Folder meta.json

```json
{
  "folder": "",
  "purpose": "",
  "status": "placeholder",
  "notes": "This JSON file keeps the folder visible in GitHub until content assets are added."
}
```

---

## Asset Types

`onboarding_intelligence` currently supports these asset types:

```text
1. Training Plans
2. Product Intelligence Assets
3. Evaluation Assets
4. Mindmaps
5. Checklists
6. Performance Tracking Assets
```

---

## 1. Training Plan Format

Training plans define what a recruit should learn, in what order, and how progress should be reviewed.

```markdown
# Training Plan: [Role / Cohort / Team]

## Purpose

[Why this training plan exists]

## Audience

[Who this plan is for]

## Timeline

[Training duration or phase]

## Learning Goals

- [Goal]
- [Goal]
- [Goal]

## Required Learning Assets

| Asset | Location | Required / Optional | Notes |
|---|---|---|---|
| [Asset Name] | [Path or link] | [Required / Optional] | [Notes] |

## Weekly / Phase Plan

| Phase | Focus Area | Learning Assets | Expected Outcome |
|---|---|---|---|
| [Phase] | [Focus] | [Assets] | [Outcome] |

## Evaluation Points

- [Evaluation point]
- [Evaluation point]

## Completion Criteria

- [Criteria]
- [Criteria]

## Notes

[Internal notes]
```

---

## 2. Product Intelligence Asset Format

Product Intelligence assets explain product knowledge needed for onboarding.

These may reference S.Academy courses, videos, product documents, or learning material.

```markdown
# Product Intelligence Asset: [Product / Topic]

## Product

[Hayley / Halo / Helix / Other]

## Purpose

[Why this asset is needed for onboarding]

## Audience

[Who should use this asset]

## Learning Material

| Material | Type | Location |
|---|---|---|
| [Material Name] | [Course / Video / Doc / Checklist] | [Path or link] |

## Key Concepts

- [Concept]
- [Concept]
- [Concept]

## Related S.Academy Content

[Path or link to related S.Academy course or asset]

## Notes

[Internal notes]
```

---

## 3. Evaluation Asset Format

Evaluation assets define how recruits or teams will be assessed.

```markdown
# Evaluation Asset: [Evaluation Name]

## Purpose

[What this evaluation measures]

## Audience

[Who will be evaluated]

## Evaluation Type

[Quiz / Live Review / Assignment / Scorecard / Observation]

## Skills / Knowledge Areas Evaluated

- [Area]
- [Area]
- [Area]

## Evaluation Criteria

| Criteria | Description | Score / Status |
|---|---|---|
| [Criteria] | [Description] | [Score or Status] |

## Passing / Readiness Standard

[What counts as ready or complete]

## Feedback Format

[How feedback should be captured]

## Notes

[Internal notes]
```

---

## 4. Mindmap Format

Mindmaps show the learning path or concept relationships for new recruits.

```markdown
# Mindmap: [Mindmap Name]

## Purpose

[Why this mindmap exists]

## Audience

[Who should use this mindmap]

## Mindmap Link

[Cloudinary or Google Drive link if visual]

## Text Version

[Text outline of the mindmap]

## Related Assets

- [Asset path or link]
- [Asset path or link]

## Notes

[Internal notes]
```

---

## 5. Checklist Format

Checklists track completion of onboarding tasks.

```markdown
# Checklist: [Checklist Name]

## Purpose

[Why this checklist exists]

## Audience

[Who should use it]

## Checklist

[ ] Task
[ ] Task
[ ] Task

## Completion Owner

[Recruit / Manager / Trainer / Reviewer]

## Review Point

[When this should be reviewed]

## Notes

[Internal notes]
```

---

## 6. Performance Tracking Asset Format

Performance tracking assets help track goals, gaps, and refinement needs.

```markdown
# Performance Tracking Asset: [Asset Name]

## Purpose

[What this asset tracks]

## Audience

[Who this asset is for]

## Goals

| Goal | Target | Status | Notes |
|---|---|---|---|
| [Goal] | [Target] | [Status] | [Notes] |

## Gaps Identified

- [Gap]
- [Gap]

## Refinement Plan

| Gap | Action | Owner | Review Date |
|---|---|---|---|
| [Gap] | [Action] | [Owner] | [Date] |

## Notes

[Internal notes]
```

---

## Rules

`onboarding_intelligence` assets should:

- be role-specific or cohort-specific when needed
- connect training to evaluation
- connect evaluation to performance refinement
- link to S.Academy learning material where relevant
- avoid duplicating full course content if it already exists in S.Academy
- use Cloudinary or Google Drive links for videos, visuals, and mindmaps
- use clear file names with underscores

`onboarding_intelligence` assets should not:

- duplicate full S.Academy courses
- store unrelated HR documents
- include unsupported performance claims
- track sensitive employee issues without proper approval
- replace manager judgment or formal HR processes

---

## Completion Standard

An onboarding asset is complete when it clearly explains:

```text
Who it is for
What it helps them learn or complete
Which learning assets are required
How progress will be evaluated
What completion looks like
How gaps will be refined
```
