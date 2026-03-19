# Product reasoning for complex decisions AI Agent

<p align="left">
  <img src="https://img.shields.io/badge/type-llm%20skill-111827" alt="Type: LLM Skill" />
  <img src="https://img.shields.io/badge/claude-compatible-D97706" alt="Claude Compatible" />
  <img src="https://img.shields.io/badge/custom%20gpt-ready-059669" alt="Custom GPT Ready" />
  <img src="https://img.shields.io/badge/focus-ux%20reasoning-2563EB" alt="Focus: Product Reasoning" />
</p>

**Product AI Agent** is a structured UX reasoning framework for designers, product managers, and researchers who need a sharp thinking partner, not a generic feature suggester.

It transforms a general-purpose language model into a focused UX collaborator with a defined critical posture, strict reasoning standards, vocabulary constraints, and three operating modes for different decision contexts.

This is **not** a collection of UX tips.  
It is a **reasoning system** built to interrogate problems before offering direction.

---

## Why This Exists

Most AI Product assistants generate surface-level suggestions.

Product AI Agent is built to do something harder:

- question the framing
- challenge weak assumptions
- expose hidden constraints
- clarify trade-offs
- take a position with conviction

The goal is not to generate more ideas.  
The goal is to produce **better judgment**.

---

## What This Project Is

Product AI Agent is a structured skill definition designed for:

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

Product AI Agent is built for:

- **Product managers** making trade-off decisions under constraint
- **Cross-functional teams** pressure-testing decisions before launch
- **Senior UX designers** navigating ambiguity at scale
- **Design researchers** who want a second opinion with rigor

---

## Core Capabilities

| Capability | Description |
|---|---|
| User-Centered Design Mastery | Heuristics, usability principles, interaction patterns, and failure modes |
| Problem-Solving and Product Thinking | Frameworks for decomposing complex UX challenges into tractable decisions |
| Data-Driven Decision-Making | Balancing qualitative signals, quantitative evidence, and business constraints |
| Creativity and Ideation | Divergent thinking techniques grounded in real design constraints |
| Accessibility and Inclusion | WCAG, cognitive load, and universal design applied to real product decisions |
| AI and Automation in UX | Where AI helps design, where it distorts it, and how to tell the difference |
| Ethics and Responsibility | Dark patterns, fairness in interfaces, trust as a design material |
| Continuous Learning and Iteration | Feedback loop design, usability testing structures, and learning from failure |
| Effective Communication | How to present design decisions to stakeholders who think in revenue, not flows |
| Strategic Decision Support | Prioritization, trade-off analysis, and the long-term cost of short-term design debt |
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
Product AI Agent takes a stance. It explains why one path is stronger than another.

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
├── README.md                        ← This file
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
```
---

## Quick Start

### Using with Claude (claude.ai)

1. Open a new **Project** in Claude  
2. Paste the contents of `prompts/system-prompt.md` into the project instructions  
3. Start a conversation with one of the starter prompts below  

### Using via Anthropic API

```python
import anthropic

with open("prompts/system-prompt.md", "r") as f:
    system_prompt = f.read()

client = anthropic.Anthropic()

message = client.messages.create(
    model="claude-opus-4-6",
    max_tokens=2048,
    system=system_prompt,
    messages=[
        {
            "role": "user",
            "content": "Give me three alternative UX solutions for reducing drop-off in enterprise onboarding."
        }
    ]
)

print(message.content[0].text)
```
---

## Starter Prompts

```text

Give me three alternative UX solutions for [insert problem or scenario].

How do I balance business goals and user needs when designing [insert feature]?

What are the best UX patterns for [insert feature]?

Challenge my assumptions about [insert UX principle or trend].

How do I design for uncertainty and ambiguity in [insert complex problem]?

What are emerging trends I can incorporate into [insert UX feature]?
```
---

## Design Principles

### Positions, Not Suggestions
The agent takes a stance. It explains why one direction is stronger than another. It does not offer five equally valid options and ask you to choose.

### Evidence Before Opinion
Every claim is anchored to a principle, a behavioral pattern, or a documented failure mode. Opinions without grounding are not offered.

### Clarity Under Complexity
The harder the problem, the more important the structure. This agent does not retreat into abstraction when problems get complicated.

### Commitment Over Hedging
The agent does not hide behind endless qualifiers or reflexive “it depends” language. It accounts for context, then commits.

---

## Vocabulary Constraints

This skill enforces a strict vocabulary policy. Words that signal vague, corporate, or inflated thinking are prohibited.

See `docs/vocabulary-constraints.md` for the full list.

---

## Author

**Melisa Battal**  
Product Manager, AI/UX Systems  
[melisabattal.com](https://melisabattal.com)
