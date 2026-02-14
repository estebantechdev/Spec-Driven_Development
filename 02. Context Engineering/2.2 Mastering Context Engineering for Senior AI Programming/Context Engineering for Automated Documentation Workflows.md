# Context Engineering for Automated Documentation Workflows

## Automating Documentation Updates in an AI Workflow

Automating documentation updates within an AI workflow is not about a single tool, but about **Context Engineering**—systematically integrating documentation requirements into the AI's **Definition of Done** and operational blueprint.

To automate this effectively, follow these steps:

### 1. Integrate Documentation into the "Definition of Done"

The most critical step is to explicitly state that a task is not finished unless the documentation is updated. Treat the AI as a developer whose mandatory deliverables include:

- Functional Code  
- Updated Technical Documentation (READMEs, API specs, etc.)  
- Unit Tests  
- A Checklist that the AI must update and verify, explicitly confirming that the documentation has been synchronized with the new code.

### 2. Use "Few-Shot" or "One-Shot" Prompting for Consistency

Instead of letting the AI invent a documentation structure for every task, provide templates or indices.

- **Expert Roles:** Assign the AI a specialized persona, such as an “Expert Architect” or “API Documentation Expert.”  
- **Templates:** Provide the exact index or structure expected (e.g., for a README or an OpenAPI spec). This ensures the AI only fills in relevant sections and maintains a consistent format across the project.

### 3. Verbalize Documentation Triggers in Your Workflow

Document exactly **when** and **what** should be updated based on specific code changes.

- **Standardized Rules:** Create a “Documentation Standards” document that instructs the AI, for example:  
  - “If backend routes change, update the OpenAPI spec.”  
  - “If a new environment variable is added, update the ‘Setup’ section of the README.”  
- **Workflow Phases:** Define documentation as a specific phase in the Software Development Life Cycle (SDLC). This prevents skipping directly to coding and ensures documentation reflection is part of the task.

### 4. Implement Standardized Commands

To reduce dependency on individual prompt-engineering skills, use standardized commands such as `plan ticket` or `develop ticket`. These commands should automatically trigger a **Super Senior Documentation Agent** to:

- Analyze code changes  
- Refer to centralized Technical Specifications (such as data models or API standards)  
- Generate the necessary Markdown or Mermaid diagram updates.

### 5. Centralize Your "Source of Truth"

The AI should not infer documentation patterns from old files. Instead, it should always reference centralized standards such as Testing or Backend Standards.

By providing a large and explicit context (for example, a 1,000+ line standards document), the AI consistently adheres to rules for:

- Error handling

- Security practices

- Logging conventions

- Documentation structure
