# System Overview

The BMAD RFQ Government Expansion Pack is designed as a modular extension to the BMAD Method core system, providing specialized capabilities for government RFQ proposal development. The architecture follows a service-oriented approach with clear separation of concerns and integration points with the core BMAD infrastructure.

## High-Level Architecture

```mermaid
graph TB
    RFQ[RFQ Project Folder] --> VSCode[VS Code Environment]
    VSCode --> Extensions[VS Code Extensions]
    Extensions --> Analysis[Document Analysis]
    Analysis --> CompMatrix[Compliance Matrix Builder]

    CompMatrix --> Strategy[Strategy Development Service]
    Strategy --> WinThemes[Win Theme Generator]

    CompMatrix --> Content[Content Generation Service]
    WinThemes --> Content

    Content --> Review[Review & Evaluation Service]
    Review --> Export[Export & Submission Service]

    subgraph "BMAD Core Integration"
        Orchestrator[Agent Orchestrator]
        Extensions[VS Code Extensions]
        Templates[Template Engine]
    end

    Extensions --> Analysis
    Orchestrator --> Strategy
    Orchestrator --> Content
    Templates --> Content
```
