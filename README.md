# LinkedIn Profile Optimization Assistant

[![Antigravity Native](https://img.shields.io/badge/Antigravity-Native-4285F4?logo=google&logoColor=white)](https://antigravity.google)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Privacy: 100% Local](https://img.shields.io/badge/Privacy-100%25%20Local-brightgreen.svg)]()

An AI-powered assistant that gives your LinkedIn profile a complete, executive-grade makeover. 

It helps you **get found by recruiters**, highlights your strongest career achievements, and **sounds 100% human**—with zero robotic AI clichés.

---

## ⚡ The Problem: Why 99% of AI LinkedIn Rewrites Fail

When you ask ChatGPT or generic AI to write your LinkedIn profile, the results usually backfire:

1. **The "Robot Sound" Trap**: Generic AI loves clichés like *"passionate visionary"*, *"spearheaded"*, *"delve"*, and dramatic phrasing (*"Not just a data analyst, but a strategic partner..."*). Hiring managers spot AI-written profiles instantly and skip them.
2. **Invisible to Recruiters**: AI often invents fancy job titles that corporate recruiters never actually search for, or invents skills that don't match LinkedIn’s official search filters.
3. **Floating, Disconnected Skills**: Most tools dump a random list of 50 skills without connecting them to your real jobs, making your experience look unverified.
4. **Outdated 50-Skill Cap**: LinkedIn updated its platform to support up to **100 skills**, but most AI tools still stop at 50, missing half of your search potential.

---

## 🏗️ The Solution: A Step-by-Step 4-Phase Makeover

Instead of dumping a generic wall of text, this assistant builds your profile in 4 clear, logical phases:

* **Phase 1: Solid Proof & Foundation**  
  Crafts your **Headline**, **About** summary, **Work Experience** bullets, and **Projects** using real numbers and achievements—matching the exact keywords recruiters search for.
* **Phase 2: Complete 100-Skill Bank**  
  Identifies up to 100 relevant skills and links each one directly to your past roles, giving you official LinkedIn "Used in: [Role]" credibility badges.
* **Phase 3: Featured Visual Showcase**  
  Recommends the best presentations, portfolio links, or PDF decks to pin to the top of your profile so visitors stay and engage.
* **Phase 4: Targeted Recommendations**  
  Provides pre-drafted, 2–3 sentence endorsement templates you can send to past managers, peers, or mentors to build social proof.

---

## 🛡️ Core Innovations: Why It Actually Works

* 🔒 **Strict Approval Gates (Zero Hallucination)**: The assistant will never run ahead, guess, or invent things you never did. It writes **one section at a time** and pauses. It literally cannot proceed until you review the text and explicitly reply **"I approve"**.
* ✍️ **100% Human Writing Standard**: Every sentence is checked against an anti-AI style filter to ensure it sounds like an articulate, confident professional, not a machine.
* 🧪 **Battle-Tested on a Real Case Study**: This entire workflow isn't theoretical. It was refined through a real-world case study on the creator, capturing platform quirks, edge cases, and hard-won lessons learned (documented in [`PROCESS_LOGS.md`](./references/PROCESS_LOGS.md)).
* 📏 **Formatted for LinkedIn's Exact Limits**: Every headline (220 characters), summary (2,600 characters), and bullet is measured to prevent awkward cutoffs on mobile and desktop.

---

## 🚀 How to Install & Use

### 1. Add the Skill to Antigravity (One-Time Setup)
Choose the method that is easiest for you:

* **Method A: Just Ask the AI in Chat (Easiest)**  
  Open Antigravity or Antigravity IDE, open a chat in your workspace, and say:
  > *"Please install the skill from `https://github.com/SpiderPig107/linkedin-profile-optimization` into my workspace."*  
  Antigravity will automatically download and set it up for you.

* **Method B: Download & Drag-and-Drop**  
  1. Click the green **`< > Code`** button at the top of this GitHub page and select **Download ZIP**.
  2. Unzip the file.
  3. Move the `linkedin-profile-optimization` folder into your project workspace under `.agents/skills/`.

---

### 2. Start Your LinkedIn Makeover
Once installed, open a conversation in Antigravity:
* **Option A:** Type `/linkedin-profile-optimize` in the chat.
* **Option B:** Or simply ask:  
  > *"Help me optimize my LinkedIn profile for [Target Role, e.g. Strategy Manager or Data Analyst] positions."*

---

### 3. Share Your Background
* Drop your current resume (PDF or Word) directly into the chat, or paste your career history.

---

### 4. Review & Approve Step-by-Step
* The assistant will guide you through each section of your profile one at a time.
* For each section, it explains the strategy and how it helps you get noticed.
* **You stay in full control:** The assistant will only move to the next section when you explicitly say **"I approve"**.

---

### 5. Copy and Paste into LinkedIn
* When finished, the assistant creates a clean cheat sheet that you simply copy and paste straight into your LinkedIn profile!

---

## 📁 Repository Structure

Here is what is included in this repository and what each file does:

```text
linkedin-profile-optimization/
├── SKILL.md                        # The core instruction engine that guides the AI assistant
├── README.md                       # This guide (overview, setup, and instructions)
├── LICENSE                         # MIT License (free to use and adapt)
├── .gitignore                      # Privacy shield: prevents your personal resume and profile data from being uploaded to GitHub
└── references/
    ├── SIGNS_OF_AI_WRITING.md      # Anti-AI style guide (rules that ensure the writing sounds 100% human)
    └── PROCESS_LOGS.md             # Real-world case study: lessons learned and LinkedIn platform quirks
```

---

## 🔒 Privacy & Data Safety

* **100% Private to You**: Your resume and career history are never uploaded to any public database, tracker, or external server.
* **Local Storage**: When using Antigravity, all generated profile copy is saved locally on your own computer.
* **Safe & Code-Free**: This tool contains no executable programs or background scripts—it operates purely as a guided AI assistant.

---

## 🌐 Using on Other Platforms (ChatGPT / Claude)

While built natively for Antigravity, you can also use this assistant on other AI platforms:

* **ChatGPT**: Open [`SKILL.md`](./SKILL.md), copy the text, and paste it into a Custom GPT's Instructions (or directly into your chat alongside your resume).
* **Claude**: Create a Claude Project, upload [`SKILL.md`](./SKILL.md) to Project Knowledge, and start a conversation.

---

## 💻 Developer / Command Line Setup (Optional)

For technical users who prefer using Git in the terminal:

```bash
# Install to current workspace
mkdir -p .agents/skills
git clone https://github.com/SpiderPig107/linkedin-profile-optimization.git .agents/skills/linkedin-profile-optimization

# Or install globally across all workspaces
mkdir -p ~/.gemini/config/skills
git clone https://github.com/SpiderPig107/linkedin-profile-optimization.git ~/.gemini/config/skills/linkedin-profile-optimization
```

---

## 📄 License

Distributed under the [MIT License](./LICENSE). Free for individual job seekers, professionals, career coaches, and open-source contributors.
