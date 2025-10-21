# Working with Spreadsheets Prompt Guide: RACI Matrix Population

## Summary

**Populating Structured Spreadsheets with M365 Copilot**
Learn how to use M365 Copilot to intelligently populate spreadsheet templates with structured data, leveraging contextual information from multiple worksheets to make informed assignments.

## Explanation

This prompt demonstrates how to use M365 Copilot to automate the population of a RACI (Responsible, Accountable, Consulted, Informed) matrix by analyzing project context from multiple data sources within a workbook.

The prompt works because it:
- References structured data across multiple worksheets
- Provides clear assignment rules and constraints
- Leverages Copilot's ability to understand relationships between data
- Applies business logic consistently across all deliverables
- Uses Excel's native integration with M365 Copilot

## The Prompt

```
**Behavioral Statements:**

- Use technical terminology
- Format for Excel
- Stay focused on the current task
- Use consistent naming conventions
- Include specific examples

**Meta-Directives:**

- Think step by step
- Learn from examples in worksheets
- Verify understanding before proceeding
- Consider multiple perspectives (roles and expertise)
- Prioritize by expertise and capacity



**TASK:**
Using the attached RACI spreadsheet, populate the "RACI Template" worksheet based on the following:

1. **Activities Worksheet**:
   - Each row contains a milestone and its associated deliverable.
   - Example:
     - Milestone: Planning
     - Deliverable: Plan A — Initial draft of the project plan
     - Deliverable: Plan B — Finalized project plan with stakeholder input

2. **Participants Worksheet**:
   - Each row defines either an individual or a team.
   - Includes a brief description of their role.
   - Example:
     - Name: DevOps (Team) — Responsible for deployment and infrastructure
     - Name: Bob Smith (Individual) — Project Manager overseeing planning and execution

3. **Instructions**:
   - For each deliverable, assign:
     - **Responsible (R)**: Who does the work
     - **Accountable (A)**: Who owns the decision (only one per deliverable)
     - **Consulted (C)**: Who provides input
     - **Informed (I)**: Who should be kept in the loop
   - Use job titles or names consistently.
   - Ensure each deliverable has exactly one Accountable party.

**CONTEXT:**
I am a Project Manager setting up governance for a new infrastructure deployment project. I have documented all project milestones, deliverables, and team members with their roles, but need to establish clear accountability for each deliverable. This RACI matrix will be reviewed by stakeholders next week and must reflect realistic work assignments based on each participant's expertise and capacity.

**REFERENCES:**
Please generate RACI assignments for each deliverable in the "RACI Template" worksheet using the context provided in the "Activities" and "Participants" worksheets. Apply these rules:

- Match deliverable types to participant expertise (e.g., design deliverables → designers)
- Assign Accountable (A) to the role with decision authority for that phase
- Assign Responsible (R) to those who execute the work
- Include in Consulted (C) those whose input affects quality or feasibility
- Include in Informed (I) stakeholders who need status updates but don't contribute directly
- Avoid assigning the same person as both Responsible and Accountable unless they're the only resource
- If a team is listed, use the team name (e.g., "DevOps Team") not individual members
```

## Evaluation

To evaluate the RACI assignments:
- **Completeness** - Is every deliverable fully assigned (R, A, C, I)?
- **Logical consistency** - Do assignments match participant roles and expertise?
- **RACI rules** - Exactly one Accountable per deliverable? No conflicts?
- **Workload balance** - Is responsibility distributed reasonably across team?
- **Stakeholder coverage** - Are key decision-makers and stakeholders included appropriately?

## Iteration

To improve the RACI matrix:
- **Unbalanced workload?** Add "Distribute Accountable assignments more evenly across senior team members"
- **Wrong expertise match?** Specify "Technical deliverables should have Engineering as Accountable, not Project Manager"
- **Too many consulted?** Add "Limit Consulted (C) to maximum 3 people per deliverable to avoid decision paralysis"
- **Missing stakeholders?** Include "Ensure Executive Sponsor is Informed for all major milestone deliverables"
- **Ambiguous roles?** Clarify "When both team and individual exist, assign team for execution (R) and individual for accountability (A)"
- **Phase-specific rules?** Add "During Planning phase, Business Analyst should be Accountable; during Execution, Technical Lead should be Accountable"
