# REPORT: AI Subagent Setup Guide: Spec-Driven Development (SDD) Framework

## 1. Introduction to Spec-Driven Development (SDD)

Spec-Driven Development (SDD) mandates a paradigm shift in enterprise engineering. It abandons the "code as documentation" fallacy, where developers reverse-engineer system behavior from the codebase. Instead, SDD establishes natural language specifications as the absolute source of truth. These formal specs serve as the blueprint for designing, implementing, and validating every system component.

In the AI era, shifting from "magical" prompting to "Software Engineering with AI" is non-negotiable. Without standardized engineering processes, the rapid output of AI assistants creates unmanageable entropy.

### The Risks of Unstructured AI Development

- **Exponential Technical Debt:** Since 2022, technical debt---defined as code requiring immediate rework after being committed to a branch---has surged from 1.5% to 6% in environments lacking rigorous SDD standards.

- **Architectural Decay:** Without rigid constraints, AI agents generate rapid but inconsistent code that violates established design patterns, leading to total system chaos within six months.

- **The Validation Bottleneck:** Increasing development speed without automated validation merely shifts the bottleneck. Humans end up spending more time verifying AI output than they would have spent writing it manually.

- **Memory and Detail Exhaustion:** Human memory cannot maintain the level of detail required for modern enterprise tasks; SDD leverages AI to maintain 100% adherence to exhaustive acceptance criteria and technical constraints.

## 2. The Core Toolset: OpenSpec Framework

For existing, complex codebases, the OpenSpec framework is the industry standard. While Spec-Kit is optimized for "Greenfield" (new) projects and BMAT suffers from prohibitive setup complexity, OpenSpec provides the precise balance required for production-level development in established environments.

### OpenSpec Feature Lifecycle Commands

| Command               | Action      | Description |
|-----------------------|------------|-------------|
| `init`                | Initialize | Configures the environment and links AI assistants (e.g., Cursor, Cloud Code). |
| `new`                 | Structure  | Generates the standardized folder structure for a new feature or change. |
| `fast-forward (ff)`   | Artifacts  | Generates the Proposal, BDD Specs, Technical Design, and Task Checklist. |
| `apply`               | Implement  | Executes coding via TDD. Must provide raw terminal/console logs as evidence of success. |
| `verify`              | Validate   | Audits the implementation for completeness and coherence against the spec. |
| `archive`             | Document   | Transitions the "change" into the permanent, formal project documentation. |
| `commit`              | Release    | Triggers Automated AI Code Review (e.g., Code Rabbit) to generate sequence diagrams and PR summaries. |

## 3. Parallel Execution: Git Worktrees

To prevent code collisions and enable high-velocity development, this framework utilizes Git Worktrees. Instead of managing multiple branches within a single directory, worktrees allow autonomous subagents to operate on different features (e.g., Scrum-1, Scrum-2) in completely isolated instances of the codebase. This architectural approach ensures that parallel agent execution never results in local state corruption or dependency conflicts.

## 4. Technical Context Configuration (The Context Recipe)

AI subagents function as senior engineers only when provided with the "Perfect Recipe" of context. This context is stored in version-controlled Markdown files.

### The Three Pillars of Context

1. **Technical Specs:** Tech stack definitions, environment setup, architecture (DDD), file structures, and data relationships.

2. **Workflows:** Systematic steps for TDD, team roles, and mandatory deliverables (e.g., moving a ticket from "Pending" to "Pending Refinement").

3.  **Project-Specific Skills:** Explicit behavioral instructions and technical constraints stored in the `/skills` directory.

### Example `config.yaml` Template:

``` yaml
# OpenSpec Configuration & MCP Hooks
context:
  specs:
    - path: "./docs/tech-stack.md"
    - path: "./docs/architecture-ddd.md"
  workflows:
    - path: "./docs/workflow-tdd.md"
    - path: "./docs/roles.md"
  skills:
    - path: "./docs/skills/react-18-ddd.md"
    - path: "./docs/skills/security-hardened-backend.md"
mcp_hooks:
  jira: "mcp://jira-connector"
  sentry: "mcp://sentry-debug-mode"
```

## 5. Defining Specialist AI Subagent Personas

Every agent must strictly adhere to SOLID and DRY principles. We define three distinct specialist roles:

### Product Strategist

- **Expertise:** Requirements engineering and BDD translation.

- **Behavioral Constraints:** Zero-tolerance for ambiguous requirements; must refine tickets until they are implementation-ready.

- **Core Skills:** Ticket enrichment, defining exhaustive acceptance criteria, and edge-case identification.

### Backend Developer

- **Expertise:** Domain-Driven Design (DDD) and API orchestration.

- **Behavioral Constraints:** Sanitize every input by design; prevent SQL injection and XSS at the architectural level.

- **Core Skills:** API contracts, SOLID compliance, and server-side business logic isolation.

### Frontend Developer

- **Expertise:** React 18 and Frontend DDD.

- **Behavioral Constraints:** Enforce contract-first development and strict state management patterns.

- **Core Skills:** Component lifecycle management, usability/accessibility (A11y), and DDD folder structures for UI state.

## 6. Skill-Based Agent Guidance (The Skills Library)

- **React 18 Standards:** Explicitly define usage of Axios vs. Fetch and list all deprecated features to be avoided. Enforce DDD for
    component organization.

- **Testing Protocols:** Mandate a failing-test-first TDD cycle. Agents must mock database variables and achieve a 90% coverage threshold to prevent the validation bottleneck.

- **Documentation Standards:** Mandatory automated updates for Swagger/OpenAPI and project Markdown files upon every `archive` command.

## 7. Model Context Protocol (MCP) & Debug Mode

MCPs integrate subagents into the external ecosystem for autonomous
operations:

- **Jira (Requirement Enrichment):** The `enrich` command transforms a simple description into an exhaustive technical contract. This process automatically triggers a state change in Jira from "Pending" to "Pending Refinement/Validation."

- **Figma:** Direct design-to-code context for frontend agents.

- **Sentry & Debug Mode:** This specialized mode is designed for autonomous bug fixing. The agent sets breakpoints, monitors Chrome console logs, and reads raw terminal output to diagnose and resolve production threats without human intervention.

## 8. The SDD Operational Workflow: Step-by-Step

1. **Requirement Enrichment:** The Product Strategist transforms a user story into a full technical contract.

2. **Artifact Generation:** Use `fast-forward` to produce the Proposal, Specs (BDD), Design (including technical alternatives), and a granular Task Checklist.

3. **Implementation Phase:** Run `apply`. The agent writes failing tests, implements logic, and provides raw terminal output to verify success.

4. **Automated Verification:** The `verify` command audits the work. The resulting Verify Report identifies critical deviations, such as "Controller fails to return a 400 error for specific invalid IDs."

5. **Archiving & AI Review:** Move changes to permanent docs. The `commit` command triggers an AI reviewer (e.g., Code Rabbit) to generate sequence diagrams and PR summaries.

## 9. Quality Assurance & Technical Debt Prevention

Technical debt is eliminated through a rigorous Definition of Done
(DoD):

- **Unit & Integration Tests:** 100% pass rate with 90% minimum coverage.

- **E2E Validation:** Mandatory browser-based testing for all frontend paths.

- **Manual Endpoint Testing:** Required verification via Curl or similar tools.

- **Verification Evidence:** Implementation is only accepted if supported by terminal logs---never trust an agent's summary alone.

## 10. Conclusion: The AI Product Engineer

The adoption of SDD transitions the developer into the role of an AI Product Engineer. By offloading the "middle" (the tedious execution of coding) to specialized subagents, the engineer focuses on the high-value "edges": Definition/Design and Validation/Verification. This method ensures architectural integrity and speed without the 4x increase in technical debt seen in unstructured AI environments.
