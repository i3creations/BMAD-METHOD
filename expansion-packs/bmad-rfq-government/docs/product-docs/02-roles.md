# RFQ Expansion Pack: Roles

## Purpose of this Document

This document defines the **roles** required for the RFQ Expansion Pack.  
BMAD operates on a role-based orchestration model: each role represents a **perspective, responsibility, and task set**. By extending BMAD with RFQ-specific roles, we ensure the proposal process is **structured, compliant, and AI-assisted**.

---

## Mapping BMAD Roles to RFQ Process Roles

Below is a mapping between **BMAD roles** and the **government contracting RFQ process**.  
Each role can be human, AI agent, or a **hybrid** (AI generates content, humans refine it).

---

### Business Developer

**Responsibilities:**

- Identify opportunities (SAM.gov, GSA eBuy, IDIQ task orders)
- Conduct quick qualification (vehicle access, NAICS, scope fit)
- Provide capture intelligence (customer priorities, competition, incumbent performance)

**AI Agent Capabilities:**

- Summarize RFQ opportunities from PDFs or portals
- Highlight eligibility criteria
- Generate Bid/No-Bid summary sheets

---

### Capture Manager

**Responsibilities:**

- Define win strategy and teaming approach
- Shape opportunity prior to release (when possible)
- Align solution strengths with evaluation factors
- Ensure customer hot buttons are addressed

**AI Agent Capabilities:**

- Suggest differentiators and win themes
- Benchmark against competitor profiles (if data provided)
- Generate SWOT analysis for opportunity

---

### Proposal Manager

**Responsibilities:**

- Owns proposal schedule and compliance
- Builds compliance matrix
- Assigns sections to SMEs/writers
- Ensures timely delivery

**AI Agent Capabilities:**

- Auto-generate compliance matrices from RFQ
- Produce section outlines mapped to Section L/M
- Monitor draft completion status

---

### Technical SME(s)

**Responsibilities:**

- Provide subject matter expertise for technical approach
- Contribute management, staffing, and solution details
- Supply past performance examples

**AI Agent Capabilities:**

- Generate first-pass technical narratives
- Insert relevant past performance from corpus
- Draft risk mitigation strategies

---

### Pricing/Contracts Lead

**Responsibilities:**

- Map labor categories to RFQ requirements
- Develop pricing strategy and cost realism assumptions
- Ensure contract compliance

**AI Agent Capabilities:**

- Suggest labor mappings based on rate sheets
- Draft cost narratives (assumptions, escalation, basis of estimate)
- Highlight pricing risks

---

### Review Teams (Pink/Red/Gold)

**Responsibilities:**

- **Pink Team**: Early compliance/content check
- **Red Team**: Independent evaluator-style review
- **Gold Team**: Executive messaging and final readiness

**AI Agent Capabilities:**

- Simulate evaluator scoring based on Section M
- Produce Strengths, Weaknesses, Risks, and Deficiencies (SWaRD)
- Flag compliance issues (page limits, missing sections)

---

### Executive Sponsor

**Responsibilities:**

- Approves final proposal
- Ensures bid aligns with corporate strategy
- Signs off on risk posture and pricing

**AI Agent Capabilities:**

- Generate multiple versions of Executive Summary (mission-focused, innovation-focused, price-focused)
- Provide “at-a-glance” dashboards for leadership decision-making

---

## AI Agent Mapping to Roles

| BMAD RFQ Role      | Example AI Agent Function                          |
| ------------------ | -------------------------------------------------- |
| Business Developer | RFQ Opportunity Summarizer                         |
| Capture Manager    | Win Theme Generator & Competitor Analyzer          |
| Proposal Manager   | Compliance Matrix Builder & Outline Generator      |
| Technical SME      | Technical Narrative Drafter & Risk Mitigator       |
| Pricing/Contracts  | Labor Mapping Assistant & Cost Narrative Generator |
| Review Teams       | Evaluator Simulator & Compliance Checker           |
| Executive Sponsor  | Executive Summary Generator & Dashboard Assistant  |

---

## Example Role Definitions (YAML)

Below is an example of how RFQ roles could be expressed in BMAD configuration:

```yaml
roles:
  - name: 'Proposal Manager'
    description: 'Ensures compliance and manages RFQ response'
    ai_agents:
      - compliance_matrix_builder
      - outline_generator

  - name: 'Capture Manager'
    description: 'Defines win strategy and aligns themes'
    ai_agents:
      - win_theme_generator
      - competitor_profiler

  - name: 'Technical SME'
    description: 'Provides solution expertise and past performance'
    ai_agents:
      - technical_drafter
      - risk_mitigator
```

## Summary

- BMAD’s role-based structure is directly extendable to RFQ workflows.
- Each human role has a corresponding AI agent role for automation.
- Roles and agents together form the orchestration backbone of the RFQ Expansion Pack.
