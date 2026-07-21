# Chapter 5: Diligence + Three Modes of AI at Hyly

This chapter introduces the fourth D: **Diligence**. Diligence is about using AI responsibly.

## 5.1 What Diligence Means

### Watch: Diligence

https://res.cloudinary.com/dtlycu2wl/video/upload/v1777010862/Chapter_5__Diligence_hqaim6.mp4

**Diligence = Using AI responsibly — protecting data, being transparent about AI’s role, and owning everything you produce with AI.**

### Knowledge Check

**Question:** A teammate wants to paste client lead data into an AI tool to save time. What should they do first?

A. Check whether the data is safe to share and anonymize sensitive information before using AI.

B. Paste the data immediately because faster work is the main goal of AI.

C. Use any AI tool because all tools handle client data the same way.

D. Ask AI to decide whether the data is sensitive after pasting it.

**Correct Answer:** A — Check whether the data is safe to share and anonymize sensitive information before using AI, is correct because Creation Diligence requires safe data handling before using AI.

## 5.2 Creation, Transparency, and Deployment Diligence

https://res.cloudinary.com/dtlycu2wl/image/upload/v1776941480/ch5_diligence_triangle_qbd0f1.png

| Aspect | What It Means | Quick Test |
|---|---|---|
| **Creation Diligence** | Be thoughtful about which AI you use and what data you share | “Would I be comfortable if my manager saw what I just pasted into this tool?” |
| **Transparency Diligence** | Be honest about AI’s role in your work | “I used Claude to analyse trends, then applied my own judgment.” |
| **Deployment Diligence** | Own what you produce with AI | AI drafts it. You send it. If there is an error, you own it. |

### Knowledge Check

**Question:** You use Claude to analyze trends, then apply your own judgment before sharing the final recommendation. How should you describe AI’s role?

A. “Claude helped analyze the trends, and I reviewed the output before making the recommendation.”

B. “This recommendation came fully from me, and AI was not involved.”

C. “Claude made the decision, so I am not responsible for the recommendation.”

D. “AI created the answer, so no further explanation is needed.”

**Correct Answer:** A — “Claude helped analyze the trends, and I reviewed the output before making the recommendation,” is correct because Transparency Diligence means being honest about AI’s role while Deployment Diligence keeps ownership with the human.

## 5.3 Access Rules and Risk Questions

| Access Rule | Why It Exists | What Happens Without It |
|---|---|---|
| Read from QA Bug Tracker | Agent needs source data to do its job | Agent cannot function |
| Create one entry per bug in PM.Bugs | Agent’s core job is to map the bug | Duplicates flood the PM database |
| Link bi-directionally between databases | QA and PM teams need traceability | Orphaned records nobody can trace |
| Do not modify the QA Bug Tracker | Source of truth must stay untouched | Agent overwrites QA findings |
| Do not delete anything | Prevent accidental data loss | Active sprint items get wiped |
| Do not add AI commentary | Output structured data only | AI commentary misleads PMs |

### The 4 Big Access Questions

| Access Type | The Question | The Risk |
|---|---|---|
| **CRM Data** | When AI pulls lead data — names, emails, lease terms — what do I need to anonymise? | Resident PII in an external system |
| **Notion Database** | What scope did I set? Can AI read HR records or NDA-covered meeting transcripts? | Confidential data exposed to AI |
| **Delete Access** | Does this agent need delete permissions? Almost always: no. | One bad rule wipes active sprint items |
| **API Access** | What is the blast radius if this API call is wrong? | Wrong status update signals Sales that a feature is live when it is still in QA |

### Knowledge Check

**Question:** An AI agent only needs to read QA bugs and create linked PM.Bugs entries. Someone suggests giving it delete access “just in case.” What is the best response?

A. Do not give delete access unless the workflow truly requires it, because one bad rule could wipe important records.

B. Give delete access because more permissions always make agents more useful.

C. Give full access first and design guardrails after the workflow breaks.

D. Avoid access rules because they slow down AI adoption.

**Correct Answer:** A — Do not give delete access unless the workflow truly requires it, because one bad rule could wipe important records, is correct because access should be limited to what the workflow actually needs.

## 5.4 Three Modes of AI + 4D Monday Checklist

https://res.cloudinary.com/dtlycu2wl/image/upload/v1776941481/ch5_three_modes_nkhwnj.png

| Mode | What it means | Why it matters |
|---|---|---|
| **Automation** | AI handles repetitive tasks based on rules | Needs clear Delegation and Diligence |
| **Augmentation** | AI supports human work and improves output | Needs strong Description and Discernment |
| **Agency** | AI acts with more independence | Needs all 4Ds at a higher level |

https://res.cloudinary.com/dtlycu2wl/image/upload/v1776941480/ch5_diligence_throne_rhgxki.png

### Your 4D Monday Checklist

https://res.cloudinary.com/dtlycu2wl/image/upload/v1776941479/ch5_4d_monday_checklist_xfotq5.png

| D | Monday Checklist Question |
|---|---|
| Delegation | Should AI do this task? |
| Description | Have I explained what I need clearly? |
| Discernment | How will I check whether the output is good? |
| Diligence | Am I using AI responsibly and safely? |

### Knowledge Check

**Question:** A workflow moves from AI helping draft outputs to AI acting more independently across systems. What should increase as AI independence increases?

A. Guardrails, monitoring, human accountability, and use of all 4Ds should increase.

B. Human review should decrease because AI is now more advanced.

C. Description becomes unnecessary because the AI can act independently.

D. Diligence matters less because agency mode is more automated.

**Correct Answer:** A — Guardrails, monitoring, human accountability, and use of all 4Ds should increase, is correct because Agency mode needs the strongest guardrails as AI acts with more independence.
