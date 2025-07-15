# Prompt Chaining Guide: Multi-Perspective Summary Synthesis

## Summary

**Prompt Chaining with M365 Copilot**  
Learn how to chain multiple prompts together to create refined outputs by generating different perspectives and synthesizing the best elements into a superior final result.

## Explanation

This prompt chain demonstrates how to create multiple summary variations of a press release, then combine their strongest elements into an impactful final version.

The technique works because it:
- Generates diverse perspectives on the same content
- Identifies the most effective elements from each approach
- Synthesizes strengths while eliminating weaknesses
- Creates output that's better than any single attempt
- Leverages iterative refinement through sequential prompts

## The Prompt Chain

### Prompt 1: Technical Summary
```
## Configuration

**Behavioral Statements:**

- be concise
- use active voice
- maximum 100 words per summary
- no self-reference unless necessary
- write with energy and momentum (for synthesis)

**Meta-Directives:**

- adapt tone and detail level to task type
- focus on actionability
- synthesize before responding
- compare alternatives



## Prompt

**TASK:**
Create a technical summary of the Enterprise Products Partners Q1 2025 earnings press release focusing on operational metrics and engineering achievements.

**CONTEXT:**
I need a summary that highlights operational performance for our engineering team meeting. Focus on throughput, reliability, and technical capabilities.

**REFERENCES:**
Emphasize: pipeline volumes, uptime percentages, capacity utilizations, technical project completions, and operational efficiency metrics. Maximum 100 words.
```

### Prompt 2: Financial Summary
```
**TASK:**
Create a financial-focused summary of the same Enterprise Products Partners Q1 2025 earnings press release emphasizing monetary performance and shareholder value.

**CONTEXT:**
I need a summary for investor relations that highlights financial strength and returns. Focus on profitability and growth.

**REFERENCES:**
Emphasize: EBITDA growth, margin improvements, distribution coverage, capital allocation, and fee-based revenue stability. Maximum 100 words.
```

### Prompt 3: Strategic Summary
```
**TASK:**
Create a strategic summary of the Enterprise Products Partners Q1 2025 earnings press release focusing on market position and competitive advantages.

**CONTEXT:**
I need a summary for the board that demonstrates strategic execution and market leadership. Focus on competitive differentiation.

**REFERENCES:**
Emphasize: market share gains, strategic project progress, customer diversification, integrated value chain benefits, and long-term positioning. Maximum 100 words.
```

### Prompt 4: Synthesis (The Chain Completion)
```
**TASK:**
Review these three summaries of Enterprise Products Partners Q1 2025 results and create a single, impactful 100-word summary that combines the strongest elements of each into a compelling narrative for the company website.

**CONTEXT:**
I'm the Communications Director needing a powerful summary that excites multiple stakeholder groups - employees, investors, and customers. It should be energetic, confident, and memorable.

**REFERENCES:**
Here are the three summaries to synthesize:

[Technical Summary - paste output from Prompt 1]
[Financial Summary - paste output from Prompt 2]  
[Strategic Summary - paste output from Prompt 3]

Combine the most impactful elements from each summary:
- Technical: Pick the most impressive operational achievement
- Financial: Highlight the strongest financial metric
- Strategic: Include the most compelling competitive advantage

Write with energy and momentum. Start with a powerful opening statement. Use active voice and strong verbs. End with forward-looking confidence.
```

## Evaluation

To evaluate the chained output:
- **Integration** - Does it smoothly blend elements from all three sources?
- **Impact** - Is it more compelling than any individual summary?
- **Balance** - Does it address multiple stakeholder interests?
- **Clarity** - Is the message clear despite combining multiple perspectives?
- **Memorability** - Does it stick in the reader's mind?

## Iteration

To enhance prompt chaining:
- **More perspectives?** Add a sustainability-focused summary to the chain
- **Different synthesis?** Try "Create a haiku using the most powerful word from each summary"
- **Audience-specific?** Chain into multiple final versions for different stakeholders
- **Sentiment analysis?** Add intermediate step to identify most positive elements
- **Iterative refinement?** Chain the synthesis output into another refinement prompt