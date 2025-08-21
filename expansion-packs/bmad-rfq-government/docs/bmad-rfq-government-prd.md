# Product Requirements Document: BMAD RFQ Government Expansion Pack

## 1. Executive Summary

The BMAD RFQ Government Expansion Pack extends the BMAD Method into the domain of government contracting proposal development, specifically for Requests for Quotes (RFQs). This expansion pack provides a structured approach to AI-driven proposal generation that empowers capture teams, proposal managers, and subject matter experts to rapidly create compliant, competitive, and compelling proposals while maintaining the rigor and discipline required in federal contracting.

### 1.1 Problem Statement

Responding to government RFQs is a resource-intensive process that requires:

- Strict adherence to Section L (Instructions) and Section M (Evaluation Criteria)
- Detailed compliance matrices
- Technical, management, staffing, and past performance narratives
- Pricing narratives and assumptions
- Formatting and submission compliance

Proposal teams often struggle with:

- Time pressure (short RFQ deadlines, often < 14 days)
- Volume of content to generate
- Complexity of compliance requirements
- Consistency across multiple proposals

### 1.2 Solution Overview

The BMAD RFQ Government Expansion Pack leverages AI within the BMAD framework to:

- Accelerate draft creation (hours instead of days or weeks)
- Ensure compliance traceability from requirements to response
- Standardize outputs across proposals
- Reduce costs by cutting labor hours spent on repetitive drafting

## 2. Product Scope

### 2.1 Key Features

1. **Role-Based Orchestration**
   - Domain-specific roles (Capture Manager, Proposal Manager, etc.)
   - AI agent configurations that simulate those roles
   - Hybrid approach (AI generates content, humans refine it)

2. **Data Ingestion**
   - Conversion of RFQ text, attachments, and corporate data into structured format
   - Parsing of Section L, Section M, SOW/PWS, and amendments
   - Leveraging BMAD's Flattener Tool for consistent structure

3. **Compliance Matrix Generation**
   - Automated extraction of requirements from RFQ documents
   - Unique identifier assignment for each requirement
   - Mapping requirements to proposal sections
   - Status tracking and validation

4. **Win Theme Development**
   - Structured approach to creating persuasive win themes
   - Linking win themes to evaluation factors
   - AI prompts for drafting differentiators
   - Checklist for strong win themes

5. **Proposal Drafting**
   - AI-generated content for major proposal sections
   - Customizable prompt templates
   - Integration of compliance matrix and win themes
   - Structured drafting workflow

6. **Pricing Support**
   - Labor category mapping
   - Rate benchmarking
   - Cost narrative generation
   - Risk identification and mitigation strategies

7. **Review Simulation**
   - AI-simulated evaluator reviews
   - Identification of strengths, weaknesses, risks, and deficiencies
   - Simulated scoring grids
   - Integration with Pink/Red/Gold Team reviews

8. **Submission Checklist**
   - Formatting and compliance verification
   - AI white glove compliance check
   - File organization and naming conventions
   - Amendment handling

9. **Continuous Improvement**
   - Debrief feedback capture
   - Prompt library updates
   - Versioning and changelog
   - Performance metrics tracking

### 2.2 Target Users

- Government Contractors (both primes and subs)
- Proposal & Capture Teams (managers, writers, reviewers, SMEs)
- Business Developers (identifying and qualifying opportunities)
- Executives (sponsoring bids and approving themes)
- AI/Automation Engineers (implementing and tuning the pack within BMAD)

### 2.3 Integration with BMAD

The RFQ Expansion Pack builds on BMAD's role-based orchestration and:

- Introduces domain-specific roles
- Provides AI agent configurations
- Includes prompt libraries and workflow pipelines
- Supplies templates for compliance matrices, proposal sections, and checklists
- Leverages BMAD's Flattener Tool

## 3. Detailed Requirements

### 3.1 Role Definitions

| Role                   | Responsibilities                                                               | AI Agent Capabilities                                                                                        |
| ---------------------- | ------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------ |
| Business Developer     | Identify opportunities, conduct qualification, provide capture intelligence    | Summarize RFQ opportunities, highlight eligibility criteria, generate Bid/No-Bid summary sheets              |
| Capture Manager        | Define win strategy, shape opportunity, align solution strengths               | Suggest differentiators and win themes, generate SWOT analysis, benchmark against competitor profiles        |
| Proposal Manager       | Own proposal schedule and compliance, build compliance matrix, assign sections | Auto-generate compliance matrices, produce section outlines, monitor draft completion status                 |
| Technical SME(s)       | Provide subject matter expertise, contribute management and solution details   | Generate first-pass technical narratives, insert relevant past performance, draft risk mitigation strategies |
| Pricing/Contracts Lead | Map labor categories, develop pricing strategy, ensure contract compliance     | Suggest labor mappings, draft cost narratives, highlight pricing risks                                       |
| Review Teams           | Conduct Pink/Red/Gold Team reviews                                             | Simulate evaluator scoring, produce SWaRD findings, flag compliance issues                                   |
| Executive Sponsor      | Approve final proposal, ensure bid aligns with corporate strategy              | Generate multiple versions of Executive Summary, provide dashboards for decision-making                      |

### 3.2 Data Ingestion Requirements

1. **RFQ Artifact Processing**
   - Parse PDFs, Word documents, and ZIP archives
   - Extract Section L (Instructions)
   - Extract Section M (Evaluation Factors)
   - Extract Statement of Work / Performance Work Statement (SOW/PWS)
   - Process amendments and Q&A

2. **BMAD Flattener Tool Integration**
   - Convert diverse formats into consistent structure
   - Tag items with metadata
   - Support command-line interface for processing

### 3.3 Compliance Matrix Requirements

1. **Requirement Extraction**
   - Parse RFQ documents (Section L, Section M, SOW/PWS, Amendments)
   - Break down requirements into discrete items
   - Assign unique identifiers

2. **Matrix Structure**
   - Req ID
   - RFQ Text
   - Source Section
   - Proposed Response Section
   - Owner
   - Status
   - Evidence

3. **AI Automation**
   - Scan RFQ documents and extract requirement statements
   - Generate Req IDs automatically
   - Suggest response locations
   - Pre-populate Proposed Response Section
   - Flag ambiguous or missing instructions

### 3.4 Win Theme Requirements

1. **Win Theme Structure**
   - Claim: What you offer
   - Proof: Evidence
   - Benefit: Why it matters to the customer
   - Risk Reduction: How it reduces risk

2. **Theme Characteristics**
   - Customer-Centric
   - Evidence-Based
   - Evaluator-Focused
   - Differentiated
   - Repeatable

3. **AI Prompts**
   - Generate themes aligned to evaluation criteria
   - Include claim, proof, benefit, and risk reduction
   - Ensure customer-centricity and differentiation

### 3.5 Proposal Drafting Requirements

1. **Section Generation**
   - Executive Summary
   - Technical Approach
   - Management Plan
   - Staffing & Key Personnel
   - Past Performance Narratives

2. **Prompt Templates**
   - Customizable with placeholders
   - Reusable, repeatable drafting workflows

3. **Integration**
   - Compliance Matrix Integration
   - Win Themes Integration
   - Traceability through requirement IDs

4. **Workflow**
   - Load Corpus
   - Generate Section Drafts
   - Insert Win Themes
   - Human Review
   - Review-Sim Pass
   - Finalize

### 3.6 Pricing Support Requirements

1. **Labor Category Mapping**
   - Match company roles to RFQ LCATs
   - Flag mismatches
   - Suggest alternative mappings

2. **Rate Benchmarking**
   - Compare company rates to benchmarks
   - Identify uncompetitive rates
   - Highlight price realism issues

3. **Cost Narrative Generation**
   - Draft pricing narratives
   - Include basis of estimate, indirect costs, escalation, assumptions
   - Address risk mitigations

### 3.7 Review Simulation Requirements

1. **Evaluator Simulation**
   - Understand Section M evaluation criteria
   - Identify strengths, weaknesses, risks, and deficiencies (SWaRD)
   - Generate qualitative scoring

2. **Scoring Grids**
   - Factor-based assessment
   - Strengths, weaknesses, risks, deficiencies columns
   - Overall assessment

3. **Review Integration**
   - Pink Team: Early compliance check
   - Red Team: Independent evaluator simulation
   - Gold Team: Leadership review

### 3.8 Submission Checklist Requirements

1. **Formatting Verification**
   - Page limits
   - Fonts and sizes
   - Margins and line spacing
   - File formats
   - File naming conventions

2. **White Glove Compliance Check**
   - Validate compliance matrix coverage
   - Confirm requirements are addressed
   - Check formatting and pagination
   - Verify document headers/footers
   - Ensure acronyms are defined

3. **File Organization**
   - Folder structure
   - Naming conventions
   - Amendment handling

### 3.9 Continuous Improvement Requirements

1. **Debrief Capture**
   - Log evaluator comments
   - Tag feedback by section
   - Cross-reference with compliance matrix IDs
   - Store positive and negative themes

2. **Prompt Library Updates**
   - Identify relevant evaluator feedback
   - Update prompt instructions
   - Maintain version history

3. **Versioning**
   - Semantic versioning
   - Changelog maintenance

4. **Performance Metrics**
   - Proposal Development KPIs
   - Business Development KPIs
   - AI Performance KPIs

## 4. Technical Requirements

### 4.1 BMAD Integration

1. **Directory Structure**
   - `/expansion-packs/bmad-rfq-government/`
   - `/agent-teams/` - Team configurations
   - `/agents/` - Agent definitions
   - `/checklists/` - Compliance and quality checklists
   - `/data/` - Knowledge base and reference data
   - `/docs/` - Documentation
   - `/tasks/` - Task definitions
   - `/templates/` - Document and prompt templates
   - `/workflows/` - Process workflows

2. **Configuration**
   - `config.yaml` with expansion pack metadata
   - Role definitions in YAML format
   - Agent configurations

### 4.2 AI Agent Requirements

1. **Agent Types**
   - RFQ Opportunity Summarizer
   - Win Theme Generator & Competitor Analyzer
   - Compliance Matrix Builder & Outline Generator
   - Technical Narrative Drafter & Risk Mitigator
   - Labor Mapping Assistant & Cost Narrative Generator
   - Evaluator Simulator & Compliance Checker
   - Executive Summary Generator & Dashboard Assistant

2. **Prompt Engineering**
   - Structured prompts for each agent function
   - Templating system with placeholders
   - Version control for prompts

### 4.3 Data Processing

1. **Input Formats**
   - PDF documents
   - Word documents
   - Excel spreadsheets
   - ZIP archives

2. **Output Formats**
   - Structured proposal sections
   - Compliance matrices
   - Review reports
   - Submission checklists

## 5. Implementation Plan

### 5.1 Development Phases

1. **Phase 1: Core Framework**
   - Role definitions
   - Basic agent configurations
   - Directory structure setup
   - Configuration files

2. **Phase 2: Data Ingestion & Compliance**
   - Flattener Tool integration
   - Compliance matrix generation
   - Requirement extraction

3. **Phase 3: Content Generation**
   - Win theme development
   - Proposal section drafting
   - Pricing support

4. **Phase 4: Review & Submission**
   - Review simulation
   - Submission checklist
   - White glove compliance check

5. **Phase 5: Continuous Improvement**
   - Debrief capture system
   - Versioning and changelog
   - KPI tracking

### 5.2 Testing Strategy

1. **Unit Testing**
   - Individual agent functionality
   - Prompt effectiveness
   - Data processing accuracy

2. **Integration Testing**
   - End-to-end workflow testing
   - BMAD core integration
   - Cross-agent communication

3. **User Acceptance Testing**
   - Real RFQ processing
   - Proposal team feedback
   - Compliance verification

### 5.3 Documentation

1. **User Documentation**
   - Getting started guide
   - Role-specific instructions
   - Prompt libraries
   - Best practices

2. **Technical Documentation**
   - Architecture overview
   - Agent configurations
   - Integration points
   - Customization guide

## 6. Success Metrics

1. **Efficiency Metrics**
   - Time to first draft (target: <48 hours)
   - Number of review cycles needed (target: decreasing trend)
   - Labor hours saved per proposal

2. **Quality Metrics**
   - Compliance coverage (target: 100%)
   - Evaluator strengths vs. weaknesses ratio
   - Incidence of compliance deficiencies (target: zero)

3. **Business Impact**
   - Win rate improvement
   - Number of proposals submitted
   - Revenue impact

## 7. Future Roadmap

1. **Near-Term Enhancements**
   - Fine-tuned LLMs on past proposal language
   - Resume Tailoring Agent
   - Orals/Slides Generator

2. **Mid-Term Enhancements**
   - Auto-Amendment Diff Checker
   - Integration with GovWin/GovTribe APIs
   - Advanced analytics dashboard

3. **Long-Term Vision**
   - End-to-end RFQ lifecycle management
   - Predictive win probability modeling
   - Automated debrief analysis and incorporation

## 8. Appendices

### 8.1 Glossary

- **RFQ**: Request for Quote
- **Section L**: Instructions section of an RFQ
- **Section M**: Evaluation criteria section of an RFQ
- **SOW/PWS**: Statement of Work / Performance Work Statement
- **LCAT**: Labor Category
- **SWaRD**: Strengths, Weaknesses, Risks, and Deficiencies
- **Pink/Red/Gold Teams**: Progressive review stages for proposals

### 8.2 Reference Materials

- Federal Acquisition Regulation (FAR)
- Agency-specific acquisition guidelines
- BMAD Method documentation
