# RFQ Expansion Pack: Data Ingestion

## Purpose of this Document

The purpose of this document is to describe how to **ingest, prepare, and structure data** for use with the RFQ Expansion Pack.  
High-quality data ingestion is the foundation of **AI-driven proposal generation**. If data is incomplete, poorly formatted, or non-compliant, the outputs will suffer.

This guide ensures all relevant RFQ materials and corporate assets are captured, organized, and optimized for BMAD agents.

---

## Preparing RFQ Artifacts for AI

Government RFQs are often published as **PDFs, Word documents, or ZIP archives** containing multiple attachments. Each element needs to be ingested, labeled, and parsed.

### Section L (Instructions)

- Defines **how proposals must be formatted and submitted**.
- Includes page limits, file types, margins, font requirements, and submission deadlines.
- AI Extraction: Parse Section L and generate a **submission checklist**.

### Section M (Evaluation Factors)

- Defines **how proposals will be scored** (e.g., Technical, Management, Past Performance, Price).
- Subfactors may include staffing approach, risk management, or transition planning.
- AI Extraction: Tag each evaluation factor with a **response placeholder**.

### Statement of Work / Performance Work Statement (SOW/PWS)

- Describes the **technical tasks and deliverables** the contractor must perform.
- AI Extraction: Break into task IDs (e.g., Task 1.1, 1.2…) for traceability in the compliance matrix.

### Amendments & Q&A

- Often published late in the process.
- May change page limits, due dates, or add new requirements.
- AI Extraction: Run a **diff comparison** between original RFQ and amendments.

---

## Using the BMAD Flattener Tool

BMAD provides a **Codebase Flattener Tool**, originally built for software code ingestion.  
For RFQs, it can be repurposed to:

- Convert **RFQ text, attachments, and corp data** into flattened XML for AI context.
- Normalize diverse formats (Word, PDF, CSV, HTML) into a **consistent structure**.
- Tag each item with metadata (`Section L`, `Section M`, `Past Performance`, etc.).

**Example Command:**

```bash
npx bmad-method flatten --input rfq.zip --output rfq_flattened.xml
```

This produces a machine-readable corpus ready for AI agents.

## Preparing Corporate Data

Beyond the RFQ, proposals require internal data.
AI needs access to these sources to generate accurate drafts.

### Past Performance

- Contract descriptions, period of performance, contract value
- Relevance tags: scope, size, complexity, technology
- AI Usage: Draft Past Performance Narratives tailored to RFQ tasks

### Resumes / Key Personnel

- Skills, certifications, relevant project history
- Map to RFQ-required Key Personnel positions
- AI Usage: Generate tailored resumes and staffing justifications

### Labor Rate Sheets

- GSA schedule rates, IDIQ ceiling rates, or company pricing sheets
- Labor category mappings (Engineer I → Computer Engineer II, etc.)
- AI Usage: Support cost realism narratives and assumptions

---

## Data Redaction & Security

AI ingestion should respect confidentiality:

- Redact PII (e.g., SSNs, personal addresses)
- Mask company-sensitive pricing unless needed for draft generation
- Use tags to mark sensitive data (e.g., <restricted>) so agents know what not to expose in outputs

---

## Building an AI-Ready Corpus

Steps to build a robust corpus for RFQ proposal generation:

1. Collect RFQ artifacts (L, M, SOW, Amendments, Attachments).
2. Run the Flattener Tool to normalize into structured XML.
3. Ingest corporate data (past performance, resumes, rates).
4. Tag sensitive content with redaction labels.
5. Store outputs in /corpus/YYYY-MM-DD/ with version control.
6. Provide agents controlled access to corpus subsets (e.g., Review-Sim agent only sees RFQ + drafts, not internal rate sheets).

## Summary

- Data ingestion is the foundation of AI-driven proposal generation.
- RFQ artifacts (Sections L, M, SOW, Amendments) must be parsed and tagged.
- Corporate data (past performance, resumes, rates) enriches AI outputs.
- BMAD’s Flattener Tool transforms unstructured files into AI-ready XML.
- Redaction ensures compliance and protects sensitive information.
