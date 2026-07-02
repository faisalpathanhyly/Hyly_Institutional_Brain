# Course Schema

## Purpose

This schema defines the standard structure for courses stored in the Hyly Institutional Brain and consumed by S.Academy.

The schema applies to courses across knowledge domains. It does not define the course topic or course content. It only defines how approved course content should be organized, formatted, linked, and maintained.

---

## Standard Course Folder Structure

Each course should follow this structure:

```text
course_name/
├── meta.json
├── initial_message.md
├── table_of_contents.md
├── chapters/
│   ├── chapter_1_title.md
│   ├── chapter_2_title.md
│   └── chapter_n_title.md
└── questions_and_answers/
    └── question_bank.md
```

---

## 1. meta.json

The `meta.json` file stores course-level information.

### Standard Format

```json
{
  "course_id": "",
  "course_title": "",
  "course_type": "course",
  "status": "",
  "cohort": "",
  "knowledge_domain": "",
  "last_updated": ""
}
```

### Rules

- Use underscores in `course_id`.
- Keep the course title aligned with the approved course name.
- Use the same cohort name used in the approved course source.
- Keep metadata factual and limited to course classification.

---

## 2. initial_message.md

The `initial_message.md` file contains the learner-facing opening message.

### Standard Format

```markdown
# Initial Message

[Course opening message]
```

### Rules

- Use this file only for the learner-facing course introduction.
- Do not add chapter content here.
- Do not add quiz or assessment questions here.

---

## 3. table_of_contents.md

The `table_of_contents.md` file defines the course sequence.

### Standard Format

```markdown
# Table of Contents

## Chapter 1: [Chapter Title]

1.1 [Subchapter Title]  
1.2 [Subchapter Title]  
1.3 [Subchapter Title]  

**Evaluation and Feedback on Chapter 1**

---

## Chapter 2: [Chapter Title]

2.1 [Subchapter Title]  
2.2 [Subchapter Title]  

**Evaluation and Feedback on Chapter 2**
```

### Rules

- Keep chapters in the approved course order.
- Keep subchapters in the approved course order.
- Keep each chapter and subchapter on a separate line.
- Include evaluation or feedback references only if the course uses them.

---

## 4. chapters/

The `chapters/` folder contains one Markdown file per chapter.

### Naming Format

```text
chapter_1_title.md
chapter_2_title.md
chapter_3_title.md
```

### Rules

- Use one file per chapter.
- Use underscores in file names.
- Do not combine multiple chapters into one file.
- Do not split one chapter across multiple files unless the approved course source already does that.

---

## 5. Chapter File Format

Each chapter file should follow this structure:

```markdown
# Chapter [Number]: [Chapter Title]

## [Number].[Number] [Subchapter Title]

[Subchapter content]

#### [Number].[Number].[Number] [Media or Topic Title]

[Media link placeholder]

### Key Takeaways

- [Key takeaway]
- [Key takeaway]
- [Key takeaway]

**Knowledge Check:**

**Question:** [Question text]

A. [Option A]  
B. [Option B]  
C. [Option C]  
D. [Option D]  

**Correct Answer:** [Correct answer with explanation]

---
```

---

## 6. Subchapter Standard

Each subchapter should contain the learning content for that section.

### Standard Subchapter Flow

```text
Subchapter Title
↓
Content
↓
Media link, if applicable
↓
Key Takeaways
↓
Knowledge Check
```

### Rules

- Each subchapter should end with a knowledge check when applicable.
- If a video is included, place the video link inside the relevant subchapter.
- A video should be accompanied by key takeaways.
- If an image is included, place the image link where the visual belongs in the subchapter.
- Do not move media links into unrelated sections.

---

## 7. Media Placeholder

Media should not be uploaded directly into the course folder unless required later.

Videos and images should be uploaded to Cloudinary or Google Drive. The link should be added in the relevant media placeholder.

### Video Placeholder

```markdown
#### [Media Title]

[Cloudinary or Google Drive video link]
```

### Image Placeholder

```markdown
#### [Image or Diagram Title]

[Cloudinary or Google Drive image link]
```

### Rules

- Use Cloudinary or Google Drive links for videos and images.
- Place media links in the subchapter where they belong.
- Keep each media link on its own line.
- Do not place all media links at the end of the chapter.

---

## 8. Key Takeaways

Key takeaways summarize the important points from the related video, image, or subchapter.

### Standard Format

```markdown
### Key Takeaways

- [Takeaway 1]
- [Takeaway 2]
- [Takeaway 3]
```

### Rules

- Place key takeaways after the related video or section content.
- Keep takeaways directly connected to the subchapter.
- Do not use key takeaways to introduce new content.

---

## 9. Knowledge Check

Each subchapter should end with a knowledge check when the course design includes checks at the subchapter level.

### Standard Format

```markdown
**Knowledge Check:**

**Question:** [Question text]

A. [Option A]  
B. [Option B]  
C. [Option C]  
D. [Option D]  

**Correct Answer:** [Correct answer with explanation]
```

---

## 10. Chapter Assessment

Each chapter should end with assessment questions.

Assessment questions may be stored at the end of the chapter file or in the course question bank, depending on how the course is maintained.

```markdown
## Chapter Assessment

| SL No. | Question | Answer | Type | Chapter | Subchapter |
|---|---|---|---|---|---|
| 1 | [Question] | [Answer] | [Type] | [Chapter] | [Subchapter] |
```

If assessments are stored in the question bank, use:

```text
questions_and_answers/question_bank.md
```

---

## 11. Question Bank

The `question_bank.md` file stores the full course assessment bank.

### Standard Format

```markdown
# Question Bank

| SL No. | Question | Answer | Type | Chapter | Subchapter |
|---|---|---|---|---|---|
| 1 | [Question] | [Answer] | [Type] | [Chapter] | [Subchapter] |
```

---

## 12. Course Completion Checklist

```text
[ ] meta.json
[ ] initial_message.md
[ ] table_of_contents.md
[ ] chapters folder
[ ] one Markdown file per chapter
[ ] questions_and_answers folder
[ ] question_bank.md
[ ] all subchapters in order
[ ] all media links placed in the right section
[ ] all videos accompanied by key takeaways
[ ] each applicable subchapter ends with a knowledge check
[ ] chapter assessment questions are included
[ ] no approved content is removed
[ ] no new course content is invented
[ ] GitHub preview renders cleanly
```

---

## Migration Rule

```text
Approved Course Source -> Git Markdown Course
```

The Git version should preserve the approved course structure and content as closely as Markdown allows.

Do not rewrite, summarize, expand, or compress approved course content during migration.
