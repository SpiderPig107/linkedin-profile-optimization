# LinkedIn Profile Optimization Skill (`linkedin-profile-optimization`)

[![Antigravity Skill](https://img.shields.io/badge/Antigravity-Skill-4285F4?logo=google&logoColor=white)](https://antigravity.google)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Production Ready](https://img.shields.io/badge/Status-Production%20Ready-success.svg)]()
[![Security: Evaluated](https://img.shields.io/badge/Security-Evaluated%20%26%20Zero--Leak-brightgreen.svg)]()
[![LinkedIn Capacity](https://img.shields.io/badge/LinkedIn%20Capacity-100%20Skills-0A66C2?logo=linkedin&logoColor=white)]()

A recruiter-grade, conversion-engineered skill for **Antigravity**, **Antigravity IDE**, and agentic AI pair programmers. 

It transforms any professional's LinkedIn profile into an **information architecture of hard proof**—maximizing recruiter search visibility, passing automated Boolean filters, dismantling hiring manager skepticism, and eliminating every telltale sign of machine-generated prose.

---

## ⚡ The Problem: Why 99% of AI LinkedIn Rewrites Fail

Most LLMs generate catastrophic LinkedIn profile copy:
1. **The "AI Sound" Trap:** LLMs compulsively use theatrical negative parallelisms (*"Not just a data analyst, but a strategic partner..."*), purple copulatives (*"Stands as a testament to..."*), and statistical dead-giveaways (*"delve"*, *"tapestry"*, *"pivotal"*, *"beacon"*, *"spearhead"*). Hiring managers immediately recognize machine-generated text and dismiss the candidate.
2. **The Recruiter Taxonomy Mismatch:** Generic AI invents composite job titles (e.g. *"Quantitative Strategy Analyst"*) that corporate recruiters never search for, or invents composite skill tags that do not exist in LinkedIn's standardized atomic skill database.
3. **Premature Aggregation:** Standard AI tools dump a list of 50 skills without linking them to actual work, education, or projects, producing unverified floating keywords that fail algorithmic context weighting.
4. **Outdated Platform Limits:** Most tools still enforce an obsolete 50-skill cap, needlessly pruning 50% of the candidate's keyword surface area rather than utilizing LinkedIn's modern **100-skill ceiling**.

---

## 🏗️ The Solution: The 4-Phase Hard-Proof Architecture

This skill treats LinkedIn as an interconnected dependency graph. You cannot aggregate or curate what has not yet been anchored to proof:

```
Phase 1: Proof-Building (Tasks 4.1 – 4.6)
  │  • Headline (Standard Recruiter Taxonomy, <220 chars)
  │  • About Section (1,800–2,100 char sweet spot, 1:1 symmetry with Top 5)
  │  • Experience (Quantified metrics, atomic skills, multi-workstream media)
  │  • Education & Certs (Consortium rules, credential links)
  │  • Standalone Projects (Architecture, models, verified deliverables)
  │  • Supporting Sections (Publications, Honors, Languages)
  ▼
Phase 2: Master Aggregation & 100-Skill Capacity (Task 4.7)
  │  • Harvest upstream skills to generate "Used in: [Role X]" trust badges
  │  • Backfill remaining slots up to 100 skills using verified hard skills
  │  • Lock Top 5 Pinned Skills widget to mirror About section
  ▼
Phase 3: Curated Featured Showcase (Task 4.8)
  │  • Curate 3–5 sensory cards based on explicit cognitive perception goals
  │  • Mitigate bounce rates using native interactive PDF decks in Position 1
  ▼
Phase 4: Zero-Friction Social Proof (Task 4.9)
     • 3 targeted recommenders (Manager, Peer, Academic/Advisor)
     • Pre-drafted, ghostwritten 2–3 sentence endorsement copy
```

---

## 🛡️ Core Architectural Innovations

### 1. Strict Explicit Approval Loops (`"I approve"`)
The agent never hallucinates or races ahead. Rewrites are delivered **one section at a time**, accompanied by clear strategic rationale. The agent is hard-gated: it will not proceed to the next section until the user explicitly replies with **"I approve"** or **"I approved"**.

### 2. Anti-AI Writing Engine (Wikipedia Standard)
All suggested text is verified against the accompanying [SIGNS_OF_AI_WRITING.md](./references/SIGNS_OF_AI_WRITING.md) engine. It eliminates:
* **Negative parallelisms:** Zero *"not just X, but also Y"* or *"Y rather than X"*.
* **Purple copulatives:** Zero *"serves as"*, *"marks a"*, or *"stands as"*.
* **Robotic triplets:** Breaks rhythmic three-item list habits.
* **Outline conclusions:** Zero *"As the industry evolves..."* essays; strictly professional CTAs.

### 3. Recruiter Search Taxonomy vs. Atomic Skill Standardization
* **Job Titles:** Strictly aligned with standard LinkedIn Recruiter Boolean search taxonomy.
* **Skills:** Strictly aligned with LinkedIn's atomic autocomplete database (e.g. `Strategy` and `Business Operations` rather than non-standard composite phrases).

### 4. Resilient Multi-Channel Ingestion
Automated ATS scrapers frequently hit 403 bot walls or single-page apps (Workday, SuccessFactors, Tesla, etc.). The skill executes an automatic multi-channel fallback:
$$\text{URL Ingestion} \longrightarrow \text{Targeted Search Fallback} \longrightarrow \text{Direct User Paste}$$

### 5. Adaptive Sequential Inquiry (No Question Dumps)
Background clarification is conducted **strictly one question at a time** using structured multiple-choice options (A, B, C) paired with an open write-in fallback (D).

---

## 🔒 Security, Privacy & Safety Evaluation

This skill has undergone a rigorous security and privacy evaluation aligned with the **OWASP Top 10 for Large Language Model Applications**:

* **Zero Data Exfiltration (100% Local Execution):** The skill contains zero external API calls, tracking scripts, webhooks, or telemetry. All extracted candidate data and generated profile drafts remain entirely on the user's local disk in `./LINKEDIN_PROFILE_DATA.md` and `./LINKEDIN_PROFILE_REWRITES.md`.
* **Zero Arbitrary Code Execution (Zero Attack Surface):** The repository contains **no executable code, bash scripts, or binaries** (0 `.py`, 0 `.js`, 0 `.sh`). It operates purely as an Antigravity prompt workflow, eliminating arbitrary code execution (ACE) risks.
* **Prompt Injection Resilience:** To mitigate untrusted ATS job postings or CV text containing hidden prompt injections (OWASP LLM01), the skill enforces:
  1. *Verbatim Entity Parsing:* Extracts factual entities (titles, tools, dates) while ignoring embedded instructional commands.
  2. *Hard Approval Gates:* Requires the explicit user phrase `"I approve"` before advancing, preventing runaway agent execution.
* **Supply Chain & Accidental Leak Prevention:** The included `.gitignore` strictly blocks personal career artifacts (`LINKEDIN_PROFILE_DATA.md`, `LINKEDIN_PROFILE_REWRITES.md`, `*.pdf`, `*.docx`, `*.csv`) from ever being committed to public version control.
* **Secret & Credential Cleanliness:** Verified zero hardcoded API keys, authorization tokens, or private filesystem paths.

---

## 📁 Repository Structure

```text
linkedin-profile-optimization/
├── SKILL.md                        # Core Antigravity skill instructions & prompt engine
├── README.md                       # Documentation & setup guide
├── LICENSE                         # MIT License
├── .gitignore                      # Prevents accidental commits of personal profile data
└── references/
    ├── SIGNS_OF_AI_WRITING.md      # Anti-AI style guide (Wikipedia writing standards)
    └── PROCESS_LOGS.md             # Battle-tested engineering logs, edge cases & platform quirks
```

---

## 🚀 Installation & Setup

### Option 1: Workspace Installation (Recommended)
To use this skill within a specific project or career workspace:

1. Clone or copy this repository into your workspace's `.agents/skills/` directory:
   ```bash
   mkdir -p .agents/skills
   git clone https://github.com/<your-username>/linkedin-profile-optimization.git .agents/skills/linkedin-profile-optimization
   ```
2. Open Antigravity or Antigravity IDE in your workspace. The skill will be automatically discovered.

### Option 2: Global Installation (All Workspaces)
To make this skill available across every project on your local machine:

```bash
mkdir -p ~/.gemini/config/skills
git clone https://github.com/<your-username>/linkedin-profile-optimization.git ~/.gemini/config/skills/linkedin-profile-optimization
```

---

## 💻 How to Use

1. Launch your Antigravity conversation and trigger the skill:
   * **Slash Command:** Type `/linkedin-profile-optimize`
   * **Natural Prompt:** *"Optimize my LinkedIn profile for Strategy & Operations and Data Analyst roles."*
2. Provide your raw background (drop your CV, PDF, DOCX, or paste LinkedIn export CSVs).
3. The agent will:
   * Extract your verified data verbatim into `LINKEDIN_PROFILE_DATA.md`.
   * Ask targeted clarification questions one-by-one.
   * Propose 2–3 target positioning archetypes and an SEO keyword blueprint.
   * Walk you through the 4-Phase build step-by-step, waiting for your `"I approve"` at each milestone.
   * Save all production copy directly to `LINKEDIN_PROFILE_REWRITES.md` for clean, zero-friction copy-pasting into LinkedIn.

---

## 📄 License

Distributed under the [MIT License](./LICENSE). Free for individual professionals, career coaches, and open-source contributors.
