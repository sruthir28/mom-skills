---
name: practical-ai-skills
description: Practical frameworks for consulting and product management. Use for strategic problem-solving (SCPR), breaking down complex problems (Issue Trees), building presentation storylines, and prioritizing features/roadmaps (RICE, Impact/Effort, Value/Complexity, Weighted Scoring).
---

# Practical AI Skills

Practical frameworks for non-technical professionals — from consulting to product management.

---

## Available Frameworks

### 1. SCPR Framework
Structure strategic problems and executive communications

### 2. Issue Tree Builder
Break down complex problems with MECE principles

### 3. Storyline Builder
Create presentation decks where each line = one slide

### 4. PM Prioritization
RICE, Impact/Effort, Value/Complexity, Weighted Scoring

---

# 1. SCPR Framework

Structured approach to problem-solving using Situation-Complication-Problem-Recommendation format.

## Framework Components

**S - Situation**: Current state of the market/business
- What is the lay of the land?
- Establish baseline context
- Describe the stable environment before changes

**C - Complication**: Recent shift or change
- What has changed recently?
- New market dynamics (AI boom, regulatory changes, competitive threats)
- The catalyst that creates urgency

**P - Problem**: Crisp question to solve
- What specific strategic question must be answered?
- Must be specific and answerable

**R - Recommendation**: Proposed actions
- What should be done and by when?
- Specific, actionable, time-bound

## Core Principles

**MECE (Mutually Exclusive, Collectively Exhaustive)**
- Recommendations should not overlap
- Together they should cover all necessary actions

**Clarity**
- Each section should be concise
- Problem statement must be answerable
- Recommendations must be actionable

## Example Format

**Situation**
Series B SaaS startup with $15M ARR selling project management software to creative agencies. 200 customers with average contract $75K.

**Complication**
AI-powered tools emerging as workflow automation alternatives. Customer usage declining 15% over last 6 months.

**Problem**
How should we reposition the product and business model to return to 25%+ growth within 12 months?

**Recommendations**
1. **Product**: Launch AI-native workflow engine by Q2
2. **Positioning**: Shift from "project management" to "AI-augmented operations"
3. **Pricing**: Introduce usage-based AI tier

## When to Use
- Structuring strategic arguments
- Creating executive summaries
- Developing clear problem statements
- Writing memos or recommendations

---

# 2. Issue Tree Builder

Break down complex problems into MECE components using hypothesis-driven approach.

## What is an Issue Tree?

Visual hierarchy that decomposes a governing question into increasingly specific sub-questions.

**Key characteristics:**
- Top-down structure (question -> branches -> sub-branches)
- MECE at each level
- Hypothesis-driven
- Actionable at terminal branches

## Framework Components

**Level 0: Governing Question**
- Main strategic question to answer
- Must be specific and answerable

**Level 1: Major Branches (3 branches preferred)**
- Consulting "rule of 3"
- Common structures:
  - Revenue: Price x Quantity x Pipeline
  - Profit: Revenue - Cost
  - Growth: New customers + Expand existing + New products

**Level 2: Sub-branches (Hypotheses)**
- Terminal branches = clear hypotheses to test with data
- Each should be provable/disprovable

## Example

```
How to increase revenue 50% in 18 months?
+-- Average Order Value (Price)
|   +-- Pricing 15% below market - hypothesis: can increase
|   +-- Cart 1.8 items vs industry 2.5 - cross-sell opportunity
+-- Traffic Volume (Quantity)
|   +-- Paid CAC $45 vs LTV $120 - can 2x spend profitably
|   +-- Organic 20% vs 40% competitor - SEO underinvested
+-- Conversion Rate (Pipeline)
    +-- Checkout abandonment 68% vs 58% benchmark - friction
    +-- Mobile 1.2% vs desktop 3.5% - mobile UX broken
```

## Prioritization

```
High Impact + Low Effort = Start here
High Impact + High Effort = Plan carefully
Low Impact + Low Effort = Do if time permits
Low Impact + High Effort = Deprioritize
```

## When to Use
- Beginning of strategic initiative
- Structuring analysis before data work
- Creating work plans with workstreams

---

# 3. Storyline Builder

Build presentation storylines where each line becomes one slide title.

## Core Principles

**Action Titles**
- State findings, not topics
- Good: "Market grew 40% while revenue declined 5%"
- Bad: "Market Analysis"

**Logical Progression**
- Problem -> Context -> Analysis -> Solution -> Roadmap
- Each slide builds on previous

## Storyline Templates

### Market Strategy / Pitch Deck
```
1. [Market] represents $XXB opportunity growing at XX% CAGR
2. We operate in [segment] worth $XXB
3. Top 3 competitors generate $XXM-XXB revenue
4. Our revenue of $XXM positions us as [rank]
5. [Product] addresses [use case] for [target segment]
6. Three growth opportunities identified
7. 18-month roadmap prioritizes [capability 1], [2], [3]
```

### Problem-Solving
```
1. [Problem statement] - current state vs target
2. Problem driven by three factors
3-5. [Each factor with impact quantified]
6. Root cause analysis reveals [key insight]
7-9. Three solution approaches with impact/investment/timeline
10. Prioritize [solution] based on impact/effort
11. Implementation roadmap with phases
```

## When to Use
- Structuring presentation decks
- Building pitch decks
- Creating executive communications

---

# 4. PM Prioritization Framework

## RICE Scoring
**Formula:** `(Reach x Impact x Confidence) / Effort`

| Feature | Reach | Impact | Confidence | Effort (PM) | RICE Score | Rank |
|---------|-------|--------|------------|-------------|------------|------|
| Feature A | 5000 | 2.0 | 100% | 3.0 | 3333 | 1 |

### Impact/Effort Matrix

```
           LOW EFFORT          HIGH EFFORT
         +------------------+------------------+
HIGH     |  QUICK WINS      |   BIG BETS       |
IMPACT   |  Do First        |   Plan & Resource |
         +------------------+------------------+
LOW      |  FILL-INS        |   MONEY PIT      |
IMPACT   |  Do If Time      |   Avoid          |
         +------------------+------------------+
```

### Weighted Scoring
Custom criteria with weights. Common setup:
- Strategic alignment (30%)
- Customer value (25%)
- Revenue potential (20%)
- Effort (15%)
- Risk (10%)

## Framework Selection Guide

| Situation | Framework | Why |
|-----------|-----------|-----|
| Have quantitative data | RICE | Most objective |
| Need quick decision | Impact/Effort | Fast alignment |
| High technical complexity | Value vs. Complexity | Engineering reality |
| Custom business criteria | Weighted Scoring | Flexible |

## When to Use
- Prioritizing product roadmap
- Deciding which features to build
- Allocating team resources
- Making tradeoff decisions

---

## How to Use

Simply ask Claude:
- "Build an SCPR for my product pivot"
- "Create an issue tree for revenue growth"
- "Help me structure a pitch deck storyline"
- "Prioritize these 5 features using RICE"
