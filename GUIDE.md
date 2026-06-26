# Guide - How This Skill Works

This repository contains a reusable AI agent skill for improving career materials for AI and Agentic AI roles.

The skill can be used by compatible AI agents or coding assistants that support skill-style workflows, such as Claude, Codex, Cursor, Gemini CLI, OpenCode, or other tools that can read a `SKILL.md` file and supporting Markdown references.

## 1. Repository Structure

```text
skill/
├── README.md
├── GUIDE.md
└── ai-career-linkedin-growth/
    ├── SKILL.md
    ├── agents/
    │   └── openai.yaml
    └── references/
        ├── ai-keyword-bank.md
        ├── checklists.md
        ├── content-playbook.md
        ├── cv-application-playbook.md
        ├── profile-playbook.md
        └── source-notes.md
```

## 2. What Each File Does

### `README.md`

This file introduces the repository.

It explains:

- what the skill is for;
- how to install it;
- the main use cases.

### `ai-career-linkedin-growth/SKILL.md`

This is the main instruction file.

It tells an AI assistant:

- when to use the skill;
- what the skill is designed to do;
- which workflow to follow;
- which reference file to open depending on the task.

For example, if a user asks:

```text
Improve my LinkedIn profile for an Agentic AI Developer internship.
```

The assistant should use the skill because the task is about LinkedIn, employability, and AI developer positioning.

### `agents/openai.yaml`

This file contains interface metadata.

It can be used by AI tools that display skills in a UI.

It defines:

- display name;
- short description;
- default prompt.

This file is not the main knowledge base. The main logic is in `SKILL.md`.

### `references/`

The `references` folder contains detailed playbooks.

These files are loaded only when needed.

This keeps `SKILL.md` short and makes the skill easier to maintain.

## 3. Reference Files

### `profile-playbook.md`

Use this file for LinkedIn profile work.

It covers:

- online image cleanup;
- visibility and search behavior;
- headline;
- About section;
- experience;
- education;
- skills;
- recommendations;
- featured section;
- connection notes;
- profile benchmarking;
- visual profile advice.

### `cv-application-playbook.md`

Use this file for CVs, cover letters, and job applications.

It covers:

- ATS-friendly CV structure;
- project bullets;
- experience bullets;
- cover letter structure;
- recruiter messages;
- follow-up messages;
- weekly job search routine.

### `content-playbook.md`

Use this file for LinkedIn posts and content strategy.

It covers:

- post hooks;
- post structure;
- project posts;
- technical lessons;
- job search posts;
- comment strategy;
- watch routine;
- posting cadence.

### `ai-keyword-bank.md`

Use this file for AI and Agentic AI keywords.

It includes:

- AI Developer titles;
- Agentic AI vocabulary;
- LLM keywords;
- RAG keywords;
- MLOps / LLMOps keywords;
- business and product keywords;
- soft skills for AI roles.

### `checklists.md`

Use this file before finalizing outputs.

It checks:

- LinkedIn profile quality;
- CV quality;
- cover letter quality;
- LinkedIn post quality;
- common anti-patterns.

### `source-notes.md`

This file explains where the guidance came from.

It includes:

- workshop advice;
- public career and LinkedIn guidance;
- skills ecosystem references.

## 4. How The Skill Works Step By Step

Example user request:

```text
Help me improve my LinkedIn profile for an AI Developer apprenticeship.
```

Recommended assistant workflow:

1. Read `SKILL.md`.
2. Identify the task type: LinkedIn profile optimization.
3. Open `references/profile-playbook.md`.
4. Open `references/ai-keyword-bank.md`.
5. Ask for missing user information if needed.
6. Generate headline options, About section, skills, and Featured recommendations.
7. Add networking notes, target-profile benchmarking, or watch actions when useful.
8. Use `references/checklists.md` to verify the result.
9. Return text that the user can paste directly into LinkedIn.

## 5. Main Use Cases

This skill is useful for:

- improving a LinkedIn headline;
- writing a LinkedIn About section;
- optimizing a CV for AI Developer roles;
- writing a cover letter;
- creating recruiter messages;
- preparing LinkedIn posts;
- planning a job search routine;
- choosing AI / LLM / RAG / MLOps keywords;
- positioning a junior or transitioning profile toward Agentic AI.

## 6. Installation

If your AI tool supports the Skills CLI, install with:

```bash
npx skills add https://github.com/ganda15/skill --skill ai-career-linkedin-growth
```

If your tool does not support the Skills CLI, you can still use the skill manually:

1. Download or clone the repository.
2. Open `ai-career-linkedin-growth/SKILL.md`.
3. Give that file to your AI assistant as instructions.
4. Add the relevant reference files depending on the task.

## 7. How To Contribute Without Touching `main`

Do not commit directly to the `main` branch.

Use branches and pull requests.

Recommended workflow:

```bash
git clone https://github.com/ganda15/skill.git
cd skill
git checkout -b improve-linkedin-playbook
```

Make your changes, then commit:

```bash
git add .
git commit -m "Improve LinkedIn profile playbook"
git push origin improve-linkedin-playbook
```

Then open a pull request on GitHub:

```text
base branch: main
compare branch: improve-linkedin-playbook
```

The maintainer can review the pull request and merge it only if the changes are good.

## 8. Suggested Contribution Rules

Good contributions:

- improve clarity;
- add useful examples;
- add realistic AI Developer keywords;
- improve checklists;
- correct mistakes;
- add better recruiter message templates;
- add more LinkedIn post examples.

Avoid:

- generic motivational advice;
- fake metrics;
- unsupported claims;
- spammy LinkedIn tactics;
- changes that make the skill too long or hard to use;
- direct edits to `main`.

## 9. Recommended Branch Names

Use clear branch names:

```text
improve-cv-playbook
add-agentic-ai-keywords
fix-cover-letter-template
add-linkedin-post-examples
update-checklists
```

## 10. Review Checklist

Before merging a pull request, check:

- Does the change help AI job seekers?
- Is it specific to CV, LinkedIn, job search, or AI career positioning?
- Is the advice honest and not exaggerated?
- Does it keep the skill easy to use?
- Are examples clear and reusable?
- Is `SKILL.md` still concise?
- Are detailed examples placed in `references/` instead of bloating `SKILL.md`?
