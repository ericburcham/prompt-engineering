# Data Extraction Prompt Guide: Quarterly Earnings Analysis

## Summary

**Extracting Data from Documents with M365 Copilot**  
Learn how to extract specific financial and operational data from complex documents like earnings reports and press releases in the midstream oil and gas industry.

## Explanation

This prompt demonstrates how to efficiently extract key performance metrics from quarterly earnings documents using M365 Copilot.

The prompt works because it:
- Specifies exact data points to extract
- Provides clear output format requirements
- Uses M365's ability to parse complex documents
- Requests data in immediately usable formats (tables, lists)

## The Prompt

```
**TASK:**
Extract key financial and operational metrics from the attached Enterprise Products Partners Q1 2025 earnings report. Create an Excel table with the extracted data and a bulleted summary of significant changes compared to prior periods.

**CONTEXT:**
I am a financial analyst preparing a quarterly performance review for our executive team. We need to benchmark our midstream operations against Enterprise Products Partners' performance, focusing on pipeline throughput, storage utilization, and margin trends. This data will inform our strategic planning session next week.

**REFERENCES:**
Extract the following specific metrics:
- Pipeline volumes by product type (crude oil, NGL, natural gas, petrochemicals)
- Gross operating margins by business segment
- Capital expenditure figures
- Storage capacity utilization percentages
- Fee-based vs. commodity-sensitive revenue split
- Major project updates and completion timelines

Create an Excel table with columns for:
1. Metric Name
2. Q1 2025 Value
3. Q1 2024 Value (if provided)
4. % Change
5. Business Segment
6. Notes/Comments

Also provide a bulleted summary highlighting:
- Top 3 positive performance drivers
- Top 3 challenges or headwinds mentioned
- Major capital projects status
- Forward-looking guidance changes
```

## Evaluation

To evaluate the quality of Copilot's extraction:
- **Accuracy** - Cross-check 2-3 key figures against the source document
- **Completeness** - Verify all requested metrics were found or marked as "not disclosed"
- **Context** - Ensure period comparisons are correctly identified (Q1 2025 vs Q1 2024)
- **Usability** - Is the Excel format ready for immediate analysis?
- **Insights** - Does the summary capture material business drivers?

## Iteration

If the extraction needs refinement:
- **Missing data?** Add "If data not available, note as 'Not disclosed' with page reference"
- **Wrong periods?** Specify "Use calendar Q1 (Jan-Mar) not fiscal quarters"
- **Need more detail?** Add specific page ranges or section names to search
- **Format issues?** Provide example row: "Pipeline - Crude | 2,547 MBPD | 2,422 MBPD | +5.2% | Onshore | Texas System"
- **Want ratios?** Add "Calculate margins as percentage of revenue where possible"