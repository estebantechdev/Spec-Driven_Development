# REPORT - Enterprise Blueprint for Specialized AI Subagents in Spec-Driven Development

## 1. The Foundation of Spec-Driven Development (SDD)

As a Lead AI Platform Engineer who has scaled teams from 50 to 500 engineers at organizations like WFOX and Revolut, I have observed a critical shift in the development landscape. Since the mass adoption of AI coding assistants in 2022, technical debt has multiplied dramatically—rising from a stable 1.5% to over 6% in mere months. This surge in unmanaged complexity stems from treating AI as a coding shortcut rather than as an engineering framework.

Spec-Driven Development (SDD) is the structured response to this systemic drift. It redefines engineering as a measurable and predictable discipline. In SDD, the **Specification (Spec)** is the formal contract and the single source of truth for system design, implementation, and validation.

By leveraging frameworks such as OpenSpec (or alternatives like Kiro, Spec Kit, GSD, and BMAD), the cost of generating exhaustive engineering contracts approaches zero. Human engineers shift toward high-level design and rigorous validation, while AI systems execute dense implementation logic.

### Core Characteristics of a Valid Spec

- **Exhaustiveness**  

  The Spec must eliminate ambiguity. It explicitly defines behaviors, including failure states (404, 500), JSON structures, and edge cases.

- **Validability**  

  Every requirement must be testable. Engineering demands proof. Validation must be automatable and objective.

## 2. Configuration of Specialized AI Subagents

SDD at enterprise scale requires highly specialized subagents. While the methodology is tool-agnostic (Cursor, Claude Code, Windsurf, etc.), each agent’s internal skill configuration must be precise and role-driven.

### Backend Developer Subagent

The following directives define the operating contract for a Senior Backend Systems Architect.

```md
#### PERSONA AND ARCHITECTURAL PHILOSOPHY

You are a Senior Backend Systems Architect specializing in high-scale distributed systems. Your mission is to implement secure, robust, and maintainable systems that strictly follow Domain-Driven Design (DDD) and SOLID principles. Architectural integrity takes precedence over delivery speed.

### DOMAIN-DRIVEN DESIGN (DDD) PROTOCOLS

1. **Layer Separation**  

   Strict isolation of Domain Model, Application Services, and Infrastructure.

2. **Value Objects**  

   Use strongly validated value objects (Email, Currency, etc.) instantiated with enforced constraints.

3. **Service Layer Discipline**  

   Application services coordinate workflows but do not embed business rules.

### API CONTRACT AND INTERFACE STANDARDS

1. **Strict Contracts First**

2. **Complete HTTP Coverage**

   - 200/201 – Success  

   - 400 – Validation errors (clear field-level feedback)  

   - 401/403 – Auth failures  

   - 404 – Not found  

   - 500 – Unexpected exceptions  

3. **Standardized JSON**

   - camelCase keys  

   - ISO-8601 date-time strings  

4. **Versioning**

   - Breaking changes via `/v1/`, `/v2/`

### PERSISTENCE AND DATA INTEGRITY

- Avoid N+1 queries  

- Use transactions for multi-entity operations  

- Enforce versioned migration scripts  

### CYBERSECURITY AND DATA PROTECTION

- Parameterized queries only  

- Full input sanitization  

- No stack trace leakage  

- Least-privilege DB access  

### TEST-DRIVEN DEVELOPMENT (TDD)

- Red-Green-Refactor cycle mandatory  

- Mock all external dependencies  

- Boundary and edge-case coverage required  

### PERFORMANCE AND RELIABILITY

- Circuit breaker patterns  

- Caching (Redis where specified)  

- Structured logging with trace IDs  

### SPEC COMPLIANCE

- Full traceability to Spec requirements  

- Synchronized Swagger/OpenAPI documentation  

```

### Frontend Developer Subagent

**Focus:** React 18, design fidelity, and modular architecture.

- Advanced React 18 usage (Concurrent Rendering, Transitions)  

- Pixel-perfect implementation via Figma integration  

- Modular component structure (Atomic or Feature-Based)  

- Consistent state management strategy  

- Standardized data-fetching approach (Axios or Fetch as defined)

### Product Strategist Subagent

**Focus:** Business intent and user story precision.

- Converts raw requirements into exhaustive user stories  

- Bridges product and engineering  

- Protects alignment between architecture and business value  

### Subagent Mapping Table

| Subagent Role        | Core Responsibilities                              | Engineering Principles Enforced |
|----------------------|---------------------------------------------------|----------------------------------|
| Backend Developer    | API Design, Security, Data Integrity              | SOLID, DRY, TDD, Clean Architecture |
| Frontend Developer   | React 18, UI/UX Fidelity, Accessibility           | DRY, Modularity, Accessibility |
| Product Strategist   | Story Enrichment, BDD, Business Validation        | Business Alignment, Acceptability |

## 3. Repository-Based Technical Context Architecture

To prevent documentation decay, all context must live inside the repository as Markdown files.

### Implementation Standards

- **Git Worktrees** for parallel agent execution  
- **Context Files** defining:

  - Stack & versions (React 18, Node.js, etc.)

  - Architecture patterns

  - Mandatory principles (TDD, SOLID, DRY)

## 4. Leveraging Model Context Protocols (MCPs)

MCPs enable subagents to interact directly with engineering tools.

### Jira MCP & `enrich`

- `enrich [Ticket-ID]`

- Injects technical contracts into raw tickets

- Moves status to "Pending Refinement"

- Requires active authentication

### Figma MCP

Direct design-token ingestion for frontend accuracy.

### Sentry MCP

Autonomous error analysis and proactive PR generation.

### Git / Terminal Integration

Agents execute tests, manage branches, and verify endpoints via `curl`.

## 5. The SDD Operational Workflow

1. **new** – Initialize change structure  

2. **ff / continue** – Generate:

   - Proposal (Why)

   - Specs (BDD scenarios)

   - Design Decisions

   - Implementation Checklist  

3. **apply** – TDD-based implementation  

4. **verify** – Automated audit:

   - Completeness

   - Correctness

   - Coherence  

5. **archive** – Convert change into permanent Delta update  

## 6. Engineering Quality & Validation Standards

**Definition of Done (DoD):**

- 90% minimum test coverage  

- Unit, Integration, and E2E validation  

- Mandatory SQLi/XSS sanitization  

- Automated AI PR review  

- Generated sequence diagrams  

## 7. The AI Product Engineer: The Golden Triangle

Modern engineering excellence requires mastery of:

1. **AI Systems & SDD**

2. **Architecture & Technical Vision**

3. **Cross-Functional Collaboration**

This triad defines the AI Product Engineer.

## 8. Implementation Commands Summary

| Command | Action |
|---------|--------|
| enrich [Ticket-ID] | Fetches and enriches Jira ticket |
| openspec init | Initializes SDD configuration |
| new | Creates feature directory structure |
| ff | Generates Proposal, Spec, Design, Tasks |
| continue | Generates artifacts sequentially |
| apply | Executes implementation via TDD |
| verify | Automated audit of work |
| archive | Converts change into Delta |
| commit | Prepares PR with AI-generated summary |

## 9. Conclusion

By embedding architectural rigor, repository-based context, and specialized AI subagents, Spec-Driven Development transforms AI from a coding accelerator into an enterprise engineering framework.
