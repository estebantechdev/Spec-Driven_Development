# The Architect's Blueprint: Establishing the AI Definition of Done

Architecting the AI Definition of Done

## Definition of Done (DoD) for AI

To define a Definition of Done (DoD) for AI, you must explicitly document and verbalize the standards that a lead or product owner would use to consider a task finished. This ensures the AI does not just “write code” but follows the systematic checklist required by your team.

A robust Definition of Done for AI agents should include the following components:

### 1. Mandatory Deliverables

The AI must be instructed that it cannot consider a task complete unless it delivers a package similar to a human developer. This includes:

- **Functional Code:**

  The primary implementation of the requested feature or fix.

- **Updated Documentation:**

  Any change in code must trigger a corresponding update to technical documentation, such as READMEs, API specifications (OpenAPI), or data models.

- **Unit Tests:**

  A complete set of tests accompanying the new code.

### 2. Quality and Testing Gates

The DoD should incorporate strict, non-negotiable quality metrics that the AI must verify:

- **Test Coverage:**

  A minimum requirement (for example, 90% coverage) for all new functionality.

- **Passing the Suite:**

  All unit tests and end-to-end (E2E) tests (e.g., using Playwright) must pass.

- **Automated Reporting:**

  The AI should emit a report confirming that new tests pass and that no existing functionality has been broken (regression testing).

### 3. Workflow Adherence

The AI must follow the team’s specific Software Development Life Cycle (SDLC) or “blueprint.” This includes:

- **TDD Compliance:**

  If the team uses Test Driven Development, the DoD must require writing tests first, verifying their failure, and only then implementing functional code.

- **Git Standards:**

  Follow the documented Git workflow, including proper branch naming, rebasing when required, and creating a correct pull request.

- **Security and Patterns:**

  Verify that the code avoids documented anti-patterns and adheres to “security by design” principles such as input validation and protection against SQL injection.

### 4. The Verification Checklist

The most effective implementation method is to provide the AI with a checklist that it must update and verify before declaring completion. Commands such as `plan ticket` or `develop ticket` can enforce these phases systematically.

By documenting this **Definition of Done** as part of Context Engineering practices, both AI agents and junior developers using AI can consistently produce senior-level, high-quality output.
