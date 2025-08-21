# RFQ Expansion Pack: Compliance Matrix

## Purpose of this Document

The compliance matrix is the **cornerstone artifact** of every government RFQ response.  
It ensures that every requirement in the solicitation is:

- Identified
- Traced to a proposal section
- Assigned to an owner
- Verified before submission

This document explains how to **create, manage, and automate** compliance matrices using the RFQ Expansion Pack.

---

## Why a Compliance Matrix Matters

- **Mandatory in GovCon**: Missing even one requirement can result in a "non-compliant" rating and automatic rejection.
- **Proposal Manager’s Dashboard**: Tracks progress of assignments and gaps.
- **Evaluator’s Guide**: Shows evaluators exactly where requirements are addressed.
- **Traceability**: Links Section L (instructions), Section M (evaluation), and SOW/PWS (work requirements) to proposal content.

---

## Extracting Requirements from RFQ

Key steps for building a compliance matrix:

1. **Parse RFQ documents**:
   - Section L → Instructions (deliverables, formats, page limits, submission rules).
   - Section M → Evaluation factors and subfactors.
   - SOW/PWS → Technical requirements, tasks, deliverables.
   - Amendments → Any changes to L/M/SOW.

2. **Break down requirements** into discrete items:
   - Avoid lumping multiple requirements into one line.
   - Example: Instead of “Contractor shall provide technical support and training,” create:
     - R-001: Provide technical support
     - R-002: Provide training

3. **Assign identifiers**:
   - Each requirement gets a unique Req ID (R-001, R-002, etc.).
   - IDs should be sequential and traceable.

---

## Compliance Matrix Table Template

The following table format is recommended:

| Req ID | RFQ Text                                   | Source Section | Proposed Response Section        | Owner       | Status  | Evidence            |
| ------ | ------------------------------------------ | -------------- | -------------------------------- | ----------- | ------- | ------------------- |
| R-001  | Contractor shall provide technical support | SOW 3.1        | Section 2.1 – Technical Approach | SME – John  | Draft   | Past Performance #3 |
| R-002  | Contractor shall provide training          | SOW 3.2        | Section 2.2 – Training Plan      | SME – Sarah | Pending | Training Curriculum |

- **Req ID**: Unique identifier.
- **RFQ Text**: Verbatim requirement text.
- **Source Section**: L, M, or SOW reference.
- **Proposed Response Section**: Where it will appear in the proposal.
- **Owner**: Assigned drafter/SME.
- **Status**: Draft, Pending, Final, or Gap.
- **Evidence**: Supporting data (past performance, resumes, rate tables).

---

## Automating Compliance Matrix with AI Agents

The RFQ Expansion Pack includes **Compliance Agents** that:

- Scan RFQ documents and extract requirement statements.
- Generate Req IDs automatically.
- Suggest response locations (map requirements to Section L outline).
- Pre-populate **Proposed Response Section** based on headings.
- Flag ambiguous or missing instructions for human review.

**Example Prompt for Compliance Agent:**

```
From the attached RFQ, extract all requirements in Section L and M.
Create a compliance matrix with Req ID, RFQ Text, Source, and Proposed Response Section.
Assign unique IDs (R-001, R-002, …).
```

---

## Human Validation & Risk Management

Even with automation, human oversight is critical:

- **SME Review**: Ensure technical accuracy of requirement breakdown.
- **Proposal Manager Review**: Confirm all requirements are captured and assigned.
- **Capture Manager Review**: Validate that requirements align to win themes.
- **Compliance Check**: Conduct a final sweep before submission.

**Best Practice:** Run **two independent validations** (Proposal Manager + SME) before freezing the compliance matrix.

---

## Summary

- The compliance matrix guarantees **traceability and compliance** in RFQ responses.
- Requirements must be broken down into **atomic, trackable units**.
- AI agents can accelerate matrix creation but require **human validation**.
- A well-maintained compliance matrix reduces **risk of disqualification** and improves proposal quality.
