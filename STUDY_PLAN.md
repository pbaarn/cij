# Dynamics 365 Customer Insights – Journeys: Antigravity Study Plan

This study plan is tailored to working in `/Users/paulbaarn/code/CI` alongside your interactive hub ([dynamics_365_customer_insights_journeys_knowledge_hub.html](file:///Users/paulbaarn/code/CI/dynamics_365_customer_insights_journeys_knowledge_hub.html)), which contains **35 knowledge points** across **8 categories**.

---

## 1. Workspace & Progress Tracking Setup

Your HTML hub stores learned/saved state in browser `localStorage`. Because `localStorage` lives inside the browser and is not directly readable as a Markdown file across Antigravity sessions, pair the HTML hub with a lightweight repo-based tracker:

1. **Serve the HTML hub on a stable localhost port** (instead of `file://`, where `localStorage` can be isolated or cleared):
   - Ask Antigravity: *"Start a local HTTP server in this folder and open the knowledge hub in the browser."*
   - Serving on `http://localhost:8000` ensures your browser `localStorage` progress persists reliably.
2. **Keep a Markdown progress & notes log in this folder**:
   - Create a `PROGRESS.md` (with checkboxes for all 35 topics) and a `notes/` folder (one file per category, e.g. `notes/01-architecture-and-setup.md`).
   - Why: Antigravity can read `PROGRESS.md` and `notes/` at the start of any conversation to know exactly what you have mastered, where you struggled, and what to review next.

---

## 2. Curriculum Roadmap (35 Knowledge Points in 4 Phases)

Follow the hub's 8 categories in dependency order—foundations and compliance first, then orchestration, content, and real-world MVP patterns:

| Phase | Categories | Topics | Focus |
| :--- | :--- | :---: | :--- |
| **Phase 1: Foundation & Compliance** | Architecture & Setup (5)<br>Consent & Guardrails (5) | 10 | Platform overview, DKIM/SPF, Brand Profiles, Business Units, Contact-Point Consent, Preference Centers, Quiet Times, Frequency Capping |
| **Phase 2: Targeting & Orchestration** | Audience & Segments (2)<br>Triggers & Journeys (4) | 6 | Dynamic/Hybrid Segments, Segment vs. Trigger Journeys, Dataverse & Custom Triggers, A/B Testing |
| **Phase 3: Content, Events & Measurement** | Content, Forms & AI (5)<br>Events & Leads (3)<br>Analytics & Fabric (3) | 11 | Dynamic Personalization & Power Fx, Copilot Content/Form Fill, Modern Forms, Events & Teams Webinars, Lead Scoring, Sankey Drop-Offs, Microsoft Fabric |
| **Phase 4: Production Mastery** | MVP Best Practices (8) | 8 | ALM & Proactive Journeys, Website Visitor Identification, Custom Dashboards, Insights Tab, Event Journey Pattern, Consent Audit-Readiness |

---

## 3. How to Use Antigravity for Optimal Studying

### A. Active Recall & Socratic Quizzing (`/grill-me`)
- **When to use**: After reading a module or Microsoft Learn article.
- **How**: Type `/grill-me` and tell Antigravity which topic you just studied (e.g., *"Grill me on Contact-Point Consent & Compliance Profiles"*).
- **Why it works**: Instead of passive reading, Antigravity will interview you with scenario-based questions (e.g., *"A customer opts out of one brand's commercial emails—how do Business Units and Compliance Profiles handle that?"*) and expose gaps immediately.

### B. Deep-Dive Research & Documentation Synthesis (`research` & `/browser`)
- **When to use**: When a topic in the HTML hub links to a dense Microsoft Learn page or MVP blog post.
- **How**:
  - Ask Antigravity to **summarize and compare** concepts (e.g., *"Compare Segment-based vs. Trigger-based journeys with concrete examples and edge cases"*).
  - Use `/browser` when you want Antigravity to open the HTML hub or navigate interactive Microsoft Learn pages.
  - Ask Antigravity to **visualize** complex flows using Mermaid diagrams (e.g., trigger lifecycle, consent evaluation order, or Dataverse → Fabric data flow) saved directly into your `notes/`.

### C. Spaced Repetition & Study Cadence (`/schedule`)
- **When to use**: To build a consistent habit and prevent forgetting earlier modules.
- **How**: Use `/schedule` to set up a recurring check-in or quiz prompt (e.g., *"Every morning at 9:00 AM, quiz me on 3 questions from topics I marked learned last week"*).

### D. Turn Your Hub URLs into Audio, Flashcards & Quizzes (NotebookLM MCP)
You have the **NotebookLM** integration connected in this environment. You can ask Antigravity to:
1. Create a dedicated NotebookLM notebook for Dynamics 365 CI-J.
2. Feed the Microsoft Learn and MVP URLs from `dynamics_365_customer_insights_journeys_knowledge_hub.html` into it.
3. Generate **Audio Overviews** (for commuting/listening), **Flashcards**, **Quizzes**, and **Mind Maps** directly from the official sources.

### E. Structured Module Planning & Long Sessions (`/plan`, `/compact`, `/learn`)
- **`/plan`**: Before tackling a heavy phase (like Phase 3's 11 topics), use `/plan` to break it into 30–45 minute study blocks with clear objectives.
- **`/compact`**: During long Q&A or quizzing sessions, use `/compact` to summarize the conversation and free up context without losing your current study state.
- **`/learn`**: Whenever you discover a subtle Dynamics 365 rule or want Antigravity to remember how you prefer to be quizzed (e.g., *"Always include exam-style scenario questions and update PROGRESS.md after each session"*), use `/learn` to persist that behavior.

---

## 4. Recommended Daily Study Loop (30–45 Minutes)

1. **Orient (2 min)**: Open a chat in `/Users/paulbaarn/code/CI` and ask Antigravity to check `PROGRESS.md` and pick the next 1–2 topics.
2. **Learn (15 min)**: Open the topic in the HTML hub, read the summary and linked Microsoft Learn / MVP resource, and ask Antigravity to clarify any confusing mechanics or draw a diagram.
3. **Test Yourself (15 min)**: Run `/grill-me` on the topic—focus on real-world scenarios (consent edge cases, trigger timing, Power Fx fallbacks, Business Unit scoping).
4. **Log & Reinforce (5 min)**: Ask Antigravity to append key takeaways to `notes/`, check off the topic in `PROGRESS.md`, and mark it learned in the HTML hub.
