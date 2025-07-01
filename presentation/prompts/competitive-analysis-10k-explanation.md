# Prompt Engineering Breakdown: Building an Executive Competitive Analysis Prompt

## Overview
This document deconstructs the thought process and techniques used to create an advanced prompt for competitive analysis in Microsoft Copilot. The goal is to help you understand how to craft prompts that extract maximum value from LLMs when analyzing complex business documents.

## Step-by-Step Thought Process

### Step 1: Understanding the Requirements
**What I identified from the request:**
- **Target User**: EVP/COO (executive level - needs concise, actionable intelligence)
- **Purpose**: Training example for prompt engineering
- **Source Material**: Three 10-K filings (dense, technical documents)
- **Desired Output**: Competitive insights, not just data extraction
- **Context**: Enterprise Products vs. two competitors

**Key Insight**: Executives don't want raw data—they want analyzed, actionable intelligence with clear implications.

### Step 2: Choosing the Prompt Architecture

I selected a **three-phase analytical framework** because:
1. **Data Extraction Phase**: LLMs can miss details if asked to analyze and extract simultaneously
2. **Comparative Analysis Phase**: Separating analysis from extraction improves accuracy
3. **Strategic Implications Phase**: Forces the LLM to move beyond description to prescription

This mirrors how human analysts work: gather data → analyze patterns → draw conclusions.

### Step 3: Implementing Advanced Techniques

#### Technique 1: Role-Based Prompting
```markdown
"You are acting as a strategic analyst preparing a competitive assessment for Graham Bacon, EVP and Chief Operating Officer..."
```
**Why this works**: 
- Establishes expertise level expected
- Names the specific executive (personalizes output)
- Sets professional tone and business context

#### Technique 2: Chain-of-Thought (CoT) Reasoning
```markdown
"For each company, reason through:
1. What is their primary strategic focus based on recent investments?
2. Where are they expanding geographically and why?
3. What customer segments are they prioritizing?
4. How are they positioning for the energy transition?"
```
**Why this works**:
- Forces sequential thinking
- Each question builds on the previous
- Prevents superficial analysis
- Mimics strategic thinking patterns

#### Technique 3: Structured Output with Purpose
Each table includes a strategic column:
- Table 1: "Strategic Implications"
- Table 2: "Analysis"
- Table 4: "Action Required"

**Why this works**:
- Prevents pure data dumps
- Forces interpretation at each step
- Maintains executive focus on "so what?"

#### Technique 4: Progressive Depth Structure
The prompt moves from:
1. **Concrete** (asset counts) →
2. **Financial** (performance metrics) →
3. **Strategic** (positioning analysis) →
4. **Competitive** (relative advantages) →
5. **Forward-looking** (threats/opportunities)

**Why this works**:
- Builds foundation before complex analysis
- Each section informs the next
- Mirrors executive decision-making flow

#### Technique 5: Hypothetical Reasoning
```markdown
"If Williams and Energy Transfer were to merge, how would that change the competitive landscape?"
```
**Why this works**:
- Pushes LLM beyond stated facts
- Demonstrates strategic thinking
- Relevant to M&A considerations
- Shows understanding of industry dynamics

### Step 4: Designing for Executive Consumption

#### Time Horizons
- "Immediate Competitive Threats (0-12 months)"
- "Strategic Opportunities (1-3 years)"

**Why**: Executives think in time-based planning cycles

#### Actionability Requirements
Each recommendation must include:
- Resource requirements
- Implementation timeline
- Expected impact

**Why**: Transforms ideas into executable plans

#### Visual Hierarchy
- Bold key numbers
- One-page executive summary
- Tables for quick scanning

**Why**: Executives scan first, read second

### Step 5: Quality Control Mechanisms

#### Specificity Requirements
```markdown
"Use specific data from the 10-Ks, not generalizations"
"Include page references for key facts"
```
**Why**: 
- Prevents hallucination
- Enables fact-checking
- Builds credibility

#### Focus Directives
```markdown
"Focus on actionable intelligence, not just data compilation"
"Highlight surprising findings or counterintuitive insights"
```
**Why**:
- Differentiates from basic data extraction
- Adds analytical value
- Captures executive attention

## Advanced Techniques Summary

### 1. **Multi-Phase Processing**
- Separates extraction, analysis, and synthesis
- Improves accuracy and depth

### 2. **Contextual Intelligence**
- Role-based prompting
- Named stakeholders
- Industry-specific focus

### 3. **Structured Reasoning**
- Chain-of-thought for complex analysis
- Tree-of-thought for branching scenarios
- Progressive depth architecture

### 4. **Output Optimization**
- Executive-friendly formatting
- Built-in "so what?" analysis
- Action-oriented conclusions

### 5. **Quality Assurance**
- Specific data requirements
- Citation requirements
- Anti-hallucination measures

## Key Lessons for Prompt Engineers

1. **Start with the end user**: An EVP needs different information than an analyst
2. **Structure mirrors thinking**: Good prompts guide LLMs through human reasoning patterns
3. **Specificity prevents drift**: Vague prompts get vague answers
4. **Tables force completeness**: LLMs fill structured templates more thoroughly
5. **Questions drive depth**: Strategic questions produce strategic thinking

## Common Pitfalls Avoided

1. **Information overload**: Limited tables to essential comparisons
2. **Academic analysis**: Focused on business implications, not theory
3. **Data without insight**: Every table includes analysis columns
4. **Generic recommendations**: Required specific, actionable initiatives
5. **Lost context**: Maintained Enterprise Products perspective throughout

## Applying These Techniques

When creating your own advanced prompts:

1. **Define the decision-maker**: Who will use this output?
2. **Map the thinking process**: How would an expert approach this?
3. **Structure for clarity**: Use tables, phases, and clear sections
4. **Build in analysis**: Don't just extract—interpret
5. **Demand specificity**: Vague instructions yield vague results
6. **Test iteratively**: Refine based on output quality

## Conclusion

This prompt demonstrates that effective prompt engineering isn't about clever tricks—it's about understanding how to guide an LLM through complex analytical tasks in a way that produces executive-ready intelligence. The key is structuring the prompt to mirror expert human thinking while leveraging the LLM's ability to process large amounts of information systematically.