# Course Schema

## Purpose

This schema defines the standard structure for courses stored inside the S.Academy Git repository.

The schema applies to all courses regardless of topic. It does not define course content. It only defines how course content should be organized, formatted, and maintained so that humans, LLMs, and rendering systems can read courses consistently.

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

It helps classify the course without reading the full course content.

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
- Use the same cohort name used in the course source.
- Keep metadata factual and limited to course classification.

---

## 2. initial_message.md

The `initial_message.md` file contains the opening message shown to the learner before the course begins.

### Standard Format

```markdown
# Initial Message

[Course opening message]
```

### Rules

- Use this file only for the learner-facing course introduction.
- Do not add chapter content here.
- Do not add assessment questions here.

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
- Do not split one chapter across multiple files unless the course source already does that.

---

## 5. Chapter File Format

Each chapter file should follow this format:

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

## [Number].[Number] [Next Subchapter Title]

[Subchapter content]
```

---

## 6. Subchapter Standard

Each subchapter should contain the learning content for that section.

When a subchapter includes a video, the video should be followed by key takeaways.

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

- Each subchapter should end with a knowledge check.
- If a video is included, place the video link inside the relevant subchapter.
- A video should be accompanied by key takeaways.
- If an image is included, place the image link where the visual belongs in the subchapter.
- Do not move media links into unrelated sections.

---

## 7. Media Placeholder

Media should not be uploaded directly into the course folder unless required later.

Videos and images should be uploaded to Cloudinary or Google Drive, and the link should be added in the relevant media placeholder.

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
- Do not replace media links with descriptions only.
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

Each subchapter should end with a knowledge check.

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

### Rules

- Keep `Knowledge Check`, `Question`, options, and `Correct Answer` on separate lines.
- Keep each answer option on its own line.
- Do not turn the full knowledge check into a heading.
- Do not merge the question, options, and answer into one paragraph.

---

## 10. Chapter Assessment

Each chapter should end with assessment questions.

Assessment questions may be stored at the end of the chapter file or in the course question bank, depending on how the course is maintained.

If assessments are stored in the chapter file, use this format:

```markdown
## Chapter Assessment

| SL No. | Question | Answer | Type | Chapter | Subchapter |
|---|---|---|---|---|---|
| 1 | [Question] | [Answer] | [Type] | [Chapter] | [Subchapter] |
```

If assessments are stored in the question bank, the chapter file should still end after the final subchapter knowledge check, and the full assessment should be maintained in:

```text
questions_and_answers/question_bank.md
```

---

## 11. questions_and_answers/question_bank.md

The `question_bank.md` file stores the full course assessment bank.

### Standard Format

```markdown
# Question Bank

| SL No. | Question | Answer | Type | Chapter | Subchapter |
|---|---|---|---|---|---|
| 1 | [Question] | [Answer] | [Type] | [Chapter] | [Subchapter] |
```

### Rules

- Preserve the approved assessment sequence.
- Keep one row per question.
- Keep the answer in the answer column.
- Keep the question type, chapter, and subchapter references.
- Do not mix question bank rows with in-chapter knowledge checks.

---

## 12. Tables

Tables should use standard Markdown table format.

### Standard Format

```markdown
| Column 1 | Column 2 | Column 3 |
|---|---|---|
| Value | Value | Value |
```

### Rules

- Keep table columns aligned with the approved source.
- Keep row order unchanged.
- Do not place media links inside table rows unless the source table does so.

---

## 13. Course Completion Checklist

Before a course is considered complete, confirm that it includes:

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
[ ] each subchapter ends with a knowledge check
[ ] chapter assessment questions are included
[ ] no approved content is removed
[ ] no new course content is invented
[ ] GitHub preview renders cleanly
```

---

## 14. Migration Rule

Course migration should follow this rule:

```text
Approved Course Source → Git Markdown Course
```

The Git version should preserve the approved course structure and content as closely as Markdown allows.

Do not rewrite, summarize, expand, or compress course content during migration.
