# Guide - How This Skill Works

This repository contains a reusable AI agent skill for improving career materials for AI and Agentic AI roles.

The French version is presented first because this repository is mainly used for French CV, LinkedIn, and job-search workflows.

## 1. Repository Structure

```text
skill/
|-- README.md
|-- GUIDE.md
|-- ai-career-linkedin-growth-fr/
|   |-- SKILL.md
|   |-- agents/
|   |   `-- openai.yaml
|   `-- references/
|       |-- ai-keyword-bank.md
|       |-- checklists.md
|       |-- content-playbook.md
|       |-- cv-application-playbook.md
|       |-- cv-power-scan.md
|       |-- profile-playbook.md
|       `-- source-notes.md
`-- ai-career-linkedin-growth/
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

## 2. Skill Versions

### French: `ai-career-linkedin-growth-fr`

Use this version first for French requests.

Example:

```text
Utilise $ai-career-linkedin-growth-fr pour analyser mon CV de Developpeur IA Agentique et le comparer avec cette offre.
```

Install:

```bash
npx skills add https://github.com/ganda15/skill --skill ai-career-linkedin-growth-fr
```

### English: `ai-career-linkedin-growth`

Use this version for English requests.

Example:

```text
Use $ai-career-linkedin-growth to analyze my AI Developer CV and compare it with this job offer.
```

Install:

```bash
npx skills add https://github.com/ganda15/skill --skill ai-career-linkedin-growth
```

## 3. What Each File Does

### `SKILL.md`

This is the main instruction file for each skill version.

It tells an AI assistant:

- when to use the skill;
- what the skill is designed to do;
- which workflow to follow;
- which reference file to open depending on the task.

### `agents/openai.yaml`

This file contains interface metadata:

- display name;
- short description;
- default prompt.

The main logic stays in `SKILL.md`.

### `references/`

The `references` folder contains detailed playbooks loaded only when needed.

This keeps `SKILL.md` short and makes the skill easier to maintain.

## 4. Reference Files

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

The currently cited source documents/reference families are:

1. `Atelier TRE-2026_Profil en ligne & LinkedIn.pptx.pdf`, June 2026 Wild Code School & Simplon workshop PDF supplied by the user.
2. Skills.sh and public career reference sources for skill structure, ATS CV guidance, LinkedIn content, copywriting, and job applications.

## 5. Main Options

The skill has seven main options:

1. Quick CV Scan: strengths, risks, missing keywords, ATS fixes.
2. Full CV Rewrite: complete ATS-safe CV proposal.
3. Job Offer Match: CV-to-offer comparison and tailored rewrite.
4. Skill Gap Plan: what to learn, prove, add now, or avoid claiming.
5. LinkedIn Alignment: headline, About, experience, skills, Featured section.
6. Application Pack: cover letter, recruiter message, follow-up.
7. Content And Visibility: LinkedIn posts, comments, watch routine.

If the user asks for a "power option" or an extra ATS checker, search the skills ecosystem first and use a dedicated resume/ATS skill only as a second-pass checker. The main AI Developer and Agentic AI positioning should still come from this skill.

## 6. Recommended Workflow

French CV request:

```text
Analyse mon CV pour un poste de Developpeur IA Agentique et compare-le avec cette offre.
```

Recommended assistant workflow:

1. Read `ai-career-linkedin-growth-fr/SKILL.md`.
2. Open `references/cv-power-scan.md`.
3. Open `references/ai-keyword-bank.md`.
4. If application wording is needed, open `references/cv-application-playbook.md`.
5. Extract verified proof from the CV.
6. Compare the CV with the job offer when provided.
7. Return a diagnosis, missing skills, honest keyword suggestions, and a rewritten CV proposal.

French LinkedIn request:

```text
Ameliore mon profil LinkedIn pour une alternance Developpeur IA.
```

Recommended assistant workflow:

1. Read `ai-career-linkedin-growth-fr/SKILL.md`.
2. Identify the task type: LinkedIn profile optimization.
3. Open `references/profile-playbook.md`.
4. Open `references/ai-keyword-bank.md`.
5. Ask for missing user information if needed.
6. Generate headline options, About section, skills, and Featured recommendations.
7. Add networking notes, target-profile benchmarking, or watch actions when useful.
8. Use `references/checklists.md` to verify the result.

English CV request:

```text
Analyze my CV for an Agentic AI Developer role and compare it with this job offer.
```

Use the same workflow with `ai-career-linkedin-growth/SKILL.md`.

## 7. Main Use Cases

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

## 8. Contribution Workflow

Do not commit directly to `main` for larger changes. Use branches and pull requests.

Recommended workflow:

```bash
git clone https://github.com/ganda15/skill.git
cd skill
git checkout -b improve-cv-playbook
```

Make changes, then commit:

```bash
git add .
git commit -m "Improve CV playbook"
git push origin improve-cv-playbook
```

Then open a pull request:

```text
base branch: main
compare branch: improve-cv-playbook
```

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
- direct edits to `main` for substantial changes.

## 10. Review Checklist

Before merging a pull request, check:

- Does the change help AI job seekers?
- Is it specific to CV, LinkedIn, job search, or AI career positioning?
- Is the advice honest and not exaggerated?
- Does it keep the skill easy to use?
- Are examples clear and reusable?
- Is `SKILL.md` still concise?
- Are detailed examples placed in `references/` instead of bloating `SKILL.md`?
