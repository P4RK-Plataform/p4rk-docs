# Issue Writing Standards

> **Status:** Active
> **Last updated:** 2026-03-27
> **Applies to:** All P4RK-Plataform repositories

---

## Overview

Every issue in P4RK follows a strict template based on its **Item Type**: Epic, Story, or Task. Consistent formatting ensures that any contributor can quickly understand scope, intent, and progress of any item on the board.

---

## 1. Epic Template

Epics are **large feature areas** that group multiple Stories. They represent a major deliverable or system component.

```markdown
## Epic

[1-2 sentence description of the feature area and its purpose in the platform.]

## Stories

- [ ] [Story title 1]
- [ ] [Story title 2]
- [ ] [Story title 3]
```

### Rules

| Rule | Detail |
|------|--------|
| **Title** | `Epic: [Feature Area]` — use a noun phrase |
| **Heading** | Always starts with `## Epic` |
| **Description** | 1-2 sentences. What is this feature area and why does it matter? |
| **Stories list** | Checkbox list of all child Stories. Updated as Stories are added |
| **No implementation detail** | Epics describe *what*, never *how* |
| **Labels** | Must have `epic` label |

### Example

> **Title:** `Epic: Infrastructure & DevOps`

```markdown
## Epic

Set up the complete development infrastructure: CI/CD pipelines,
containerization, orchestration, and environment configuration.

## Stories

- [ ] Docker environment setup
- [ ] CI/CD Pipeline with GitHub Actions
- [ ] Rancher and orchestration setup
```

---

## 2. Story Template

Stories are **user-facing deliverables** written in user-story format. They describe *who* needs *what* and *why*.

```markdown
## Story

As a [role], I want [capability], so that [benefit].

## Acceptance Criteria

- [Criterion 1]
- [Criterion 2]
- [Criterion 3]
```

### Rules

| Rule | Detail |
|------|--------|
| **Title** | `Story: [Deliverable]` — start with a verb (Set up, Implement, Add, Build) |
| **Heading** | Always starts with `## Story` |
| **User story** | Must follow "As a... I want... so that..." format |
| **Acceptance Criteria** | Bullet list (not checkboxes). Each criterion is testable and specific |
| **No implementation detail** | Stories describe *what the user gets*, not *how to build it* |
| **Labels** | Must have `story` label |

### Example

> **Title:** `Story: Set up GitHub Actions CI pipeline`

```markdown
## Story

As a developer, I want a CI pipeline that automatically builds and tests
the code on every PR, so we catch issues before merging.

## Acceptance Criteria

- Pipeline triggers on PR to main/develop
- Builds .NET solution
- Runs unit tests
- Reports build status on PR
```

---

## 3. Task Template

Tasks are **daily work items** scoped to ~3 hours. They describe a concrete, actionable piece of work.

```markdown
## Task

[Concrete description of what to do. Reference specific files, commands,
or configurations. Should be actionable without further clarification.]

## Estimate: ~Xh
```

### Rules

| Rule | Detail |
|------|--------|
| **Title** | `Task: [Action]` — start with a verb (Create, Configure, Implement, Write, Add) |
| **Heading** | Always starts with `## Task` |
| **Description** | Concrete and specific. Mention file names, tools, commands. A developer should be able to start working immediately after reading this |
| **Estimate** | Always present. Format: `## Estimate: ~Xh`. Tasks should be 1-3h. If more than 3h, split into multiple tasks |
| **No user-story format** | Tasks are technical, not user-facing |
| **Labels** | Must have `task` label |

### Example

> **Title:** `Task: Configure GitHub Actions workflow for .NET build`

```markdown
## Task

Create `.github/workflows/ci.yml` that triggers on PR, checks out code,
sets up .NET SDK, restores packages, and builds the solution.

## Estimate: ~3h
```

---

## 4. Title Conventions

All issue titles MUST be prefixed with their Item Type using **consistent casing**:

| Type | Title Format | Example |
|------|-------------|---------|
| Epic | `Epic: [Feature Area]` | `Epic: Infrastructure & DevOps` |
| Story | `Story: [Deliverable]` | `Story: Set up GitHub Actions CI pipeline` |
| Task | `Task: [Action]` | `Task: Configure GitHub Actions workflow for .NET build` |

### Title Rules

- **Consistent casing** — always `Epic:`, `Story:`, `Task:` (title case, never ALL CAPS)
- **Max 70 characters** (excluding prefix)
- **Start with a verb** for Stories and Tasks (Set up, Create, Configure, Implement, Add)
- **Use nouns** for Epics (Infrastructure, Auth Context, Memory Module)
- **No redundancy** — don't repeat the Epic name in Story/Task titles

---

## 5. Hierarchy Rules

```
Epic
 └── Story (sub-issue of Epic)
      └── Task (sub-issue of Story)
```

| Rule | Detail |
|------|--------|
| Every Story must be a **sub-issue** of exactly one Epic | Use GitHub's native sub-issues feature |
| Every Task must be a **sub-issue** of exactly one Story | |
| Epics list their Stories as **checkboxes** in the body | Manually maintained |
| Stories do NOT list their Tasks in the body | Sub-issue panel handles this |

---

## 6. Field Requirements (Project Board)

Every issue on the project board must have ALL of these fields set:

| Field | Required Values |
|-------|----------------|
| **Status** | Backlog / To Do / In Progress / Review / Done |
| **Epic** | One of the defined Epics |
| **Priority** | Critical / High / Medium / Low |
| **Item Type** | Epic / Story / Task |
| **Estimate (hours)** | Number (Epics = sum of children; Stories = sum of tasks; Tasks = 1-3) |
| **Sprint** | Assigned sprint |

---

## 7. Writing Quality Checklist

Before submitting any issue, verify:

- [ ] Title follows the prefix convention (`Epic:` / `Story:` / `Task:`)
- [ ] Casing is consistent (title case prefix, never ALL CAPS)
- [ ] Body uses the correct template for its type
- [ ] Epics have a Stories checkbox list
- [ ] Stories use "As a... I want... so that..." format
- [ ] Stories have testable Acceptance Criteria
- [ ] Tasks are concrete and actionable (mention files, tools, commands)
- [ ] Tasks have an estimate of 1-3h
- [ ] All project board fields are set
- [ ] Sub-issue link is established (Story → Epic, Task → Story)
- [ ] Correct labels are applied

---

> *"A well-written issue is half the work done."*
