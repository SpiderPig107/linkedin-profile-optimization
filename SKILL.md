---
name: linkedin-profile-optimization
description: >-
  Recruiter-grade LinkedIn profile optimization, SEO keyword architecture, and conversion-engineered rewriting for high-impact roles. Use this skill whenever the user types /linkedin-profile-optimize, or asks to audit, rewrite, or optimize a LinkedIn profile.
---

# LinkedIn Profile Optimization Skill (`linkedin-profile-optimization`)

This skill transforms any professional's LinkedIn profile into a recruiter-magnified, proof-backed, and conversion-optimized career asset. It treats a LinkedIn profile not as an online resume, but as an **information architecture of hard proof**.

---

## Stage 1: Intake & Cross-Cutting Competency Diagnostic

Before generating any profile text, the agent must diagnose the intersection between the candidate's real-world history and the target hiring market.

### Step 1.1: Background Intake & Verbatim Persistence
Prompt the user to provide their raw background:
> *"Welcome! Let's optimize your LinkedIn profile to pass recruiter filters and land interviews. To begin, please drop your existing CV / resume (PDF, DOCX, or paste text), or paste your downloaded LinkedIn profile data in the workspace."*

**STRICT VERBATIM PARSING & ANTI-HALLUCINATION PROTOCOL:**
1. **Zero Fabrication:** Extract ONLY verified facts, metrics, job titles, degrees, and tools explicitly written in the source text. Do NOT embellish, assume, or extrapolate unstated tools or methodologies.
2. **Missing Data Flagging:** If dates, metrics, or credentials are omitted in the source, label them explicitly as `[Not specified in source — confirm with user]`. Never invent numbers, dates, or placeholders.
3. **Comprehensive 12-Section Surface Area Audit:** Ensure extraction spans all sections: Headline, About, Experience, Education, Licenses & Certifications, Projects, Publications, Honors & Awards, Volunteering, Languages, Recommendations, and Top 5 Pinned Skills.
4. **Write to Disk:** Save the extracted data into `LINKEDIN_PROFILE_DATA.md` in the user's workspace.
5. **Verification Gate:** Present the file to the user and mandate confirmation:
   > *"I have extracted your background verbatim into `LINKEDIN_PROFILE_DATA.md`. Please review this file to confirm that all metrics, dates, and titles are 100% accurate before we proceed."*

### Step 1.2: Target Roles & Job Descriptions Intake
Prompt the user to provide their target market:
> *"What roles are you aiming for? Please share:*
> * 2–4 target job titles (e.g., Strategy & Operations Analyst, Product Operations Manager)
> * Target industries, sectors, or companies
> * Links to or text from 1–2 target job descriptions (optional, but highly recommended)"*

*Resilient Multi-Channel Ingestion Protocol:* If an ATS or corporate career link blocks automated fetching (e.g., 403 bot walls on Workday, Tesla, or SPA portals), immediately fall back to live targeted web search or ask the user to paste the raw text to prevent stalls.

### Step 1.2b: Interactive Clarification Protocol (Adaptive Sequential Inquiry)
Whenever clarifying background gaps, industry nuances, core professional philosophy, or personal priorities:
* **Strictly One Question at a Time:** Never dump a batch of open-ended questions.
* **Multiple Choice with Write-In:** Provide calibrated multiple-choice options (A, B, C) paired with an explicit write-in option (D).
* **Adaptive Dynamic Branching:** Incorporate the answer from Question N before formulating Question N+1.

### Step 1.3: Common Themes & Cross-Cutting Competency Analysis
Deconstruct the target roles and identify the convergence across the job descriptions:
1. **Core Technical & Hard Competencies:** High-frequency tools, quantitative methods, and domain workflows demanded across the target roles.
2. **Strategic & Operational Competencies:** Cross-functional leadership, stakeholder management, problem-solving frameworks, and commercial acumen.
3. **The Market Gap / Skepticism:** The primary doubt or filter recruiters will apply to candidates applying for these roles (e.g., *"Is this person purely technical without commercial sense?"* or *"Is this person a high-level generalist without quantitative depth?"*).

Present this analysis to the user as a clear **Competency Convergence Matrix**.

### Step 1.4: Strategic Archetype Synthesis & Selection
Synthesize 2–3 distinct **Positioning Archetypes** based on how the candidate's specific background meets those target competencies:
* **Archetype 1 (Specialist Focus A):** Maximizes vertical depth in the candidate's primary domain.
* **Archetype 2 (Specialist Focus B):** Maximizes execution capability in the secondary or technical domain.
* **Archetype 3 (The Balanced Hybrid):** Positions the candidate as a rare, high-leverage "translator" bridging both worlds.

For each archetype, provide:
* The core narrative hook.
* Target recruiters/roles it attracts.
* Strategic trade-offs (pros and cons).

> **SELECTION GATE:** The agent must ask: *"Which positioning archetype aligns best with your target career goals?"* and wait for the user's choice before proceeding.

---

## Stage 2: Recruiter SEO Blueprint & Keyword Architecture

Once the archetype is locked, build the custom SEO keyword matrix:
1. **Standard Recruiter Title Taxonomy:** Select 2–3 standard LinkedIn Recruiter search titles. Prohibit invented or composite titles (e.g. *"Quantitative Strategy"* is an algorithmic hedge fund title, not a corporate strategy title).
2. **Boolean Filter Keywords:** 10–15 high-frequency hard skills and domain methodologies.
3. **Skills-to-Proof Mapping Matrix:** Every target skill must be mapped to a concrete source node (Work Experience, Degree, Certification, Project, or Award). No orphaned or unverified skills.

> **GATE:** Present the SEO blueprint and request explicit approval before drafting copy.

---

## Stage 3: The 4-Phase Production Rewrites (Strict Sequential Gating)

LinkedIn profiles have hard architectural dependencies—you cannot aggregate or curate what has not yet been built. The agent must strictly execute in 4 sequential phases:

```
Phase 1: Proof-Building (Tasks 4.1 – 4.6)
  │
  ▼
Phase 2: Master Aggregation & 100-Skill Capacity (Task 4.7)
  │
  ▼
Phase 3: Curated Featured Showcase (Task 4.8)
  │
  ▼
Phase 4: Zero-Friction Social Proof (Task 4.9)
```

> **THE STRICT EXPLICIT APPROVAL PROTOCOL:**
> The agent MUST NOT advance to the next section or sub-task unless the user explicitly provides the phrase **"I approve"** or **"I approved"**.
> 
> If the user provides adjustments, questions, or commentary without explicit approval words, incorporate the changes, present the revised copy, and explicitly prompt for approval before advancing.

---

### Phase 1: Proof-Building (Tasks 4.1 – 4.6)

#### Task 4.1: Headline Optimization
* Deliver 2–3 calibrated variations under 220 characters.
* Formula: `[Standardized Target Titles] | [Domain Focus & Methodology] | [High-Impact Differentiator or Credential]`.

#### Task 4.2: About Section (Story & Value Proposition)
* **Target Length:** 1,800–2,100 characters (optimal for mobile scannability and SEO keyword density).
* **Structure:**
  1. **The Authentic Personal Philosophy Hook:** Analyze the CV and LinkedIn profile data to understand the candidate's genuine trajectory and problem-solving mindset. If their core motivation or professional philosophy is unclear, ask a targeted clarifying question (using the Step 1.2b adaptive protocol). Craft a 2–3 sentence opening that articulates their distinctive professional philosophy and approach—avoiding corporate clichés, generic buzzwords, or rigid templates.
  2. Core Commercial Value Proposition.
  3. Symmetric Proof Bullets (explicitly matching the Top 5 Pinned Skills).
  4. Technical Toolkit & Domain Methodology.
  5. Location, Open-to-Work parameters, and Contact/Portfolio links.
* **SEO-Safe Visual Formatting & Unicode Ban:** Strictly ban third-party Unicode bold/italic generators (e.g. YayText). They break screen readers, accessibility, and search indexing. Use native LinkedIn bold or search-safe ALL-CAPS headers (`• STRATEGY & OPS:`).

#### Task 4.3: Experience Section
For every position, provide:
1. **Respect Proven Candidate Phrasing:** If the candidate provides polished, battle-tested accomplishment bullets, do NOT gratuitously reword them. Preserve authentic wording, injecting only standardized taxonomy terms, missing tools, or metrics where needed.
2. **Formula:** `[Action Verb] + [Context/Problem] + [Methodology/Tool] + [Quantified Metric/Impact]`.
3. **Atomic Position Skills (3–5 per role):** Recommend standard auto-complete terms recognized in LinkedIn's taxonomy (e.g. `Strategy`, `Business Operations`, never composite unstandardized phrases).
4. **Multi-Project Media Discovery:** For positions covering multiple distinct client engagements or workstreams, probe for public reports, broadcast links, or deliverables across *each distinct engagement stream*, not just the overall company entry. Provide exact copy-paste Title and Description with candidate-level attribution.

#### Task 4.4: Education & Certifications
* Structure each degree: Institution, Degree Name, Field of Study, Dates, Honors/Grades.
* **Consortia Rule:** For multi-university joint programs (e.g. Erasmus Mundus), map the `School` field to the lead degree-awarding institution and detail mobility universities in the description.
* Tag 3–5 atomic skills per degree and certification.

#### Task 4.5: Standalone Projects
* Structure each project: Problem Statement, Technical Architecture & Models, Key Finding/Impact.
* Tag 4–5 atomic skills per project to establish downstream skill verification.

#### Task 4.6: Supporting Sections
* Publications (Title, Publisher, URL, description — note: LinkedIn does not support skills tagging on Publications).
* Honors & Awards, Volunteering, and Languages.

---

### Phase 2: Master Aggregation & 100-Skill Capacity (Task 4.7)

1. **Harvest Upstream Skills:** Aggregate all skills tagged across Experience, Education, Certifications, and Projects. (This generates the high-trust LinkedIn badge: *"Used in: [Role X], [Degree Y], [Project Z]"*).
2. **Backfill up to 100 Skills:** Fully utilize LinkedIn's modern 100-skill ceiling (abandoning outdated 50-skill pruning). Fill remaining slots with verified hard skills and keywords.
3. **Categorize:** Group skills into LinkedIn's native buckets (*Industry Knowledge*, *Tools & Technologies*, *Interpersonal Skills*).
4. **Lock Top 5 Pinned Skills:** Select the 5 highest-converting role anchors for the intro card widget, maintaining 1:1 symmetry with the About section.

---

### Phase 3: Portfolio Curation (Task 4.8 - Featured Section)

Before recommending cards, the agent must explicitly answer:
1. **The Target Perception:** What exact cognitive takeaway must the recruiter have in 5 seconds? (e.g., *"An undeniable, commercially grounded Operator-Builder"*).
2. **The Strategic "Why":** Explain which hiring manager doubts are being dismantled (e.g., de-risking the hire, proving 50/50 symmetry, killing the generalist bias).

#### The 5-Card Multi-Format Sensory Rhythm:
* **Position 1 (Native Interactive PDF):** Prioritize an uploaded PDF slide deck (e.g., Thesis defense slides or project pitch). LinkedIn renders PDFs as flippable slide carousels directly inside the profile viewport, preventing external link bounce rates.
* **Position 2 (Video Demo):** Playable video thumbnail showing live software/product execution.
* **Position 3 (Press / Broadcast Link):** External media validating large-scale commercial or public impact with transparent candidate attribution.
* **Position 4 (Code / Quantitative Repository):** Technical GitHub repo demonstrating math, clean code, and tests.
* **Position 5 (Award / Credential):** Objective third-party competition or brand validation.

---

### Phase 4: External Validation (Task 4.9 - Recommendations)

Provide a zero-friction outreach playbook:
* Target 3 diverse recommenders (e.g., Former Manager, Academic Advisor, Peer/Teammate).
* For each recommender, provide:
  1. A low-pressure outreach message specifying the shared milestone.
  2. A **ghostwritten 2–3 sentence template** ready for them to edit or paste in 60 seconds.

---

## 4. Universal Rules & Quality Standards

1. **Anti-AI Writing Style Mandate (Wikipedia Standard):** All recommended text MUST strictly comply with the accompanying [references/SIGNS_OF_AI_WRITING.md](./references/SIGNS_OF_AI_WRITING.md) style guide. Strictly prohibit:
   * *Negative Parallelisms:* Zero "not just X, but also Y", "not X, but Y", or "Y rather than X" structures.
   * *AI Vocabulary:* Zero "delve", "tapestry", "pivotal", "beacon", "testament", "spearhead", "foster", "holistic", "seamless", "vibrant".
   * *Avoidance of Copulatives:* Zero inflated purple verbs ("serves as", "stands as", "marks a" instead of "is" or "achieved").
   * *Robotic Triplets:* Break the compulsive rule-of-three list pattern.
   * *Outline Conclusions:* Zero generic future-looking essays ("As the industry evolves..."); replace with concrete, professional CTAs.
2. **Strict Neutral Point of View & Tone:** Write in clear, active, confident prose. Let hard numbers, verified awards, and validated project outcomes carry the prestige.
3. **Label Inflation Prevention (The "Tier-1" Trap):** Strictly ban inflated prestige labels. In corporate and consulting hiring, "Tier-1" exclusively denotes MBB (McKinsey, BCG, Bain); using it for boutique firms or internships triggers immediate hiring manager skepticism. Use accurate terms like *"Management Consulting"* or *"Strategy & Transformation Advisory"* and let quantified commercial results carry the prestige.
4. **The Defensibility Rule:** Never recommend or feature any project, technical tool, or claim that the candidate cannot confidently defend for 10 straight minutes under technical interview scrutiny. Distinguish classical econometrics/statistics (ARIMA, TBATS, regressions) from Machine Learning. Ground every tool in candidate reality.
5. **Permanent Output Artifact:** Write all final copy-paste outputs into `LINKEDIN_PROFILE_REWRITES.md` in the user's workspace.
6. **Reference Knowledge Base:** For edge cases and historical platform quirks, consult [references/PROCESS_LOGS.md](./references/PROCESS_LOGS.md). For writing standards, consult [references/SIGNS_OF_AI_WRITING.md](./references/SIGNS_OF_AI_WRITING.md).

