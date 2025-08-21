# Technical Assumptions

## Repository Structure: Monorepo

The RFQ Expansion Pack will follow BMAD's monorepo structure for expansion packs, with dedicated directories for agents, templates, workflows, and data assets.

## Service Architecture

The expansion pack will leverage BMAD's existing agent orchestration system, implementing specialized agents for proposal functions as modular components. The architecture will maintain separation between:

- RFQ document processing services
- Requirement extraction and compliance mapping
- Content generation and templating
- Review and evaluation simulation

## Testing Requirements

- **Unit Testing**: For core functions like requirement extraction and compliance mapping
- **Integration Testing**: For workflow orchestration between agents
- **User Acceptance Testing**: With proposal professionals using real RFQ documents
- **Compliance Validation**: Automated testing of requirement coverage and traceability

## Additional Technical Assumptions and Requests

- The system will leverage VS Code extensions (Roo Code, Cline, Claude) for reading RFQ documents
- Documents will be organized in project folders with appropriate access controls
- The system will support common RFQ document formats readable by VS Code extensions
- Integration points will be provided for potential future connections to GovWin/GovTribe APIs
- The system will support export to standard proposal formats required by government submission portals
