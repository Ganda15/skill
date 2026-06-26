# CV Power Scan

Use this reference when the user gives a CV and wants analysis, suggestions, a stronger CV, or comparison with a job offer for AI Developer, Agentic AI Developer, LLM, RAG, Data/AI, or junior AI consultant roles.

## Modes

Choose the smallest mode that satisfies the request:

1. Quick Scan: identify strengths, weak sections, missing keywords, and top fixes.
2. Full Rewrite: produce a complete ATS-safe CV proposal.
3. Job Match: compare the CV against one job offer and tailor the CV to that offer.
4. Skill Gap Plan: suggest which AI/agentic skills to learn, prove in projects, or add only after confirmation.
5. LinkedIn Alignment: make LinkedIn headline, About, Skills, and Featured section consistent with the CV.
6. Application Pack: produce cover letter angle, recruiter message, and follow-up after the CV is tailored.
7. Power Option: combine this skill with a dedicated resume or ATS skill if the user asks for an extra specialist pass.

## Option Menu To Offer

When the user's request is broad, offer these concise options:

```text
1. Quick CV scan
2. Full rewritten CV
3. CV + job offer match
4. Missing skills and project proof plan
5. LinkedIn + CV alignment
6. Cover letter and recruiter message
7. Power ATS second pass
```

If the user gives both a CV and a job offer, default to option 3 unless they ask for something narrower.

## Inputs

Ask only for missing inputs that materially change the result:

- current CV text or file;
- target role: AI Developer, Agentic AI Developer, LLM/RAG Developer, AI Solutions Developer, Data/AI Developer, Junior AI Consultant;
- contract type: internship, apprenticeship, junior job, freelance, CDI, remote/hybrid/on-site;
- target country, language, and availability;
- job offer text if the user wants matching;
- proof links: GitHub, portfolio, LinkedIn, deployed app, notebooks, screenshots, demos;
- true project details: problem, stack, action, output, metrics, learning.

If the CV is weak or incomplete, still produce a useful scan. Mark assumptions clearly and ask for exact details before inventing metrics.

## Scan Workflow

1. Extract facts from the CV:
   - target title;
   - education and certifications;
   - technical stack;
   - AI, LLM, RAG, agentic AI, MLOps, and software proof;
   - projects and outcomes;
   - work experience and transferable skills;
   - languages, location, availability, links.

2. Diagnose fit for the target:
   - role clarity;
   - keyword coverage;
   - proof strength;
   - ATS readability;
   - recruiter readability;
   - project credibility;
   - gaps for the target role.

3. Separate three lists:
   - Verified: already proven in the CV.
   - Missing but likely: ask the user to confirm before adding.
   - Missing and risky: do not add unless the user provides proof.

4. Recommend improvements:
   - stronger title;
   - sharper summary;
   - reordered sections;
   - better project bullets;
   - grouped technical skills;
   - old experience translated into transferable value;
   - keywords to add only when true;
   - missing proof to create through a portfolio project.

5. Rewrite the CV if requested:
   - ATS-safe text;
   - one target title;
   - 3 to 5 line summary;
   - grouped skills;
   - project bullets using action + stack + purpose + result;
   - experience bullets using context + action + tool/method + result;
   - no fake numbers or inflated seniority.

## Job Offer Match Workflow

When a job offer is included, create a compact comparison before rewriting:

| Job requirement | Evidence in CV | Gap | CV action |
| --- | --- | --- | --- |
| Python / API | Project uses Python and API calls | Needs clearer API result | Add one bullet with action, stack, purpose |
| RAG / vector search | RAG project mentioned | Missing evaluation detail | Add retrieval/evaluation wording if true |
| Docker / deployment | Not visible | Confirm if used | Do not add unless confirmed |

Then produce:

- match score from 0 to 100 with a short rationale;
- must-add keywords from the offer, only if honest;
- missing requirements to learn or prove;
- tailored CV title and summary;
- rewritten project and experience bullets;
- optional cover letter angle.

## Skill Gap Plan

When the user asks what skills to add, separate the answer into:

- Learn next: skills needed for the target role but not yet proven.
- Prove next: small projects, tests, demos, or GitHub evidence that can validate the skill.
- Add now: skills already supported by the CV or user-provided proof.
- Do not claim yet: keywords that would be risky without evidence.

Example:

| Skill | Status | Proof action |
| --- | --- | --- |
| RAG | likely | Add project bullet only if the user built retrieval with embeddings |
| Docker | missing | Build and document a simple containerized FastAPI demo |
| Agent evals | prove next | Create 10 test cases and compare agent outputs |

## Scoring Rubric

Use scores to guide improvement, not to discourage the user:

- 90-100: strong match; minor tailoring needed.
- 75-89: credible match; add sharper evidence and keywords.
- 60-74: possible match; projects or skills need clearer proof.
- 40-59: stretch role; build missing proof before applying.
- 0-39: poor match; choose a closer role or create new evidence.

Score dimensions:

- Target clarity: 15 points.
- Technical keyword coverage: 20 points.
- AI/LLM/RAG/agent proof: 25 points.
- Software engineering readiness: 15 points.
- ATS and structure: 10 points.
- Recruiter readability: 10 points.
- Honest fit with job offer: 5 points.

## Agentic AI / AI Developer Signals

Look for proof of:

- Python, APIs, Git, SQL, FastAPI or Streamlit;
- OpenAI API or Anthropic API;
- prompt engineering and structured outputs;
- embeddings, vector search, RAG, citations;
- tool calling, function calling, workflows, memory, guardrails;
- evaluation, tests, hallucination checks, monitoring;
- Docker, CI/CD basics, deployment, documentation;
- business use case: automation, internal assistant, document search, workflow optimization.

Do not add advanced terms if the CV gives no proof. Suggest them as learning or project gaps instead.

## Output Templates

### CV Analysis

Use this structure:

1. Target read: what role the CV currently suggests.
2. Strengths: 3 to 6 bullets.
3. Risks: 3 to 6 bullets.
4. Missing AI/agentic signals: grouped by must-have and nice-to-have.
5. ATS fixes: structure, titles, keywords, formatting.
6. Project fixes: better bullets and missing proof.
7. Suggested skills to learn or prove next.
8. Rewritten CV sections or full CV, depending on the request.
9. Optional next proof plan: 3 practical actions to strengthen the CV.

### Rewritten CV

Use this structure:

```text
NAME
Target title | Location | Phone | Email | LinkedIn | GitHub

PROFESSIONAL SUMMARY
3 to 5 lines focused on target role, stack, proof, and availability.

TECHNICAL SKILLS
AI / LLM:
RAG / Search:
Backend / APIs:
Data:
Tools / DevOps:

AI PROJECTS
Project name
- Bullet with action + stack + purpose + result.
- Bullet with evaluation, documentation, or learning.

EXPERIENCE
Role - Company | Dates
- Transferable bullet.

EDUCATION

CERTIFICATIONS

LANGUAGES
```

## Optional External Skill Pass

If the user explicitly asks to search for a resume/CV skill or wants an extra ATS specialist pass, use the skills ecosystem before finalizing.

Suggested search commands:

```bash
npx skills find "resume ats job match"
npx skills find "cv analysis"
```

At the time this workflow was created, a strong public option was:

```bash
npx skills add paramchoudhary/resumeskills@resume-ats-optimizer -g -y
```

Use that kind of external skill as a second-pass checker, not as a replacement for this skill's Agentic AI / AI Developer positioning. Verify current install count and quality before recommending installation.
