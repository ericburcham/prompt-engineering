# Chain of Thought Prompting Guide: Pipeline Maintenance Scheduling Optimization

## Summary

**Chain of Thought Prompting with M365 Copilot**  
Learn how to prompt AI to explicitly show its reasoning process step-by-step, making complex problem-solving transparent and debuggable.

## Explanation

This prompt demonstrates how to use chain of thought prompting to solve a complex pipeline maintenance scheduling problem while exposing the entire reasoning process.

The technique works because it:
- Forces the model to break down complex problems into steps
- Makes assumptions and logic explicit and verifiable
- Allows you to spot errors in reasoning before accepting conclusions
- Creates auditable decision trails for compliance
- Helps identify which factors most influenced the recommendation

## The Prompt

```
## Configuration

**Behavioral Statements:**

- number all steps
- show calculations
- include units of measurement
- use markdown formatting

**Meta-Directives:**

- think step by step
- provide reasoning for complex decisions
- show calculations
- identify assumptions
- consider edge cases
- question the premise



## Prompt

**TASK:**
Determine the optimal maintenance schedule for our three critical pipeline segments over the next 6 months. Think through this step-by-step, showing all reasoning and calculations at each stage.

**CONTEXT:**
I am the Pipeline Integrity Manager responsible for scheduling maintenance windows that minimize revenue impact while ensuring compliance and safety. We must complete all required maintenance before hurricane season (June 1) while managing customer commitments and operational constraints.

**REFERENCES:**
Pipeline segments requiring maintenance:
- Segment A: Houston to Beaumont crude line (500K bpd capacity, 92% average utilization)
- Segment B: Beaumont to Port Arthur refined products (300K bpd capacity, 78% average utilization)  
- Segment C: Texas City to Houston NGL line (200K bpd capacity, 95% average utilization)

Constraints:
- Each maintenance takes 5 days
- Cannot maintain multiple segments simultaneously (crew limitation)
- Segment A has firm delivery commitments of 450K bpd through March
- Segment C feeds a fractionator with 10-day feedstock storage
- Refined products demand typically drops 20% in February-March
- Maintenance costs increase 30% if done after April 1 (contractor availability)
- Weather delays likely 15% of time in January, 25% in February, 10% in March-May

Please solve this step-by-step:

Step 1: Calculate the revenue impact per day of downtime for each segment. Show your math.

Step 2: Identify the least disruptive month for each segment based on demand patterns and constraints. Explain your reasoning.

Step 3: Consider weather risk factors and adjust timing. Show probability calculations.

Step 4: Evaluate the cost trade-offs between pre-April and post-April maintenance. Display your analysis.

Step 5: Check for constraint violations in your proposed schedule. List each constraint and verify compliance.

Step 6: Propose the final maintenance schedule with rationale for each decision.

Step 7: Identify the key assumptions that most influenced your recommendation and what could change your decision.

After each step, briefly explain why you approached it this way and what alternatives you considered.
```

## Evaluation

To evaluate chain of thought quality:
- **Completeness** - Is every step fully reasoned through?
- **Transparency** - Can you follow the logic at each decision point?
- **Accuracy** - Are calculations shown and verifiable?
- **Alternatives** - Were other options considered and explained?
- **Assumptions** - Are all assumptions explicitly stated?

## Iteration

To improve chain of thought prompting:
- **Need more detail?** Add "Show at least 2 alternatives considered at each step"
- **Want risk analysis?** Include "Calculate confidence levels for each decision"
- **Check logic?** Add "After each step, state what could invalidate this reasoning"
- **Stress test?** Request "Show how schedule changes if key assumptions are wrong"
- **Decision tree?** Ask for "Draw out decision branches at critical choice points"