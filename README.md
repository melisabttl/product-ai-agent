# UX Prism AI

![LLM Skill](https://img.shields.io/badge/Type-LLM%20Skill-111827)
![Claude Compatible](https://img.shields.io/badge/Claude-Compatible-D97706)
![Custom GPT Ready](https://img.shields.io/badge/Custom%20GPT-Ready-059669)
![Focus](https://img.shields.io/badge/Focus-UX%20Reasoning-2563EB)

**A high-performance UX reasoning framework for designers, product managers, and researchers who need a sharp thinking partner—not a generic feature suggester.**

UX Prism AI is built to interrogate product and design problems before offering direction. It operates at the intersection of **UX strategy**, **behavioral psychology**, **product thinking**, and **ethics**, helping teams challenge assumptions, expose trade-offs, and make stronger decisions before they ship.

---

## Why UX Prism AI Exists

Most AI UX tools generate surface-level suggestions.  
UX Prism AI is built to do something harder:

- question the framing
- challenge weak reasoning
- surface hidden constraints
- take a position with clarity

This is **not** a prompt pack.  
It is **not** a library of UX tips.  
It is a **structured reasoning system** for teams working through decisions that matter.

---

## What This Project Is

UX Prism AI is a structured skill definition designed for:

- **Claude (Anthropic)**
- **custom GPTs**
- **any LLM platform that supports system-level instructions**

It transforms a general-purpose language model into a focused UX reasoning partner with:

- a defined critical posture
- strict vocabulary constraints
- clear reasoning standards
- three operational modes for different decision contexts

The goal is not to produce more ideas.  
The goal is to produce **better judgment**.

---

## Who It’s Built For

UX Prism AI is built for:

- **Senior UX designers** navigating ambiguity at scale
- **Product leads** making trade-off decisions under constraint
- **Design researchers** who want a second opinion with substance
- **Cross-functional teams** pressure-testing product decisions before launch

---

## Core Capabilities

### Structured UX reasoning
The agent does not jump to solutions. It examines the problem, the assumptions behind it, and the trade-offs that shape the outcome.

### Position-taking
It does not offer five equally safe options and ask you to choose. It takes a stance and explains why that stance is stronger.

### Constraint awareness
It accounts for behavioral, operational, ethical, and product constraints instead of treating UX as an isolated layer.

### Critical challenge
It is designed to interrogate confidence, not reinforce it blindly.

---

## Operational Modes

### Strategic Mode _(Default)_
Deep analysis for decisions with meaningful downstream consequences.

Use this mode when you need to:

- examine trade-offs
- identify hidden constraints
- reference real-world patterns or failure modes
- make a decision that is hard to reverse

Best for: product direction, flow design, onboarding strategy, platform UX, AI feature decisions.

---

### Direct Mode
One recommendation. Minimal hedging. Compressed reasoning.

Use this mode when:

- speed matters
- the team needs a clear next move
- you want a judgment, not a workshop

Best for: quick decisions, prioritization, design reviews, execution calls.

---

### Provocative Mode
Adversarial reasoning designed to break weak logic before the market does.

Use this mode when you want to:

- challenge your assumptions
- pressure-test your rationale
- expose blind spots before launch

Best for: validating confidence, reviewing polished concepts, interrogating “obvious” solutions.

---

## Design Principles

### Positions, not suggestions
UX Prism AI takes a clear position. It explains why one path is stronger than another.

### Evidence before opinion
Claims are grounded in principles, user behavior, product logic, or known failure patterns.

### Clarity under complexity
As the problem gets harder, the reasoning gets sharper—not more abstract.

### No performative hedging
It does not hide behind endless qualifiers. It considers context, then commits.

---

## Repository Structure

```text
ux-wise-agent/
├── README.md                         ← This file
├── skill.md                         ← Master skill definition
├── prompts/
│   ├── system-prompt.md             ← Full system prompt for Claude and compatible LLMs
│   ├── starter-prompts.md           ← Curated prompt library
│   ├── strategic-mode.md            ← Strategic Mode prompt layer
│   ├── direct-mode.md               ← Direct Mode prompt layer
│   └── provocative-mode.md          ← Provocative Mode prompt layer
├── examples/
│   ├── onboarding-analysis.md       ← Strategic Mode example
│   ├── checkout-friction.md         ← Direct Mode example
│   └── navigation-challenge.md      ← Provocative Mode example
├── knowledge/
│   ├── ux-principles.md             ← Core UX knowledge base summary
│   ├── heuristics.md                ← Nielsen’s heuristics with applied commentary
│   └── ai-ux-considerations.md      ← AI-specific UX reasoning guide
├── integrations/
│   ├── claude-skill.md              ← How to use with Claude Projects or API workflows
│   ├── custom-gpt.md                ← How to deploy in OpenAI custom GPTs
│   └── api-usage.md                 ← Direct API usage with system prompt injection
└── docs/
    ├── contribution-guide.md        ← How to extend or refine the skill
    ├── vocabulary-constraints.md    ← Banned words, reasoning standards, and tone rules
    └── changelog.md                 ← Version history




# ux-agent-
UX AI is a structured skill definition that turns general purpose LLMs into focused UX reasoning partners with a critical posture, constrained vocabulary, and three operational modes.
