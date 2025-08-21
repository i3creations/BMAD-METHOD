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
