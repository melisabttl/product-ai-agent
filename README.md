# UX AI Agent

<p align="left">
  <img src="https://img.shields.io/badge/type-llm%20skill-111827" alt="Type: LLM Skill" />
  <img src="https://img.shields.io/badge/claude-compatible-D97706" alt="Claude Compatible" />
  <img src="https://img.shields.io/badge/custom%20gpt-ready-059669" alt="Custom GPT Ready" />
  <img src="https://img.shields.io/badge/focus-ux%20reasoning-2563EB" alt="Focus: UX Reasoning" />
</p>

**UX AI Agent** is a structured UX reasoning framework for designers, product managers, and researchers who need a sharp thinking partner, not a generic feature suggester.

It transforms a general-purpose language model into a focused UX collaborator with a defined critical posture, strict reasoning standards, vocabulary constraints, and three operating modes for different decision contexts.

This is **not** a collection of UX tips.  
It is a **reasoning system** built to interrogate problems before offering direction.

---

## Why This Exists

Most AI UX assistants generate surface-level suggestions.

UX AI Agent is built to do something harder:

- question the framing
- challenge weak assumptions
- expose hidden constraints
- clarify trade-offs
- take a position with conviction

The goal is not to generate more ideas.  
The goal is to produce **better judgment**.

---

## What This Project Is

UX AI Agent is a structured skill definition designed for:

- **Claude (Anthropic)**
- **custom GPTs**
- **any LLM platform that supports system-level instructions**

It turns a general-purpose model into a UX reasoning partner that:

- thinks critically instead of performing agreement
- evaluates decisions through product, behavioral, and ethical lenses
- avoids vague, inflated, or corporate language
- gives sharper guidance when the stakes are high

---

## Who It’s For

UX AI Agent is built for:

- **Senior UX designers** navigating ambiguity at scale
- **Product managers** making trade-off decisions under constraint
- **Design researchers** who want a second opinion with rigor
- **Cross-functional teams** pressure-testing decisions before launch

---

## Core Capabilities

### Structured UX Reasoning
The agent does not rush to solutions. It examines the problem, the assumptions behind it, and the trade-offs that shape the outcome.

### Position-Taking
It does not present five equally safe options and ask you to choose. It takes a stance and explains why.

### Constraint Awareness
It considers behavioral, operational, ethical, and product constraints instead of treating UX as an isolated layer.

### Critical Challenge
It is designed to interrogate confidence, not reinforce it blindly.

---

## Operational Modes

### Strategic Mode *(default)*
Deep analysis for decisions with meaningful downstream consequences.

Use this mode when you need to:

- examine trade-offs
- surface hidden constraints
- reference patterns or failure modes
- take a position on a complex decision

Best for: onboarding, navigation systems, platform UX, enterprise workflows, and AI-assisted experiences.

### Direct Mode
One recommendation. Minimal hedging. Compressed reasoning.

Use this mode when:

- time is limited
- a decision must be made quickly
- you need a recommendation, not a workshop

Best for: reviews, prioritization, quick product calls, and execution decisions.

### Provocative Mode
Adversarial reasoning designed to break weak logic before users do.

Use this mode when you want to:

- challenge assumptions
- pressure-test rationale
- expose blind spots before finalizing a direction

Best for: high-confidence ideas, risky launches, internal debate, and decision validation.

---

## Design Principles

### Positions, Not Suggestions
UX AI Agent takes a stance. It explains why one path is stronger than another.

### Evidence Before Opinion
Claims should be grounded in UX principles, user behavior, product logic, or known failure patterns.

### Clarity Under Complexity
As the problem gets harder, the reasoning should become sharper, not more abstract.

### Commitment Over Hedging
The system accounts for context, then makes a judgment.

---

## Quick Start

### Positions, Not Suggestions
UX AI Agent takes a stance. It explains why one path is stronger than another.

### Evidence Before Opinion
Claims should be grounded in UX principles, user behavior, product logic, or known failure patterns.

### Clarity Under Complexity
As the problem gets harder, the reasoning should become sharper, not more abstract.

### Commitment Over Hedging
The system accounts for context, then makes a judgment.

---



## Repository Structure

```text
ux-ai-agent/
├── README.md                         ← Project overview
├── skill.md                          ← Master skill definition
├── prompts/
│   ├── system-prompt.md              ← Full system prompt for Claude and compatible LLMs
│   ├── starter-prompts.md            ← Curated prompt library
│   ├── strategic-mode.md             ← Strategic Mode prompt layer
│   ├── direct-mode.md                ← Direct Mode prompt layer
│   └── provocative-mode.md           ← Provocative Mode prompt layer
├── examples/
│   ├── onboarding-analysis.md        ← Strategic Mode example
│   ├── checkout-friction.md          ← Direct Mode example
│   └── navigation-challenge.md       ← Provocative Mode example
├── knowledge/
│   ├── ux-principles.md              ← Core UX knowledge base summary
│   ├── heuristics.md                 ← Nielsen heuristics with applied commentary
│   └── ai-ux-considerations.md       ← AI-specific UX reasoning guide
├── integrations/
│   ├── claude-skill.md               ← How to use in Claude Projects or API workflows
│   ├── custom-gpt.md                 ← How to deploy in OpenAI custom GPTs
│   └── api-usage.md                  ← Direct API usage with system prompt injection
└── docs/
    ├── contribution-guide.md         ← How to extend or refine the skill
    ├── vocabulary-constraints.md     ← Banned words, reasoning standards, and tone rules
    └── changelog.md                  ← Version history




