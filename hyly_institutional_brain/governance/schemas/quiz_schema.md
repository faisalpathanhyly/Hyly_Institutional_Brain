# Quiz Schema

## Purpose

This schema defines the standard format for quizzes, knowledge checks, chapter assessments, and course assessments used in S.Academy learning assets.

The schema ensures quiz content is structured, easy to review, and aligned with approved learning content.

---

## Quiz Types

```text
1. Knowledge Check
2. Chapter Assessment
3. Course Assessment
```

| Quiz Type | Purpose | Where It Appears |
|---|---|---|
| Knowledge Check | Confirms understanding of a subchapter or section | Inside a chapter file |
| Chapter Assessment | Evaluates understanding of a full chapter | End of chapter or question bank |
| Course Assessment | Evaluates understanding of the full course | Question bank or final assessment asset |

---

## 1. Knowledge Check

A knowledge check is a short question placed after a subchapter or key learning section.

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

- Keep the knowledge check close to the section it evaluates.
- Keep `Knowledge Check`, `Question`, options, and `Correct Answer` on separate lines.
- Keep each answer option on its own line.
- Include the correct answer with a short explanation.
- Do not merge the question, answer options, and correct answer into one paragraph.
- Do not turn the full knowledge check into a heading.

---

## 2. Chapter Assessment

A chapter assessment evaluates a learner's understanding of a full chapter.

### Standard Format

```markdown
## Chapter Assessment

| SL No. | Question | Answer | Type | Chapter | Subchapter |
|---|---|---|---|---|---|
| 1 | [Question] | [Answer] | [Type] | [Chapter] | [Subchapter] |
```

### Rules

- Questions should align with the approved chapter content.
- Each question should connect to a chapter or subchapter.
- Answers should be clear and not one-word unless the question requires it.
- Do not repeat the same question or context unnecessarily.
- Do not add questions that require knowledge outside the approved content.

---

## 3. Course Assessment

A course assessment evaluates the learner's understanding of the complete course.

### Standard Format

```markdown
## Course Assessment

| SL No. | Question | Answer | Type | Chapter | Subchapter |
|---|---|---|---|---|---|
| 1 | [Question] | [Answer] | [Type] | [Chapter] | [Subchapter] |
```

### Rules

- Course assessment questions should cover the course broadly.
- Questions should remain tied to approved course material.
- Do not invent external context.
- Do not duplicate chapter assessment questions unless reuse is intentional.

---

## Question Bank Standard

When questions are stored in a question bank, use this file:

```text
questions_and_answers/question_bank.md
```

### Standard Format

```markdown
# Question Bank

| SL No. | Question | Answer | Type | Chapter | Subchapter |
|---|---|---|---|---|---|
| 1 | [Question] | [Answer] | [Type] | [Chapter] | [Subchapter] |
```

---

## Required Columns

| Column | Purpose |
|---|---|
| `SL No.` | Sequential question number |
| `Question` | Learner-facing question |
| `Answer` | Expected answer or correct answer with explanation |
| `Type` | Question type or assessment type |
| `Chapter` | Chapter the question belongs to |
| `Subchapter` | Subchapter or topic the question belongs to |

---

## Question Types

Use the question type from the approved source when available.

Common types may include:

```text
Knowledge Check
Chapter Assessment
Course Assessment
Scenario-Based
Short Answer
Multiple Choice
```

---

## Answer Rules

Answers should:

```text
Be aligned with approved content
Be clear enough for evaluation
Include a short explanation when needed
Avoid unnecessary length
Avoid one-word answers unless appropriate
```

Answers should not:

```text
Introduce new unsupported claims
Invent examples
Add details not present in approved content
Contradict the course material
```

---

## Scenario-Based Questions

Scenario-based questions should test how the learner applies course content to a realistic situation.

### Rules

- Keep scenarios short.
- Make the situation relevant to the course.
- Do not make the question too long.
- Avoid repeating the same scenario across multiple questions.
- Keep the answer specific but not overly lengthy.

---

## Quiz Quality Checklist

```text
[ ] Questions align with approved course content
[ ] Answers are included
[ ] Answers are clear and reviewable
[ ] Question type is included
[ ] Chapter reference is included
[ ] Subchapter or topic reference is included
[ ] Questions are not duplicated
[ ] No unsupported information is added
[ ] No invented outcomes or claims are included
[ ] Markdown tables render cleanly
```

---

## Completion Standard

A quiz asset is complete when a reviewer can understand:

```text
What the question tests
Where the question belongs
What the expected answer is
Which chapter or subchapter it supports
Whether the question is aligned with approved content
```
