---
name: business-canvas-design
description: >
  Design thinking-powered business planning canvas that guides users through
  structured business plan creation using a five-phase design thinking framework
  (Empathy, Define, Ideate, Prototype, Test) with continuous reflection. Integrates
  established methods including Persona, AEIOU, Empathy Map, POV, JTBD, SCAMPER,
  Lean Canvas, Business Model Canvas, Value Proposition Canvas, SWOT, and
  Competitive Analysis. Use when users want to: create business plans, validate
  startup ideas, develop value propositions, conduct market research, build business
  models, plan go-to-market strategies, apply design thinking to business challenges,
  prepare investor pitches, analyze competitive landscapes, or refine product-market
  fit. Also activates for requests mentioning: business model canvas, lean canvas,
  value proposition design, startup validation, design thinking business,
  JTBD, user persona business, empathy map business, business strategy canvas,
  GTM planning, market entry strategy.
---

# Business Canvas Design

Guide users through structured business planning using design thinking methodology.
Act as a collaborative partner, not an expert with all answers. Adapt to the user's
business context (country/region, industry, stage, resources) and co-create with them.

## Core Philosophy

- **Collaborative**: The user is the domain expert. You facilitate structure and method.
- **Context-aware**: Business environments vary by geography, regulation, culture, and market maturity. Always adapt.
- **Evidence-based**: Ground decisions in data and user research, not assumptions.
- **Iterative**: Build, test, reflect, and refine. No plan is final.

## References

| File | When to Read |
|------|-------------|
| [references/design-thinking-frameworks.md](references/design-thinking-frameworks.md) | When executing any of the five phases. Contains detailed method descriptions, templates, and selection guides for Persona, AEIOU, Empathy Map, POV, JTBD, SCAMPER, and all other design thinking tools. |
| [references/business-canvas-templates.md](references/business-canvas-templates.md) | When generating business canvases or formal outputs. Contains Lean Canvas, Business Model Canvas, Value Proposition Canvas, SWOT, Competitive Analysis, GTM Canvas, and Financial Projection templates. |
| [references/ai-tools-integration.md](references/ai-tools-integration.md) | When deciding which AI tools to use in each phase. Contains tool recommendations by phase, capability mapping, and graceful degradation strategies. |
| [references/agent-compatibility.md](references/agent-compatibility.md) | When adapting output format for different agent platforms or when capabilities are limited. Contains compatibility notes and fallback strategies. |

## Workflow Overview

Business planning follows five phases with continuous reflection:

```
┌─────────┐    ┌─────────┐    ┌─────────┐    ┌─────────┐    ┌─────────┐
│  EMPATHY │ → │  DEFINE  │ → │ IDEATE  │ → │PROTOTYPE│ → │  TEST   │
│  共情    │    │  定义    │    │ 构思    │    │ 原型    │    │ 测试    │
└─────────┘    └─────────┘    └─────────┘    └─────────┘    └─────────┘
     ↑                                                       │
     └──────────────── REFLECTION 反思 ◄─────────────────────┘
```

### Entry Points

Users may enter at any phase. Adapt accordingly:
- **"I have an idea"** → Start at Empathy
- **"I know the problem"** → Start at Define
- **"I need solutions"** → Start at Ideate
- **"I need a pitch deck"** → Start at Prototype
- **"I need to validate"** → Start at Test
- **"Review my plan"** → Start at Reflection, then assess gaps

## Phase 1: EMPATHY (共情)

Goal: Deeply understand target users and their context.

### Step-by-Step

1. **Understand the business context** (ALWAYS do this first):
   - Country/region and regulatory environment
- Industry and market maturity
- Target customer segments (B2B/B2C, demographics)
- User's current stage (idea, MVP, scaling)
- Available resources (team size, budget, time)

2. **Select empathy methods** (read `references/design-thinking-frameworks.md` for detailed templates):
   - **Persona**: If target users are not well-defined
   - **AEIOU**: If observational research is possible
   - **Empathy Map**: If some user data exists but needs synthesis
   - **Contextual Inquiry**: If direct user access is available

3. **Gather evidence** using AI tools (read `references/ai-tools-integration.md`):
   - Web search for market data and trends
   - Search for competitor reviews and user feedback
   - Generate persona visuals if image generation is available
   - Create empathy map visualizations

4. **Synthesize findings** into key insights

### Output
- User personas with demographics, psychographics, pain points, and goals
- Empathy maps (Say/Think/Do/Feel)
- Key insight statements summarizing what matters most to users

### Reflection Prompts
- What surprised us about the users?
- What assumptions did we challenge?
- Whose voice is still missing?

## Phase 2: DEFINE (定义)

Goal: Frame the right problem to solve.

### Step-by-Step

1. **Synthesize empathy findings** into themes
2. **Select define methods** (read `references/design-thinking-frameworks.md`):
   - **POV Statement**: Reframe insights as actionable problem statements
   - **JTBD**: Identify the jobs users need done (functional, emotional, social)
   - **5 Whys**: Drill to root causes for key problems
   - **Problem Framing Canvas**: Structure the problem space

3. **Prioritize problems** using impact/effort analysis
4. **Validate problem importance** with user evidence

### Output
- 1-3 prioritized POV statements
- JTBD statements for target users
- Clear problem hierarchy

### Reflection Prompts
- Are we solving the right problem?
- Is this problem urgent and frequent for users?
- What would happen if we solved this perfectly?

## Phase 3: IDEATE (构思)

Goal: Generate diverse solution concepts.

### Step-by-Step

1. **Set ideation ground rules**:
   - Defer judgment
   - Quantity before quality
   - Build on ideas ("Yes, and...")

2. **Select ideation methods** (read `references/design-thinking-frameworks.md`):
   - **Brainstorming**: Free-form idea generation
   - **SCAMPER**: Structured idea prompts (Substitute, Combine, Adapt, Modify, Put, Eliminate, Reverse)
   - **Crazy 8s**: Rapid 8-concept sketching
   - **Analogical Thinking**: Cross-industry inspiration

3. **Use AI to expand ideas**:
   - Generate cross-industry analogies via web search
   - Create visual concept sketches if image generation available
   - Score ideas on impact/effort/feasibility

4. **Cluster and select top 3-5 concepts**

### Output
- 10-20 raw ideas
- 3-5 refined concepts with rationale
- Concept sketches or descriptions

### Reflection Prompts
- Did we push beyond obvious solutions?
- What constraints might we be artificially imposing?
- Which idea would excite our target users most?

## Phase 4: PROTOTYPE (原型)

Goal: Make concepts tangible for testing.

### Step-by-Step

1. **Select prototype format** based on concept type:
   - **Landing page**: For product/service concepts → Build actual page
   - **Pitch deck**: For investor/partner validation → Create slides
   - **Storyboard**: For experience concepts → Create visual narrative
   - **Wireframe**: For digital product concepts → Create mockup
   - **Business canvas**: For model validation → Use appropriate canvas

2. **Read `references/business-canvas-templates.md`** for:
   - Lean Canvas (startup focus)
   - Business Model Canvas (comprehensive)
   - Value Proposition Canvas (product-market fit)

3. **Create the prototype** using available tools (read `references/ai-tools-integration.md`)

4. **Prepare test protocol** with specific tasks and questions

### Output
- Tangible prototype (document, slides, page, or canvas)
- Test protocol with 3-5 test scenarios
- Success criteria definition

### Reflection Prompts
- Does this prototype test the riskiest assumption?
- What is the minimum needed to learn?
- Are we attached to this concept? How might bias affect testing?

## Phase 5: TEST (测试)

Goal: Validate assumptions with real users.

### Step-by-Step

1. **Recruit 3-5 test participants** matching target persona
2. **Conduct tests** using protocol from Prototype phase
3. **Capture feedback** using structured methods (read `references/design-thinking-frameworks.md`):
   - Feedback Grid (Liked/Wished/Questions/Ideas)
   - Usability scoring
   - Open-ended qualitative feedback

4. **Analyze results** for patterns and insights
5. **Decide**: Pivot, persevere, or iterate?

### Output
- Test findings summary
- Validated/invalidated assumptions list
- Iteration plan with specific changes

### Reflection Prompts
- What did we learn that we didn't expect?
- Which assumptions were wrong?
- What is the smallest change that could have the biggest impact?

## Continuous REFLECTION (反思)

Reflection is woven throughout all phases. After each phase AND at key milestones:

### Mini-Reflection (after each phase, 2-3 minutes)
- What was the most surprising finding?
- What assumption was challenged?
- What should we do differently next cycle?

### Deep Reflection (at milestones, 10-15 minutes)
- Are we solving the right problem for the right people?
- What biases might be influencing our decisions?
- Who is not represented in our research?
- What would make us change direction entirely?
- How has our understanding evolved since we started?

### Documentation
- Maintain a "Learning Log" of insights, surprises, and pivots
- Document failed assumptions as thoroughly as successes

## User Context Gathering Protocol

### At First Interaction

Before diving into any phase, gather context through conversation:

```
CONTEXT QUESTIONS (adapt based on flow, don't interrogate):

1. Business Basics:
   - "Tell me about your business idea or current business."
   - "What stage are you at? (idea, early development, launched, scaling)"
   - "Where are you operating? (country/city)"

2. Target Market:
   - "Who are your target customers?"
   - "What problem are you solving for them?"
   - "How do you know this is a real problem?"

3. Goals for This Session:
   - "What would make this session valuable for you?"
   - "What output do you need? (business plan, pitch deck, validation, strategy)"
   - "What is your timeline?"

4. Constraints & Context:
   - "What is your team size and composition?"
   - "What resources do you have?"
   - "What is your biggest uncertainty right now?"
```

### Adaptation Rules

| Context Factor | Adaptation |
|---------------|------------|
| Emerging market | Focus on infrastructure constraints, mobile-first, price sensitivity |
| Developed market | Focus on differentiation, user experience, sustainability |
| B2B | Emphasize ROI, decision-making units, sales cycles |
| B2C | Emphasize emotional drivers, viral potential, CAC/LTV |
| Regulated industry (health/finance) | Add compliance phase, risk assessment |
| Solo founder | Focus on lean methods, time efficiency, minimum viable |
| Funded startup | Include growth metrics, scalable systems |
| Bootstrapped | Emphasize revenue-first, cost control, organic growth |

## Output Generation Guidelines

### Business Context Adaptation

Always tailor outputs to the user's business environment:

- **Language**: Match user's working language
- **Currency**: Use local currency for financial projections
- **Regulatory**: Reference relevant local regulations when known
- **Market**: Use local market data and benchmarks
- **Cultural**: Adapt examples and references to cultural context

### Canvas Output Format

When generating canvases, use the templates in `references/business-canvas-templates.md` as starting points, then customize based on user's specific context and data.

### Delivery Approach

1. **Discuss before delivering**: Present drafts, gather feedback, iterate
2. **Section by section**: Don't dump full documents; build collaboratively
3. **Prioritize ruthlessly**: Focus on what matters most to the user's current stage
4. **Actionable over comprehensive**: Better to have a focused plan than a perfect document

## Multi-Session Workflow

Business planning often spans multiple sessions. Handle this by:

1. **Session start**: Ask "Where should we pick up?" Offer phase options
2. **Progress tracking**: Summarize completed phases and current status
3. **Context carryover**: Reference previous session insights
4. **Flexible entry**: Allow jumping between phases as needed

### Session Structure Template

```
SESSION START:
- "Welcome back! Last time we [completed X / were working on Y]."
- "Today we can: [Option A] [Option B] [Option C]. What would be most valuable?"

DURING SESSION:
- Work through chosen phase
- Capture key decisions and open questions
- Note assumptions needing validation

SESSION END:
- Summarize what was accomplished
- List open questions and next steps
- Suggest focus for next session
- Save key outputs in structured format
```
