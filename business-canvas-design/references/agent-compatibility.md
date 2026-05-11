# Agent Compatibility Guide

## Table of Contents
1. [Universal Skill Format](#universal-skill-format)
2. [Platform-Specific Adaptations](#platform-specific-adaptations)
3. [Trigger Mechanisms](#trigger-mechanisms)
4. [Capability Detection](#capability-detection)
5. [Graceful Degradation](#graceful-degradation)

---

## Universal Skill Format

This skill uses the standard format compatible with most AI agent platforms:

```
skill-name/
├── SKILL.md           (Core instructions)
├── references/        (Extended knowledge)
│   ├── file1.md
│   └── file2.md
└── scripts/           (Executable code)
    └── script1.py
```

### Key Compatibility Principles

1. **Markdown-based**: All documentation in standard Markdown
2. **No proprietary formats**: No platform-specific metadata or schemas
3. **Tool-agnostic references**: AI tool references are generic, mapped at runtime
4. **Progressive disclosure**: Core workflow in SKILL.md, details in references
5. **Imperative instructions**: SKILL.md uses imperative/infinitive form

---

## Platform-Specific Adaptations

### General Agent Platforms (Claude/GPT/Gemini/Copilot)

**Format**: Standard as-is
**Adaptation needed**: None
**Trigger**: Natural language description matching

### Kimi / Moonshot AI

**Format**: Standard with .skill packaging
**Packaging**: Use package_skill.py to create .skill file
**Trigger**: Name and description in frontmatter
**Special**: Supports web_search, data sources, code execution natively

### AutoGPT / Agent Frameworks

**Format**: SKILL.md as system prompt component
**Adaptation**: Add explicit function-calling guidance in SKILL.md
**Trigger**: Task-based description matching

### LangChain / LlamaIndex

**Format**: SKILL.md as tool description
**Adaptation**: Wrap as tool with input/output schemas
**Trigger**: Tool selection by LLM

### Custom RAG Systems

**Format**: Chunk references for retrieval
**Adaptation**: Split references into retrievable chunks
**Trigger**: Similarity search on user query

---

## Trigger Mechanisms

### Description-Based Triggering

The `description` field in YAML frontmatter serves as the primary trigger:

```yaml
---
name: business-canvas-design
description: >
  Design thinking-powered business planning canvas. Use when users want to:
  create business plans, validate startup ideas, develop value propositions,
  conduct market research, build business models, plan go-to-market strategies,
  or apply design thinking to business challenges. Covers empathy mapping,
  problem definition, ideation, prototyping, and testing with continuous reflection.
---
```

### Keyword Triggers

| User Says | Skill Activation |
|-----------|-----------------|
| "business plan", "创业计划", "商业计划" | Core workflow |
| "design thinking", "设计思维" | Full framework |
| "value proposition", "价值主张" | Value Proposition Canvas |
| "business model", "商业模式" | Business Model Canvas |
| "market research", "市场调研" | Empathy + Define phases |
| "pitch deck", "路演" | Lean Canvas + Prototype |
| "startup idea", "创业想法" | Full validation workflow |
| "JTBD", "persona", "empathy map" | Specific tools |
| "go to market", "GTM" | Go-to-Market Canvas |
| "competitive analysis", "竞争分析" | Competitive landscape |

---

## Capability Detection

### Runtime Capability Assessment

When executing, the agent should detect available capabilities:

```
CAPABILITY CHECKLIST:
□ Web search available
□ Data source APIs available
□ Code execution available
□ Image generation available
□ Document creation available
□ Slide creation available
□ Browser automation available
```

### Capability-Based Adaptation

| If Available | Use For | If Unavailable | Alternative |
|-------------|---------|----------------|-------------|
| Web search | Market research, competitor analysis | Ask user | Request manual research from user |
| Data sources | Financial data, demographics | Use estimates | Ask user for data, use benchmarks |
| Code execution | Financial modeling, analysis | Manual calculation | Simplify models, use templates |
| Image generation | Personas, concept art | Text descriptions | ASCII art, detailed text descriptions |
| Document creation | Formal business plans | Text output | Structured markdown output |
| Slide creation | Pitch decks | Outline format | Markdown structure for manual creation |
| Browser automation | Deep research | Web search summary | Targeted search queries |

---

## Graceful Degradation

### Minimal Viable Execution

Even with no special tools, the skill provides value through:

1. **Structured thinking**: Design thinking process via text
2. **Templates**: Ready-to-use canvas templates in markdown
3. **Questions**: Guided discovery through targeted questions
4. **Frameworks**: Systematic approach to business planning

### Degradation Levels

```
Full Capability ──► Limited Tools ──► Text Only
    │                   │               │
    ▼                   ▼               ▼
 Auto research    Guided research   User-provided
 Auto generation  Assisted creation Templates only
 Auto analysis    Guided analysis   Framework prompts
```

### User Compensation Strategy

When capabilities are limited, explicitly ask the user to provide:

| Missing Capability | User Compensation |
|-------------------|-------------------|
| No web search | "Please share any market research you've done" |
| No data sources | "What financial data do you have available?" |
| No image generation | "Shall I describe the visual instead?" |
| No document creation | "I'll structure this as markdown you can convert" |
| No code execution | "I'll outline the calculation; please verify with a calculator" |
