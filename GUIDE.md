# Guide - How This Skill Works

This repository contains a reusable AI agent skill for improving career materials for AI and Agentic AI roles.

The skill can be used by compatible AI agents or coding assistants that support skill-style workflows, such as Claude, Codex, Cursor, Gemini CLI, OpenCode, or other tools that can read a `SKILL.md` file and supporting Markdown references.

## 1. Repository Structure

```text
skill/
|-- README.md
|-- GUIDE.md
|-- ai-career-linkedin-growth/
    |-- SKILL.md
    |-- agents/
    |   `-- openai.yaml
    `-- references/
        |-- ai-keyword-bank.md
        |-- checklists.md
        |-- content-playbook.md
        |-- cv-application-playbook.md
        |-- cv-power-scan.md
        |-- profile-playbook.md
        `-- source-notes.md
`-- ai-career-linkedin-growth-fr/
    |-- SKILL.md
    |-- agents/
    |   `-- openai.yaml
    `-- references/
        |-- ai-keyword-bank.md
        |-- checklists.md
        |-- content-playbook.md
        |-- cv-application-playbook.md
        |-- cv-power-scan.md
        |-- profile-playbook.md
        `-- source-notes.md
```

## 2. What Each File Does

### `README.md`

This file introduces the repository.

It explains:

- what the skill is for;
- how to install it;
- the main options;
- example prompts.

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

### `ai-career-linkedin-growth-fr/SKILL.md`

This is the French version of the same skill.

It uses the distinct skill name `ai-career-linkedin-growth-fr`, so both versions can live in the same repository without conflict.

For example, if a user asks:

```text
Analyse mon CV pour un poste de Développeur IA Agentique.
```

The assistant should use the French skill because the task is the same domain but the expected working language is French.

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
- visual profile advice;
- LinkedIn alignment with verified CV proof.

### `cv-application-playbook.md`

Use this file for CV wording, cover letters, recruiter messages, follow-ups, and job applications.

It covers:

- ATS-friendly CV structure;
- project bullets;
- experience bullets;
- cover letter structure;
- recruiter messages;
- follow-up messages;
- weekly job search routine.

### `cv-power-scan.md`

Use this file when the user gives a CV for analysis, asks for a stronger AI Developer or Agentic AI Developer CV, includes a job offer, or asks what skills to add next.

It covers:

- quick CV scan;
- full CV rewrite;
- ATS-style review;
- CV-to-job-offer comparison;
- skill-gap suggestions;
- LinkedIn and CV alignment;
- application pack support;
- optional external resume/ATS skill pass.

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
- posting cadence;
- content ideas from CV gaps.

### `ai-keyword-bank.md`

Use this file for AI and Agentic AI keywords.

It includes:

- AI Developer titles;
- Agentic AI vocabulary;
- LLM keywords;
- RAG keywords;
- MLOps / LLMOps keywords;
- business and product keywords;
- soft skills for AI roles;
- job-offer keyword mapping rules.

### `checklists.md`

Use this file before finalizing outputs.

It checks:

- LinkedIn profile quality;
- CV quality;
- selected mode quality;
- cover letter quality;
- LinkedIn post quality;
- common anti-patterns.

### `source-notes.md`

This file explains where the guidance came from.

It includes:

- workshop advice;
- public career and LinkedIn guidance;
- skills ecosystem references;
- caution about third-party ATS tools.

The currently cited source documents/reference families are:

1. `Atelier TRE-2026_Profil en ligne & LinkedIn.pptx.pdf`, June 2026 Wild Code School & Simplon workshop PDF supplied by the user.
2. Skills.sh and public career reference sources for skill structure, ATS CV guidance, LinkedIn content, copywriting, and job applications.

## 4. Main Options

The skill has seven main options:

1. Quick CV Scan: strengths, risks, missing keywords, ATS fixes.
2. Full CV Rewrite: complete ATS-safe CV proposal.
3. Job Offer Match: CV-to-offer comparison and tailored rewrite.
4. Skill Gap Plan: what to learn, prove, add now, or avoid claiming.
5. LinkedIn Alignment: headline, About, experience, skills, Featured section.
6. Application Pack: cover letter, recruiter message, follow-up.
7. Content And Visibility: LinkedIn posts, comments, watch routine.

If the user asks for a "power option" or an extra ATS checker, search the skills ecosystem first and use a dedicated resume/ATS skill only as a second-pass checker. The main AI Developer and Agentic AI positioning should still come from this skill.

## 5. How The Skill Works Step By Step

Example LinkedIn request:

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

Example CV request:

```text
Analyze my CV for an Agentic AI Developer role and compare it with this job offer.
```

Recommended assistant workflow:

1. Read `SKILL.md`.
2. Open `references/cv-power-scan.md`.
3. Open `references/ai-keyword-bank.md`.
4. If application wording is needed, open `references/cv-application-playbook.md`.
5. Extract verified proof from the CV.
6. Compare the CV with the job offer when provided.
7. Return a diagnosis, missing skills, honest keyword suggestions, and a rewritten CV proposal.

Example application pack request:

```text
Use my tailored CV and this job offer to write a cover letter and recruiter message.
```

Recommended assistant workflow:

1. Open `references/cv-power-scan.md` if the CV was not already compared with the offer.
2. Open `references/cv-application-playbook.md`.
3. Extract the role title, company need, and strongest CV proof.
4. Produce a short cover letter, recruiter message, and follow-up.
5. Check the output with `references/checklists.md`.

## 6. Main Use Cases

This skill is useful for:

- improving a LinkedIn headline;
- writing a LinkedIn About section;
- optimizing a CV for AI Developer roles;
- scanning any CV for AI Developer / Agentic AI Developer fit;
- comparing a CV with a job offer;
- proposing a rewritten CV;
- finding missing skills and project proof ideas;
- writing a cover letter;
- creating recruiter messages;
- preparing LinkedIn posts;
- planning a job search routine;
- choosing AI / LLM / RAG / MLOps keywords;
- positioning a junior or transitioning profile toward Agentic AI.

## 7. Installation

If your AI tool supports the Skills CLI, install the English version with:

```bash
npx skills add https://github.com/ganda15/skill --skill ai-career-linkedin-growth
```

Install the French version with:

```bash
npx skills add https://github.com/ganda15/skill --skill ai-career-linkedin-growth-fr
```

If your tool does not support the Skills CLI, you can still use the skill manually:

1. Download or clone the repository.
2. Open `ai-career-linkedin-growth/SKILL.md` for English or `ai-career-linkedin-growth-fr/SKILL.md` for French.
3. Give that file to your AI assistant as instructions.
4. Add the relevant reference files depending on the task.

## 8. How To Contribute Without Touching `main`

Do not commit directly to the `main` branch.

Use branches and pull requests.

Recommended workflow:

```bash
git clone https://github.com/ganda15/skill.git
cd skill
git checkout -b improve-cv-playbook
```

Make your changes, then commit:

```bash
git add .
git commit -m "Improve CV playbook"
git push origin improve-cv-playbook
```

Then open a pull request on GitHub:

```text
base branch: main
compare branch: improve-cv-playbook
```

The maintainer can review the pull request and merge it only if the changes are good.

## 9. Suggested Contribution Rules

Good contributions:

- improve clarity;
- add useful examples;
- add realistic AI Developer keywords;
- improve CV scan and job-offer matching;
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

## 10. Recommended Branch Names

Use clear branch names:

```text
improve-cv-playbook
add-french-skill-version
add-agentic-ai-keywords
fix-cover-letter-template
add-linkedin-post-examples
update-checklists
```

## 11. Review Checklist

Before merging a pull request, check:

- Does the change help AI job seekers?
- Is it specific to CV, LinkedIn, job search, or AI career positioning?
- Is the advice honest and not exaggerated?
- Does it keep the skill easy to use?
- Are examples clear and reusable?
- Is `SKILL.md` still concise?
- Are detailed examples placed in `references/` instead of bloating `SKILL.md`?
