<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0A1F3F&height=200&section=header&text=Edigarlos%20Josue&fontSize=50&fontColor=E8DCC4&animation=fadeIn&fontAlignY=38&desc=AI%20Engineer%20%7C%20Lunar%20Founder%20%7C%20Agentic%20Systems%20Architect&descAlignY=55"/>
</div>

<div align="center">

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&pause=1000&color=0A9FD9&center=true&vCenter=true&width=700&lines=Building+Lunar:+The+education+AI+that+actually+learns+how+you+learn.;Production+systems+that+scale.+No+shortcuts.&repeat=false)](https://bambalunar.app)

</div>

---

## Who I Am

AI Engineer specializing in **agentic systems architecture**, **educational technology**, and **full-stack infrastructure**. Currently building **Lunar** — a pedagogically-architected AI platform designed to become the operating system of how people actually learn.

I'm **Edigarlos Josue Vasquez Mendoza** — self-taught, Venezuelan-based. Most AI engineers integrate APIs. I architect systems from database schema to frontend UI, alone, at production scale. That's not common. It's also not a flex—it's a constraint that forces you to understand every layer.

My focus:
- **Agentic Systems** — designing AI agents that reason, evaluate, and adapt (not just chain API calls)
- **Pedagogical Architecture** — building AI systems that actually understand learning, not just education chatbots
- **Full-Stack Production** — systems that work at scale with real users depending on them
- **AI Governance** — safety and controllability as a first-class design concern

---

## Lunar: The Central Project

### What It Is (Not)

Lunar is **not** a chatbot with a "study mode" bolted on top. That's what exists already.

Lunar is an **agentic learning companion** architected from first principles as an educational system. It diagnoses where you actually are in a topic. It doesn't dump information—it delivers one conceptual building block at a time. It verifies understanding before advancing. It remembers your actual progress across every topic you study, across an entire semester.

The difference isn't the LLM underneath. It's the pedagogical infrastructure built around it.

### Architecture: What Makes It Different

**Orchestrator** — Not a generic "be a good tutor" prompt. An explicit pedagogical protocol:
- New topic → delivers the core idea first, nothing else
- Next step: only the next conceptual block
- Internal classification: fundamental vs. supporting context vs. exam-relevant
- Comprehension verification only when it matters, not by routine

**Anchors System** — A concept storage layer that classifies knowledge by its actual role:
- What causes confusion
- Procedures vs. principles
- What transfers to other contexts
- Underlying mechanisms
- Supporting context

Each anchor carries a real-time "mastery state" per learner: seen, explained, validated, mastered.

**LearnerProfile** — Persistent tracking by concept, not by conversation. Your progress doesn't reset. The system knows exactly where you stand in every topic you've touched.

**Dual Agent Architecture** — Two agents, two roles, zero redundancy:
- Primary agent: guiding learning (three model variants: Classic, Creative, Tutor)
- Grok: citations, research, image analysis (has vision—the primary agent doesn't)

This isn't artificial separation. Grok literally provides the visual context the system needs.

**Intentional Communication** — Instructions are specific, not generic. Personality persists across turns. The system can say "I don't know" and mean it. Every tool has explicit boundaries.

### The Product Pieces

**Study Routes** — The core agentic layer. You give Lunar a learning goal. It converts it into a visible sequence of sub-topics. It advances only when something is actually mastered. It surfaces knowledge gaps automatically and builds routes to fill them. Everything visible. No black box.

**MicroChats** — Focused conversations anchored to a specific text passage or citation. Lives in a sidebar panel, integrated with the citation system. Each generates a two-layer context file—one human-readable, one internal metadata—so the primary agent knows what was discussed without loading the full conversation.

**Class Notes / Study Prep** — From a PDF, presentation, or lecture recording: auto-generated notes (Notion-style structure) using the same concept extraction that feeds Anchors. Not a flat summary. Concept-driven, with importance hierarchy built in.

**Spaces** — The infrastructure for daily engagement. A Space can contain Subspaces (subjects). Scale from a single semester course to an entire degree program (e.g., "Computer Science" with Subspaces like "Networks", "Advanced Programming"). This is what makes Lunar into an actual learning OS, not a tool you open once and close.

**Modes** — Study, Learn Fast, Research, Prepare for Exam. These are prompt-layer variations on the base behavior. But "Prepare for Exam" does more—it restructures interaction: topic selection + source attachment instead of freeform chat.

**Home** — Three zones, not a generic text box:
- Quick access to active Spaces/Subjects (get to work immediately)
- Discovery zone with linked concepts (like navigating Wikipedia—one term leads to another)
- Freeform chat always available (no friction for people who don't need structure)

### Why Someone Would Use It Daily

Not because it solves one problem and you close the tab. Because it's infrastructure for an entire learning period. It remembers where you stand in every subject. It doesn't repeat itself. It feels like talking to someone actually paying attention to how you learn, not just answering what you ask.

**Market validation:** Brainly spent years as a Q&A repository. Today it's pivoting to exactly this—persistent learning accompaniment, auto-generated class notes, personalized study plans, discovery as entry point. That a major player is moving the same direction doesn't diminish Lunar's opportunity. It confirms the thesis. Lunar's bet is architectural depth, not first-mover advantage.

### Brand Identity

**Current name:** Lunar (temporary—rebrand is planned but deliberately postponed until the product feels right)

**Proposed rebrand:** Traza (Spanish: "trace", captures both the route-tracing and the visible reasoning trail of the agent). Alternatives: Andamio (pedagogical scaffolding), Cursa, Norte, Indaga.

**Colors:** Dark blue-black `hsl(210, 45%, 8%)` + warm cream `#E8DCC4`. Intentionally distinct from gradient-purple edtech aesthetic and terra-cream alternatives. Carries through the rebrand unchanged.

**Logo:** Deliberately undefined until the product works well. Brand visual identity (name, logo, design language) comes after the engine is solid. When it does, it should evoke route/trace/reasoning—not moons or celestial imagery (that gets retired with "Lunar").

### The Near Term

RevenueCat Shipathon window (Aug 1 – Sep 30, 2026) demands a real mobile app in app stores with RevenueCat SDK for monetization. This isn't a detail—it's a core requirement. Strategy: port what's working in web, not rebuild from scratch.

Priority right now: the Orchestrator reasoning well, the agent feeling present, Study Routes and Spaces functioning. Name, logo, visual polish wait for the engine to be solid.

### The Horizon

After that: complete rebrand (name, logo, visual identity), user-selectable model variants (Classic/Creative/Tutor) based on real usage data, and eventually university integration as actual academic infrastructure—the original north star.

---

## Full-Stack Technical Foundation

**Frontend**
- React 18 + TypeScript + TailwindCSS
- Real-time streaming UI with optimistic updates
- Mobile-first architecture (web → app port strategy)

**Backend**
- FastAPI (async Python) + PostgreSQL
- Message queue for async agent workflows
- WebSocket for live response streaming
- Multi-provider LLM abstraction (OpenAI, Claude, Gemini)

**AI Layer**
- Orchestrator protocol (pedagogically explicit, not chain-of-thought generic)
- Dual-agent system (primary + Grok for vision)
- Token optimization and cost tracking
- Model-agnostic agent interface

**Memory & Learning**
- Vector embeddings for semantic search
- Long-term conversation history with automatic summarization
- LearnerProfile state management by concept
- Anchor classification and mastery tracking

**Infrastructure**
- Docker containerization
- Production deployment (cloud VPS)
- CI/CD pipeline for continuous delivery

---

## Tech Stack

<div align="center">

**Languages**
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

**Frontend**
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)

**Backend & Infrastructure**
![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2CA5E0?style=for-the-badge&logo=docker&logoColor=white)

**AI & Models**
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white)
![Anthropic](https://img.shields.io/badge/Claude-000000?style=for-the-badge&logo=anthropic&logoColor=white)

</div>

---

## Current Work

Lunar is under active development. The focus right now:
- Orchestrator reasoning (pedagogical protocol execution)
- Agent presence and personality (feeling deliberate, not generic)
- Study Routes and Spaces (core infrastructure)
- Mobile app development (RevenueCat Shipathon requirement)

The product is live for testing at [bambalunar.app](https://bambalunar.app)

---

## Open to

Frontier AI labs and roles where I can work on hard infrastructure problems. Looking for environments where:
- Full-stack ownership is valued over specialization
- Shipping and iteration matter more than endless planning
- AI safety is a design constraint, not an afterthought

---

## Philosophy

Most AI engineers can integrate an API. Some can architect a system. Fewer still can ship it solo and scale it to real users. That gap—between knowing what's possible and actually building it—is where I operate. Execution is the ultimate credential.

```
What I build:
- Systems that work at scale
- Reasoning that's explicit, not hidden
- Infrastructure for others to build on
- Things that actually get used by real people

How I measure it:
- Real users depending on it
- Zero excuses for "it works in staging"
- Architectural decisions that survive pressure
- Simplicity earned through complexity solved
```

---

## Let's Build

Platform: [bambalunar.app](https://bambalunar.app)
Code: [github.com/edies76](https://github.com/edies76)

---

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0A1F3F&height=100&section=footer"/>
</div>
