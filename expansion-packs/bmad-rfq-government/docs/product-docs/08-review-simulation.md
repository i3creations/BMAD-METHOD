# RFQ Expansion Pack: Review Simulation

## Purpose of this Document

This document describes how the RFQ Expansion Pack uses AI to **simulate evaluator reviews**.  
The goal is to identify compliance gaps, strengthen narratives, and anticipate evaluator findings before submission.

By integrating review simulation, proposal teams can conduct **AI-augmented Pink, Red, and Gold Team reviews** that mirror federal evaluation processes.

---

## Understanding Section M Evaluation Criteria

Federal evaluators score proposals according to **Section M** of the RFQ.  
Common criteria include:

- **Technical**: Solution feasibility, innovation, risk mitigation
- **Management**: Organization, staffing, quality control
- **Past Performance**: Similar scope, size, complexity, CPARS ratings
- **Price**: Realism, reasonableness, balance

Scoring is typically qualitative:

- Strengths
- Weaknesses
- Risks
- Deficiencies

**AI agents must emulate this process** to provide useful review feedback.

---

## AI Prompts for Evaluator-Style Reviews

**Example Prompt:**

```
Review the attached draft Technical Approach against Section M criteria.
Identify strengths, weaknesses, risks, and deficiencies (SWaRD).
Score qualitatively, citing examples from the draft.
Provide recommendations for improvement.
```

**Example Output:**

- **Strength**: Strong evidence of agile methodologies with DHS use cases.
- **Weakness**: Risk mitigation strategies are not quantified.
- **Risk**: Reliance on subcontractors without defined transition plan.
- **Deficiency**: Missing response for SOW Task 3.2 (training support).

---

## Simulated Scoring Grids

AI agents can produce evaluator-style grids for each factor/subfactor.

**Sample Grid:**

| Factor     | Strengths                             | Weaknesses               | Risks                        | Deficiencies     | Overall Assessment                   |
| ---------- | ------------------------------------- | ------------------------ | ---------------------------- | ---------------- | ------------------------------------ |
| Technical  | Agile methods with proven DHS success | Lacks quantified metrics | Subcontractor reliance       | Missing Task 3.2 | Acceptable, some improvements needed |
| Management | Experienced PM with PMP cert          | Org chart lacks clarity  | Moderate staff turnover risk | None             | Acceptable                           |

This format mirrors government evaluation worksheets.

---

## Example Evaluator Feedback

AI-generated feedback can be delivered in evaluator language:

_“The Offeror demonstrated a strong understanding of agile practices and presented relevant past performance examples. However, the lack of quantitative performance metrics reduces the government’s confidence in their ability to measure outcomes. Additionally, the omission of Task 3.2 training support is a material deficiency.”_

This style helps teams prepare for **real evaluator perspectives**.

---

## Integrating Review-Sim Before Pink/Red/Gold Teams

AI Review-Sim agents should be embedded in the review cycle:

1. **Pink Team** — Early check for compliance and section coverage.
   - AI Task: Validate compliance matrix coverage.

2. **Red Team** — Independent evaluator simulation.
   - AI Task: Score proposal sections, identify SWaRD findings.

3. **Gold Team** — Leadership review.
   - AI Task: Generate executive dashboard of strengths/weaknesses.

This ensures **AI feedback is integrated** with traditional human reviews.

---

## Summary

- Review Simulation ensures proposals are **scored before evaluators see them**.
- AI can identify strengths, weaknesses, risks, and deficiencies (SWaRD).
- Simulated scoring grids and evaluator-style language prepare teams for debriefs.
- Embedding Review-Sim into Pink, Red, and Gold Teams strengthens compliance and competitiveness.
