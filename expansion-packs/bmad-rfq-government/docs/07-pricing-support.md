# RFQ Expansion Pack: Pricing Support

## Purpose of this Document

This document explains how the RFQ Expansion Pack supports **pricing and cost narratives**.  
While AI cannot replace a pricing analyst or contracts officer, it can **assist** with:

- Labor category mapping
- Benchmarking rates
- Drafting pricing narratives
- Identifying risks and assumptions

The result: pricing volumes that are **compliant, realistic, and defensible**.

---

## Role of AI in Pricing

AI agents in this pack do **not calculate final prices**—that remains a finance/contracts responsibility.  
Instead, AI:

- Parses RFQ pricing requirements
- Maps labor categories (LCATs) to contract vehicle equivalents
- Provides benchmark comparisons (from provided rate sheets or historical data)
- Drafts cost/price narratives for compliance with Section L/M
- Highlights assumptions and risks

---

## Mapping LCATs to Government Categories

Most RFQs specify labor categories that must align to:

- **Government-defined categories** (e.g., GSA, IDIQ-specific)
- **Education and experience requirements**
- **Clearances or certifications**

**AI Agent Task**:

- Match company roles to RFQ LCATs
- Flag mismatches (e.g., resume does not meet education requirement)
- Suggest alternative mappings

**Example Prompt**:

```
From the attached RFQ LCAT table and our company labor rate sheet,
map each RFQ role to the closest company role.
Flag any mismatches in education, years of experience, or certifications.
```

---

## Benchmarking Rates with Provided Data

- **Inputs**: Company’s rate sheet, GSA schedule rates, salary benchmarks.
- **AI Function**:
  - Compare company rates to benchmarks
  - Identify where rates may be uncompetitive
  - Highlight categories with potential price realism issues

**Example Output**:

- “Engineer II is priced at $150/hr. Benchmark for similar RFQ roles is $120–130/hr. Consider adjusting or providing justification.”

---

## Drafting Assumptions & Cost Realism Narratives

Pricing narratives must demonstrate **realism and reasonableness**:

- Explain basis of estimate (BOE) for labor hours
- Justify indirect rates, escalation, or subcontractor costs
- State assumptions (e.g., government provides facilities, licenses, or equipment)

**AI Prompt Example**:

```
Draft a pricing narrative based on the attached rate sheet and assumptions.
Include labor mapping methodology, cost realism discussion,
and risk mitigation for cost overruns. Limit to 2 pages.
```

**Sample Narrative Snippet**:
“Our labor categories were mapped directly to RFQ-specified positions using GSA Schedule rates as the basis of estimate. Indirect costs reflect historical audited rates and include escalation at 2% annually. We assume the Government will provide secure workspace and licenses, minimizing overhead.”

---

## Risk Mitigations for Pricing

AI agents can highlight pricing risks such as:

- Underqualified staff assigned to senior LCATs
- Escalation rates outside industry norms
- Subcontractor costs not aligned with BOE
- Unrealistically low labor hours (may trigger “unrealistic pricing” flag)

Each risk should be paired with a **mitigation strategy**:

- Provide resume substitution plan
- Justify escalation based on inflation indices
- Include subcontractor rate agreements

---

## Example Cost Narrative Template

**Pricing Volume Outline:**

1. **Introduction**
   - Overview of pricing methodology
2. **Labor Category Mapping**
   - Table mapping company LCATs → RFQ LCATs
3. **Basis of Estimate**
   - Source of rates (GSA schedule, market benchmarks)
4. **Indirect Costs**
   - Overhead, G&A, fee assumptions
5. **Escalation**
   - Assumptions (e.g., 2% annual)
6. **Assumptions**
   - Dependencies on Government-furnished items (GFIs)
7. **Risk Mitigation**
   - Address potential evaluator concerns
8. **Conclusion**
   - Assurance of cost realism and compliance

---

## Summary

- AI accelerates pricing support by mapping LCATs, benchmarking rates, and drafting cost narratives.
- Humans remain accountable for **final numbers**.
- The combination of AI support + human validation ensures pricing volumes are **compliant, competitive, and defensible**.
