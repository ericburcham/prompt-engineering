# Data Analysis Prompt Guide: Quarterly Performance Variance Analysis

## Summary

**Data Analysis with M365 Copilot**  
Learn how to analyze operational and financial data from earnings reports to identify trends, calculate variances, and generate actionable insights for midstream operations.

## Explanation

This prompt demonstrates how to perform comprehensive data analysis on quarterly performance metrics using M365 Copilot.

The prompt works because it:
- Specifies exact calculations and comparisons needed
- Requests visual outputs that M365 can generate
- Focuses on variance analysis and trend identification
- Leverages Excel integration for calculations
- Asks for business insights, not just numbers

## The Prompt

```
**TASK:**
Analyze the attached Enterprise Products Partners Q1 2025 earnings data to identify performance trends and calculate key variances. Create visualizations and provide insights on what's driving changes in profitability across business segments.

**CONTEXT:**
I am a Senior Financial Analyst preparing a competitive benchmark analysis for our executive team. We operate similar midstream assets and need to understand Enterprise's performance drivers to inform our own operational strategies. Our CEO specifically wants to know why certain segments are outperforming others and what operational changes might be driving margin improvements or declines.

**REFERENCES:**
Perform the following analysis using the earnings data:

1. Calculate quarter-over-quarter variances for:
   - Pipeline volumes by product type (crude, NGL, natural gas, petrochemicals)
   - Gross operating margins by segment (% change and $ change)
   - Operating costs per barrel/MMBtu for each product type
   - Capital efficiency (EBITDA/CAPEX ratio)

2. Create visualizations:
   - Stacked bar chart: Segment margins Q1 2024 vs Q1 2025
   - Line graph: Volume trends by product over last 5 quarters
   - Waterfall chart: Margin walk from Q1 2024 to Q1 2025
   - Scatter plot: Volume vs. margin by business segment

3. Statistical analysis:
   - Calculate correlation between volumes and margins by segment
   - Identify top 3 positive and negative variance drivers
   - Determine margin sensitivity to volume changes

4. Provide business insights on:
   - Why octane enhancement margins declined $83 million
   - Impact of fee-based contract conversions on propylene business
   - Relationship between maintenance downtime and production volumes
   - Strategic implications of the shift from margin-based to fee-based contracts

Format output with Excel tables for data and embedded charts for visualizations.
```

## Evaluation

To evaluate the analysis quality:
- **Accuracy** - Are calculations mathematically correct?
- **Completeness** - Were all requested analyses performed?
- **Visualization clarity** - Do charts effectively communicate trends?
- **Insight depth** - Do conclusions go beyond stating numbers?
- **Business relevance** - Are findings actionable for strategy?

## Iteration

To enhance the analysis:
- **Need peer comparison?** Add "Compare margins to industry averages from EIA data"
- **Missing context?** Include "Adjust for one-time items and extraordinary events"
- **Want projections?** Add "Extrapolate Q2 performance based on stated guidance"
- **Deeper dive?** Request "Segment volume analysis by geographic region"
- **Risk focus?** Add "Calculate earnings volatility by segment over 8 quarters"