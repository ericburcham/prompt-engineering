# Behavioral Statements and Meta-Directives Reference Guide

## Summary

**Behavioral Statements** are explicit instructions that control the style, format, and communication approach of AI responses. They shape HOW the AI delivers information - its tone, structure, and presentation style.

**Meta-Directives** are higher-level instructions that influence the AI's cognitive approach and problem-solving methodology. They guide HOW the AI thinks about and processes your request, affecting the depth and quality of analysis.

Using these configurations helps you get consistent, predictable outputs tailored to your specific needs. They're particularly valuable when creating standardized reports, operational procedures, or when you need responses formatted for specific audiences or systems.

## Behavioral Statements

| Statement | Description |
|-----------|-------------|
| **Be concise** | Eliminates verbose explanations; delivers only essential information |
| **Use markdown formatting** | Structures output with headers, bullets, tables, and code blocks |
| **Ask clarifying questions** | Prompts for missing information before proceeding with incomplete requests |
| **Stay focused on the current task** | Prevents tangential information; maintains strict relevance to request |
| **No apologies or disclaimers** | Removes "I apologize," "I'm sorry," and unnecessary hedging language |
| **No self-reference unless necessary** | Eliminates "As an AI" or "I can help you" unless specifically relevant |
| **Use bullet points** | Formats lists and key points as bullets rather than paragraphs |
| **Include specific examples** | Provides concrete illustrations rather than abstract descriptions |
| **Write in active voice** | Uses direct, action-oriented language (e.g., "Execute the plan" vs "The plan should be executed") |
| **Target [audience] reading level** | Adjusts complexity for executives, engineers, operators, or other groups |
| **Number all steps** | Creates numbered sequences for procedures and instructions |
| **Highlight key metrics** | Bolds or emphasizes important numbers and measurements |
| **Use technical terminology** | Employs industry-specific language without simplification |
| **Avoid jargon** | Explains concepts in plain language for broader audiences |
| **Include units of measurement** | Always specifies bbls, MBPD, PSI, etc. with values |
| **Cite sources** | References specific documents, standards, or regulations |
| **Format for [system]** | Adapts output for Excel, SAP, CMMS, or other platforms |
| **Maximum [X] words/sentences** | Enforces strict length limits for summaries or reports |

## Meta-Directives

| Directive | Description |
|-----------|-------------|
| **Think step by step** | Breaks down complex problems into sequential logical components |
| **Adapt tone and detail level to task type** | Varies approach based on technical analysis vs. executive summary vs. operational procedure |
| **Verify understanding before proceeding** | Restates the request to confirm correct interpretation |
| **Use examples when helpful** | Illustrates abstract concepts with concrete scenarios |
| **Provide reasoning for complex decisions** | Shows the logic chain behind recommendations |
| **Consider multiple perspectives** | Analyzes from operational, financial, safety, and strategic viewpoints |
| **Identify assumptions** | Explicitly states what must be true for analysis to hold |
| **Evaluate trade-offs** | Weighs pros and cons of different approaches |
| **Prioritize by [criteria]** | Ranks options by safety, cost, efficiency, or other factors |
| **Show calculations** | Displays mathematical work for verification |
| **Consider edge cases** | Addresses unusual scenarios and exceptions |
| **Validate against standards** | Checks recommendations against industry regulations |
| **Think like a [role]** | Adopts perspective of operator, executive, regulator, etc. |
| **Question the premise** | Challenges assumptions in the original request if problematic |
| **Synthesize before responding** | Combines multiple information sources before answering |
| **Structure hierarchically** | Organizes information from general to specific |
| **Compare alternatives** | Presents multiple options with comparative analysis |
| **Focus on actionability** | Emphasizes practical next steps over theory |
| **Anticipate follow-up questions** | Addresses likely concerns proactively |
| **Learn from examples** | Extracts patterns from provided samples to guide output |

## Usage Tips

**Combining Statements and Directives:**
```
Be concise, use bullet points, and think step by step. Focus on actionability 
and provide reasoning for complex decisions. Target operations manager reading level.
```

**For Operational Reports:**
```
Use markdown formatting, include units of measurement, highlight key metrics. 
Show calculations and validate against API standards. Maximum 500 words.
```

**For Executive Communications:**
```
Be concise, no technical jargon, stay focused on business impact. 
Prioritize by financial criteria and provide reasoning for recommendations.
```

Remember: The more specific your behavioral statements and meta-directives, the more consistent and tailored your AI outputs will be. Experiment with combinations to find what works best for your recurring tasks.