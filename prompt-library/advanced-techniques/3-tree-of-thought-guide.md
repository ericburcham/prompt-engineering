# Tree of Thought Prompting Guide: Terminal Expansion Strategy

## Summary

**Tree of Thought Prompting with M365 Copilot**  
Learn how to explore multiple reasoning paths simultaneously, evaluate their merits, and prune or expand branches to find optimal solutions for complex problems.

## Explanation

This prompt demonstrates how to use Tree of Thought prompting to explore different strategic approaches to a terminal expansion decision.

The technique works because it:
- Generates multiple independent solution paths in parallel
- Allows evaluation and comparison at each decision point
- Enables pruning of weak branches and expansion of promising ones
- Avoids commitment to a single approach too early
- Discovers solutions that linear thinking might miss

## The Prompt

```
**Behavioral Statements:**

- use bullet points
- format for executive presentation
- stay focused on the current task

**Meta-Directives:**

- consider multiple perspectives
- evaluate trade-offs
- compare alternatives
- think like a [operations executive]
- anticipate follow-up questions



## Prompt

**TASK:**
I need to develop a strategy for expanding our Gulf Coast storage terminal capacity. Imagine three different operations executives are proposing the best approach. All executives will present their initial thinking, then refine their ideas through multiple rounds. If any executive's approach proves unviable, they'll be replaced with a new perspective.

**CONTEXT:**
I am the VP of Terminal Operations evaluating options to add 2 million barrels of storage capacity. We have $75M budget, 18-month timeline, and need to maintain operations during construction. The terminal currently stores crude oil and refined products with rail, truck, and pipeline connections.

**REFERENCES:**
Round 1 - Initial Strategies:
Have each executive present their core approach:
- Executive A: Focus on their specialty area
- Executive B: Take a different philosophical approach  
- Executive C: Consider an alternative priority

Each should outline:
1. Their fundamental strategy (build new vs. convert existing vs. acquire nearby)
2. Product mix recommendation (crude, refined, renewable fuels)
3. Key advantages of their approach
4. Primary implementation challenge

Round 2 - Feasibility Analysis:
All executives advance to analyzing feasibility:
- Regulatory/permitting timeline
- Construction complexity during operations
- Customer demand validation
- Financial returns estimate

Share insights between executives. Each can adopt good ideas from others.

Round 3 - Risk Assessment:
Evaluate major risks for each approach:
- Market risk (demand shifts)
- Execution risk (construction delays)
- Competitive risk (competitor expansions)
- Regulatory risk (environmental challenges)

If any approach shows fatal flaws, remove that executive and introduce a new perspective.

Round 4 - Final Recommendation:
Remaining executives present refined strategies incorporating:
- Lessons learned from eliminated approaches
- Best elements from other proposals
- Mitigation plans for identified risks
- Specific implementation roadmap

Then synthesize the best elements into a final recommended strategy.

After each round, explicitly state:
- Which ideas are strongest and why
- What concerns emerged
- Whether any approach should be eliminated
- What new angles to explore
```

## Evaluation

To evaluate tree of thought effectiveness:
- **Diversity** - Are the initial paths genuinely different?
- **Evolution** - Do ideas improve through rounds?
- **Cross-pollination** - Are good ideas shared between branches?
- **Pruning logic** - Is elimination of weak paths justified?
- **Synthesis quality** - Does final solution incorporate best elements?

## Iteration

To enhance tree of thought prompting:
- **More branches?** Start with 5 executives instead of 3
- **Deeper exploration?** Add rounds for technical design and commercial structure  
- **Competitive element?** Have executives critique each other's approaches
- **Wild cards?** Introduce market disruptions mid-process to test adaptability
- **Quantitative scoring?** Add numerical evaluation criteria at each round