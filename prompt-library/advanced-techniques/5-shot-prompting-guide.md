# No-Shot, One-Shot, and Multi-Shot Prompting Guide

## Summary

**Example-Based Prompting with M365 Copilot**  
Learn when and how to use no-shot (zero examples), one-shot (one example), and multi-shot (multiple examples) prompting techniques to get consistent, formatted outputs for operational tasks.

## Explanation

These prompting techniques control how many examples you provide to guide the AI's response format and style.

- **No-shot**: Direct request without examples - best for straightforward tasks
- **One-shot**: Single example provided - good for showing desired format
- **Multi-shot**: Multiple examples provided - ideal for complex patterns or specific styles

The techniques work because:
- Examples demonstrate exactly what you want
- Patterns help AI understand nuanced requirements
- Multiple examples reinforce consistency
- Format specifications become clearer with demonstration

## Example 1: No-Shot Prompt

```
**Behavioral Statements:**

- follow exact format provided
- use technical terminology
- be concise
- include specific examples

**Meta-Directives:**

- learn from examples
- use examples when helpful
- verify understanding before proceeding



## Prompt

**TASK:**
Generate a safety alert notification for a near-miss incident at our compression station.

**CONTEXT:**
I'm the HSE Manager and need to quickly communicate a near-miss event that occurred this morning when a pressure relief valve activated unexpectedly. No injuries occurred but we need to alert all facilities to check their PRV maintenance records.

**REFERENCES:**
Include: incident location (Brazoria County Station 3), time (09:45 today), equipment involved (Unit 2 discharge PRV), immediate actions taken (unit shutdown, area isolated), and required actions for all facilities (verify PRV test dates within 6 months).
```

## Example 2: One-Shot Prompt

```
**Behavioral Statements:**

- follow exact format provided
- use technical terminology
- be concise
- include specific examples

**Meta-Directives:**

- learn from examples
- use examples when helpful
- verify understanding before proceeding



## Prompt

**TASK:**
Create a daily operations summary following this exact format example.

**CONTEXT:**
I'm the Operations Coordinator preparing standardized daily summaries for management. These need consistent formatting for our dashboard system.

**REFERENCES:**
Follow this format exactly:

EXAMPLE:
Date: 2025-03-15
Total Throughput: 2,847 MBPD (▲ 3.2% vs plan)
System Highlights: 
• Crude: 1,521 MBPD | 98.2% utilization
• NGL: 743 MBPD | 94.7% utilization  
• Refined: 583 MBPD | 91.3% utilization
Issues: Line 200 reduced pressure (450 psi) for pigging operations
Outlook: Return to normal operations by 14:00 tomorrow

Now create today's summary with this data:
- Date: 2025-03-22
- Throughput: 2,792 MBPD (down 1.1% vs plan)
- Crude: 1,502 MBPD at 97.1% utilization
- NGL: 751 MBPD at 95.8% utilization
- Refined: 539 MBPD at 84.4% utilization
- Issues: Beaumont Terminal Tank 107 offline for cleaning
- Outlook: Tank return to service Monday AM
```

## Example 3: Multi-Shot Prompt

```
**Behavioral Statements:**

- follow exact format provided
- use technical terminology
- be concise
- include specific examples

**Meta-Directives:**

- learn from examples
- use examples when helpful
- verify understanding before proceeding



## Prompt

**TASK:**
Write a maintenance work order description following our standard format based on these examples.

**CONTEXT:**
I'm a Maintenance Planner creating work orders for our CMMS system. The descriptions must follow our precise format for consistency and searchability.

**REFERENCES:**
Follow the pattern shown in these examples:

EXAMPLE 1:
WO-2025-1847: PUMP - Replace mechanical seal on P-401A (Crude Charge Pump A). 
Isolation required: XV-401A inlet, XV-401B outlet, drain VI-401C. 
Parts: John Crane Type 2100 seal kit (PN: JC-2100-4.5-316SS).
Duration: 6 hrs. Crew: 2 mechanics, 1 operator. 
Special tools: Seal puller set, dial indicator.

EXAMPLE 2:
WO-2025-1892: VALVE - Repack stem on PCV-7734 (Fractionator Overhead Pressure Control).
Isolation required: Block valves UV-7734A upstream, UV-7734B downstream, bypass open.
Parts: Graphite packing set 1/2" (PN: GP-500-8R-GRAPH).
Duration: 3 hrs. Crew: 2 operators.
Special tools: Packing puller, torque wrench 0-150 ft-lbs.

EXAMPLE 3:
WO-2025-1923: INSTRUMENT - Calibrate FT-1205 (Pipeline Flow Transmitter).
Isolation required: Root valves closed, equalizer open, drain V-1205X.
Parts: None required, calibration only.
Duration: 2 hrs. Crew: 1 instrument tech.
Special tools: Fluke 754 calibrator, test manifold.

Now create a work order for:
Replace bearing on compressor K-301B due to high vibration readings. Need SKF 7320 bearing set. Estimated 8 hours with millwright team.
```

## Evaluation

To evaluate shot-prompting effectiveness:
- **No-shot**: Is output clear without examples? If not, add one example
- **One-shot**: Does output match the example format precisely?
- **Multi-shot**: Are patterns correctly identified and applied?
- **Consistency**: Do repeated uses generate uniform outputs?
- **Complexity match**: Does example quantity match task complexity?

## Iteration

To improve shot-prompting:
- **No-shot failing?** Add one clear example to show desired output
- **One-shot inconsistent?** Add 2-3 more examples to reinforce pattern
- **Multi-shot verbose?** Ensure examples show variety, not redundancy
- **Wrong pattern detected?** Make examples more distinct in key areas
- **Format drift?** Add explicit "follow this exact format" instruction