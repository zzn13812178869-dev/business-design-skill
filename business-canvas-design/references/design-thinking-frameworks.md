# Design Thinking Frameworks & Methods Reference

## Table of Contents
1. [Core Five-Phase Framework](#core-five-phase-framework)
2. [Continuous Reflection Loop](#continuous-reflection-loop)
3. [Empathy Phase Methods](#empathy-phase-methods)
4. [Define Phase Methods](#define-phase-methods)
5. [Ideate Phase Methods](#ideate-phase-methods)
6. [Prototype Phase Methods](#prototype-phase-methods)
7. [Test Phase Methods](#test-phase-methods)
8. [Method Selection Guide](#method-selection-guide)

---

## Core Five-Phase Framework

The foundation of this skill is a design thinking process with five phases plus continuous reflection:

```
┌─────────┐    ┌─────────┐    ┌─────────┐    ┌─────────┐    ┌─────────┐
│  EMPATHY │ → │  DEFINE  │ → │ IDEATE  │ → │PROTOTYPE│ → │  TEST   │
│  共情    │    │  定义    │    │ 构思    │    │ 原型    │    │ 测试    │
└─────────┘    └─────────┘    └─────────┘    └─────────┘    └─────────┘
     ↑                                                       │
     └──────────────── REFLECTION 反思 ◄─────────────────────┘
```

### Phase Principles

**EMPATHY**: Understand users deeply. Suspend judgment. Seek stories, not just facts. Focus on emotions, frustrations, and unspoken needs.

**DEFINE**: Synthesize findings into actionable problem statements. Narrow scope. Find the balance between breadth and focus.

**IDEATE**: Generate quantity before quality. Defer judgment. Build on others' ideas. Aim for wild, unexpected concepts.

**PROTOTYPE**: Build to think. Make tangible what was abstract. Focus on the core experience, not polish. Fail fast, learn faster.

**TEST**: Learn through observation. Let users interpret. Capture reactions, not just opinions. Iterate immediately.

**REFLECTION**: After each phase and continuously, step back to examine process, assumptions, biases, and learning. Document insights for future cycles.

---

## Continuous Reflection Loop

Reflection is not a separate phase but a continuous practice woven through all phases:

### After Each Phase, Ask:
- What surprised us most?
- What assumptions were challenged?
- What biases might have influenced our work?
- How does this change our understanding of the problem?
- What would we do differently next time?

### Meta-Questions (Continuous):
- Are we solving the right problem?
- Who is not at the table whose voice matters?
- What are we avoiding asking?
- How might our own perspective limit our view?

---

## Empathy Phase Methods

### 1. Persona (用户画像)

**Purpose**: Create archetypal representations of target users to guide decision-making.

**Template**:
```
PERSONA: [Name - representative label]

Demographics:
  - Age/Gender/Occupation/Income/Location
  - Education/Family status

Psychographics:
  - Goals & aspirations
  - Fears & frustrations
  - Values & beliefs
  - Lifestyle & behaviors

Context:
  - Typical day narrative
  - Key touchpoints related to our domain
  - Technology comfort level

Quote: [Direct quote capturing their essence]

Pain points: [Top 3-5 challenges in our domain]
Gains sought: [Top 3-5 desired outcomes]
```

**AI Enhancement**: Use web search to find demographic data, industry reports, and user behavior statistics for the target region/market.

### 2. AEIOU Method

**Purpose**: Systematic observation framework for field research.

**Framework**:
| Dimension | Description | Prompt Questions |
|-----------|-------------|------------------|
| **A**ctivities | What are people doing? | What actions are observable? What sequences exist? |
| **E**nvironments | Where does it happen? | What physical/digital spaces? What atmosphere? |
| **I**nteractions | How do people interact? | With whom? With what objects/systems? What patterns? |
| **O**bjects | What artifacts are present? | What tools, devices, documents? How are they used? |
| **U**sers | Who is involved? | What roles? What skills? What relationships? |

### 3. Empathy Map (共情图)

**Purpose**: Visualize what users say, think, do, and feel to build deeper understanding.

**Template**:
```
                    [PERSONA NAME]
                         │
    ┌────────────────────┼────────────────────┐
    │    SAYS 说          │    THINKS 想       │
    │                    │                     │
    │ • Verbalized       │ • Unspoken beliefs  │
    │ • Quotes           │ • Assumptions       │
    │ • Overt complaints │ • Hidden concerns   │
    │                    │ • Aspirations       │
    ├────────────────────┼────────────────────┤
    │    DOES 做          │    FEELS 感       │
    │                    │                     │
    │ • Observable       │ • Emotions          │
    │   actions          │ • Fears             │
    │ • Behaviors        │ • Hopes             │
    │ • Workarounds      │ • Frustrations      │
    └────────────────────┴────────────────────┘
                         │
                    [Key Insights]
```

### 4. Contextual Inquiry (情境访谈)

**Purpose**: Deep understanding through observing users in their natural environment.

**Protocol**:
1. Go to user's environment (physical or digital)
2. Observe their natural workflow without interrupting
3. Ask "why" when you see interesting behaviors
4. Have them teach you their process
5. Capture artifacts, environment details, and emotional cues

**Key Questions**:
- "Walk me through how you currently handle [task]"
- "What happened the last time you faced [problem]?"
- "Show me your workaround for [limitation]"
- "What do you wish were different about [current solution]?"

---

## Define Phase Methods

### 5. POV Statement (观点陈述)

**Purpose**: Reframe findings into actionable problem definitions.

**Template**:
```
POV: [User type] needs [need] because [insight]

Example:
"A busy working parent needs a way to quickly prepare
healthy family dinners because they feel guilty about
relying on fast food but lack time to cook from scratch."
```

**Criteria for Good POV**:
- Narrow enough to be actionable
- Broad enough to allow creative solutions
- Grounded in real user insight, not assumption
- Does not contain solution

### 6. JTBD (Jobs-to-be-Done) (待完成的工作)

**Purpose**: Understand the functional, emotional, and social jobs users hire products to do.

**Framework**:
```
When I [situation], I want to [motivation], so I can [expected outcome].

JTBD Types:
┌──────────────┬─────────────────────────────────────┐
│ Functional   │ Practical task completion           │
│ Emotional    │ How I want to feel                  │
│ Personal     │ Self-identity, values alignment     │
│ Social       │ How I want to be perceived          │
└──────────────┴─────────────────────────────────────┘
```

**Example**:
"When I'm commuting to work, I want to use my travel time productively without feeling carsick, so I can arrive prepared for my day and feel accomplished."

### 7. 5 Whys (五个为什么)

**Purpose**: Drill down to root causes of problems.

**Process**: Ask "why" five times (or until reaching root cause).

**Example**:
- Problem: Users abandon their shopping cart
- Why 1: They say shipping is too expensive
- Why 2: They didn't expect additional costs
- Why 3: Prices weren't transparent upfront
- Why 4: We hide fees to seem competitive
- Root cause: Our pricing strategy creates distrust

### 8. Problem Framing Canvas

**Template**:
```
PROBLEM FRAMING

Current state: [What is happening now?]
Desired state: [What should be happening?]
Gap: [What's missing between current and desired?]

Stakeholders affected: [Who experiences this problem?]
Impact: [What are the consequences?]
Evidence: [What data supports this framing?]

Refined problem statement:
[1-2 sentences capturing the core problem]
```

---

## Ideate Phase Methods

### 9. Brainstorming Rules

**Core Rules**:
1. Defer judgment - no criticism during generation
2. Encourage wild ideas
3. Build on others' ideas ("Yes, and...")
4. Stay focused on the topic
5. One conversation at a time
6. Be visual - sketch and write
7. Go for quantity

### 10. SCAMPER Technique

**Prompts for reimagining solutions**:
| Letter | Action | Question |
|--------|--------|----------|
| S | Substitute | What can be replaced? |
| C | Combine | What can be merged? |
| A | Adapt | What can be borrowed? |
| M | Modify | What can be magnified/minimized? |
| P | Put to other uses | What other contexts apply? |
| E | Eliminate | What can be removed? |
| R | Reverse/Rearrange | What if the order changed? |

### 11. Crazy 8s

**Process**: Fold paper into 8 sections. Sketch one idea in each section. Spend 1 minute per section. Force quantity over quality.

### 12. Analogical Thinking (类比思考)

**Process**: Look for analogous problems/solutions in unrelated domains.

**Prompts**:
- "How does nature solve a similar problem?"
- "How do other industries handle this?"
- "What's the [industry X] version of this solution?"
- "How would [famous innovator/company] approach this?"

### 13. What-If Questions

**Process**: Generate provocative constraints to force creative thinking.

- "What if we had unlimited budget?"
- "What if we had zero budget?"
- "What if this had to work without technology?"
- "What if the user had only 10 seconds?"
- "What if we had to solve this in 24 hours?"

---

## Prototype Phase Methods

### 14. Prototyping Spectrum

```
Low Fidelity ◄───────────────────────────► High Fidelity

Sketch      Storyboard    Wireframe    Clickable    Coded
(5 min)     (30 min)      (2 hrs)      (1 day)      (1 wk)

Use for:    Use for:      Use for:     Use for:     Use for:
- Exploring - Journey     - Structure  - Flow       - Real data
  concepts    mapping       & layout     testing      testing
- Many        - Scenario    - Early      - Detailed   - Performance
  options     simulation    feedback     feedback     testing
```

### 15. Storyboarding

**Template**: 4-6 panels showing user's journey
- Panel 1: User in context (situation)
- Panel 2: User encounters problem (trigger)
- Panel 3: User discovers solution (awareness)
- Panel 4: User interacts with solution (experience)
- Panel 5: User achieves outcome (resolution)
- Panel 6: User's emotional state (impact)

### 16. Role-Playing / Bodystorming

**Process**: Act out the user experience physically.
- Assign roles (user, system, environment)
- Walk through the scenario
- Note physical and emotional friction points
- Iterate in real-time

---

## Test Phase Methods

### 17. Usability Testing Protocol

**Structure**:
1. **Introduction**: Build rapport, explain process, obtain consent
2. **Pre-test questions**: Background, expectations, current behavior
3. **Tasks**: Give specific tasks, observe don't guide
4. **Think-aloud**: Ask users to verbalize thoughts
5. **Post-test**: Satisfaction ratings, open feedback
6. **Debrief**: Discuss observations, validate assumptions

### 18. A/B Testing Framework

**Process**:
1. Define hypothesis: "Changing X will improve Y because Z"
2. Identify metric: Single primary success metric
3. Create variants: Control vs. Treatment
4. Determine sample size: Statistical significance needed
5. Run test: Random assignment, simultaneous timing
6. Analyze results: Statistical and practical significance
7. Document learning: Regardless of outcome

### 19. Feedback Grid

**Template**:
```
          LIKED 喜欢          |     WISHED 希望
                              │
   • What resonated?          │   • What was missing?
   • What delighted?          │   • What confused?
   • What felt intuitive?     │   • What would improve it?
                              │
   ───────────────────────────┼───────────────────────────
                              │
   QUESTIONS 疑问             │   IDEAS 想法
                              │
   • What was unclear?        │   • Suggestions offered
   • What needs explanation?  │   • New directions proposed
   • What sparked curiosity?  │   • Build-on ideas
```

---

## Method Selection Guide

### By Business Stage

| Stage | Recommended Methods |
|-------|-------------------|
| Early exploration | AEIOU, Empathy Map, Contextual Inquiry |
| Problem validation | 5 Whys, POV, JTBD, Problem Framing |
| Solution ideation | Brainstorming, SCAMPER, Crazy 8s, Analogical Thinking |
| MVP definition | Storyboarding, Low-fi Prototyping |
| Product-market fit | Usability Testing, A/B Testing, Feedback Grid |

### By Team Size

| Team Size | Recommended Approach |
|-----------|---------------------|
| Solo founder | Focus on JTBD, Empathy Map, Storyboarding |
| Small team (2-5) | Full empathy work, collaborative ideation |
| Growing team (5-15) | Formalized Personas, structured testing |
| Organization (15+) | Full framework with documented processes |

### By Time Constraint

| Time Available | Focus |
|---------------|-------|
| 1 day | JTBD + POV + Crazy 8s |
| 1 week | Full empathy + define + ideate cycle |
| 1 month | Complete 5-phase cycle with 2 iterations |
| Ongoing | Full framework with continuous reflection |
