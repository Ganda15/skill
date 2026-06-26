---
name: ai-career-linkedin-growth
description: Optimize CVs, LinkedIn profiles, LinkedIn posts, cover letters, recruiter messages, and job-search workflows for AI Developer, Agentic AI Developer, Data/AI Developer, junior AI consultant, internship, apprenticeship, and first-job searches. Use when the user wants to improve employability, profile positioning, recruiter visibility, personal branding, application materials, or content strategy for AI, Python, LLM, RAG, agentic workflows, OpenAI/Anthropic APIs, MLOps, and related roles.
---

# AI Career LinkedIn Growth

## Overview

Use this skill to turn a learner or junior AI profile into a credible job-search system: CV, LinkedIn profile, featured projects, posts, cover letters, outreach, and proof of skills.

Core principle:

> Be searchable, credible, specific, and proof-based. Do not sound generic, desperate, or like AI-generated marketing copy.

## Workflow

1. Identify the target: internship, apprenticeship, junior job, freelance, or portfolio visibility.
2. Extract the user's proof: projects, stack, training, certifications, experience, constraints, language, location, availability.
3. Build positioning: one clear professional title, one target role family, one proof-based narrative.
4. Optimize LinkedIn: online image, headline, About, Experience, Education, Skills, Featured, Recommendations, network, watch routine.
5. Optimize CV: ATS-safe structure, keywords, quantified bullets, technical stack, projects.
6. Create application assets: cover letter, recruiter message, follow-up, networking note.
7. Create content strategy: LinkedIn posts that show learning, projects, technical judgment, and human voice.
8. Run the checklist before finalizing.

## Reference Loading

Load only the reference needed for the task:

- `references/profile-playbook.md`: LinkedIn headline, About, sections, skills, recommendations.
- `references/cv-application-playbook.md`: CV, cover letter, recruiter message, job application strategy.
- `references/content-playbook.md`: LinkedIn post strategy, hooks, post templates, cadence.
- `references/ai-keyword-bank.md`: AI developer, Agentic AI, RAG, LLM, Python, MLOps keywords.
- `references/checklists.md`: final quality checks and anti-patterns.
- `references/source-notes.md`: source links and why they matter.

## Input To Ask For

Ask for missing information only when needed. Useful inputs:

- target role and contract: stage, alternance, CDI, freelance;
- location and availability;
- current CV or LinkedIn text;
- job description if tailoring an application;
- projects with stack, goal, result, links, screenshots;
- training, certifications, school, dates;
- languages and work authorization if relevant;
- preferred tone: French, English, bilingual, direct, warm, technical.

## Output Standards

Produce practical outputs the user can paste or publish:

- 3 to 7 headline options;
- polished About section;
- experience bullets using context + action + tools + result;
- skills list organized by category;
- Featured section recommendations;
- networking notes under 300 characters when connecting on LinkedIn;
- cover letter under 400 words unless requested otherwise;
- recruiter/networking messages under 900 characters;
- LinkedIn posts with clear hook, proof, lesson, and soft call to action;
- weekly action plan for job search when asked.

## Positioning Rules

Prefer precise titles over vague learner labels.

Avoid:

- "Stagiaire IA developer"
- "Dev IA junior"
- "En formation developpeur IA agentique a la recherche..."

Prefer:

- "Developpeur IA | Python, LLM, RAG, API"
- "Developpeur IA Agentique | Recherche alternance 12 mois"
- "Developpeur Python specialise IA | OpenAI API, RAG, MLOps"
- "Developpeur Data & IA | Integration de solutions IA"
- "Consultant Junior IA | Automatisation, RAG, agents LLM"

For users in transition, make the transition explicit but not dominant. Lead with the target role and proof, then mention training.

## LinkedIn Content Rules

For posts, optimize for authenticity and usefulness:

- write from real project experience;
- show the problem, the decision, the result, and the lesson;
- avoid generic "AI changed everything" content;
- avoid engagement bait;
- avoid sounding like a template;
- use AI to refine, not replace, the user's voice.

Good Agentic AI post themes:

- "What I learned building a RAG chatbot"
- "How I evaluate an LLM agent before deployment"
- "A simple MLOps loop for AI agents"
- "Mistake I made while using OpenAI API"
- "How I debugged hallucinations in a chatbot"
- "What agentic AI means in practice, not in hype"

## Recruiter Visibility Rules

Use keywords in multiple places, not only in Skills:

- headline;
- About first 3 lines;
- Experience bullets;
- Projects;
- Education description;
- Skills;
- Featured section captions.

Keywords must be honest. Do not claim production experience, deployment experience, or expertise unless the user has proof.

## Quality Bar

Before final answer, check:

- Does the headline say the target role clearly?
- Does the About section reassure both tech and AI sides?
- Are projects concrete enough to prove capability?
- Are technologies grouped logically?
- Are experience bullets action-oriented?
- Is the CV ATS-safe?
- Does the LinkedIn post sound human?
- Is there a clear next action for the user?

If the user asks to publish on GitHub, keep the skill folder clean. Do not add unrelated documentation. Ensure `SKILL.md`, `agents/openai.yaml`, and references are valid.
