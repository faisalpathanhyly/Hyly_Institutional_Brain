# Video Schema

## Purpose

This schema defines the standard format for documenting learning videos used in S.Academy.

Videos may be acquired from the Growth team and used across courses, client intelligence, onboarding, product learning, or other learning assets.

Videos should be uploaded to Cloudinary or Google Drive. Git should store the video metadata, context, and link, not the video file itself.

---

## Standard Video Asset Format

```markdown
# Video Asset: [Video Title]

## Video Details

**Video Title:** [Title]  
**Source Team:** Growth Team  
**Product / Domain:** [Hayley / Halo / Helix / Multifamily / Client Intelligence]  
**Video Type:** [Explainer / Demo / Training / Client Story / Walkthrough]  
**Status:** [Draft / Approved / Needs Review]  
**Video Link:** [Cloudinary or Google Drive link]  

## Purpose

[Why this video exists and what learning need it supports.]

## Learning Context

[Where this video should be used: course chapter, client proof story, pre-pilot asset, onboarding module, etc.]

## Key Takeaways

- [Takeaway 1]
- [Takeaway 2]
- [Takeaway 3]

## Related Asset

**Course / Story / Knowledge Asset:** [Name or path]  
**Related Chapter or Section:** [If applicable]

## Review Notes

[Internal notes, missing captions, approval needs, update needs.]

## Usage Rules

- Do not upload video files directly into Git.
- Store only Cloudinary or Google Drive links.
- Each video should have a clear learning purpose.
- Each video should include key takeaways.
- Do not use outdated videos without review.
```

---

## Video Details

| Field | Purpose |
|---|---|
| `Video Title` | Official or working title of the video |
| `Source Team` | Team providing the video |
| `Product / Domain` | Product or knowledge domain the video supports |
| `Video Type` | Type of learning video |
| `Status` | Current review or approval status |
| `Video Link` | Cloudinary or Google Drive link |

---

## Source Team

If the video is acquired from the Growth team, use:

```text
Growth Team
```

If another team provides a video later, use the actual source team name.

---

## Product / Domain

Use the product or domain the video supports.

Examples:

```text
Hayley
Halo
Helix
Multifamily Industry Intelligence
Client Intelligence
Partner Integrations Intelligence
```

---

## Video Type

Use a clear video type.

Examples:

```text
Explainer
Demo
Training
Client Story
Walkthrough
```

---

## Status

Use a simple status.

Examples:

```text
Draft
Approved
Needs Review
```

Do not mark a video as approved unless it has been reviewed.

---

## Video Link Rules

Videos should be uploaded to:

```text
Cloudinary
Google Drive
```

The Git file should include only the video link.

### Standard Link Format

```markdown
**Video Link:** [Cloudinary or Google Drive link]
```

### Rules

- Keep the video link on its own line.
- Do not upload large video files directly into Git.
- Do not use broken or private links without noting access limitations.
- Replace outdated links only after confirming the updated video source.

---

## Purpose

The purpose section explains why the video exists.

It should answer:

```text
What learning need does this video support?
```

---

## Learning Context

The learning context explains where the video should be used.

Examples:

```text
Course chapter
Subchapter
Client Proof Story
Pre-Pilot Client Knowledge Asset
Onboarding module
Product training asset
```

If the video belongs to a course section, include the course and chapter path.

---

## Key Takeaways

Every learning video should include key takeaways.

### Standard Format

```markdown
## Key Takeaways

- [Takeaway 1]
- [Takeaway 2]
- [Takeaway 3]
```

### Rules

- Keep takeaways tied to the actual video.
- Do not add new product claims not supported by the video.
- Keep takeaways short and useful for learners.

---

## Related Asset

Use this section to connect the video to the learning asset it supports.

### Standard Format

```markdown
## Related Asset

**Course / Story / Knowledge Asset:** [Name or path]  
**Related Chapter or Section:** [If applicable]
```

---

## Review Notes

Use review notes for internal context.

Examples:

```text
Needs captions
Needs transcript
Needs updated product screen
Approved for internal use only
Replace after new Growth version is available
```

---

## Video Quality Checklist

```text
[ ] Video title is included
[ ] Source team is included
[ ] Product or domain is included
[ ] Video type is included
[ ] Status is included
[ ] Cloudinary or Google Drive link is included
[ ] Purpose is clear
[ ] Learning context is clear
[ ] Key takeaways are included
[ ] Related asset is linked if applicable
[ ] Review notes are included if needed
[ ] Git does not contain the actual video file
```

---

## Completion Standard

A video asset is complete when someone can understand:

```text
What the video is about
Where the video came from
Where the video should be used
Which product or domain it supports
What learners should take away
Whether the video is approved or needs review
Where the video file is stored
```
