# AI Development "Definition of Done" (DoD) Framework & Template

## 1. Executive Overview of AI Context Engineering

In high-scale AI-assisted engineering, **context** is the non-negotiable pillar of performance. To move beyond individual productivity and achieve collective transformation, AI agents must be treated as senior-level collaborators that require precise environmental boundaries.

**Golden Rule of Context Engineering:**

Never allow the AI to determine standards through prompts or by inferring patterns from the existing codebase. Standards must be enforced through documented **“Golden Standard” files.**

### The Three Ingredients of the Perfect AI Recipe

1. **Technical Specifications** – The granular *“What”* of the project.  

2. **Workflow** – The procedural *“How”* of the team’s SDLC.  

3. **Task-Specific Input** – External requirement (ticket, bug report, or feature request).

**Objective:** Eliminate prompt dependency and ensure any agent, regardless of user seniority, produces senior-grade, production-ready output.

## 2. The Technical Specification Layer (The “What”)

Before development begins, a set of **Context Files** must exist. These files are exhaustive (often exceeding 1,000 lines) and define both mandatory implementations and forbidden anti-patterns.

### Tech Stack & Environment (Step Zero)

- **Mandatory Documentation:** Exhaustive tech stack listings with versions and intended use cases.

- **Environment Setup:** Step-by-step instructions for running environments from scratch, independent backend/frontend execution, and database seeding with sample data.

- **Variable Management:** Strict prohibition of hardcoded secrets; mandatory use of `.env` and updated `.env.example` templates.  

### Architecture & File Structure

- **Pattern Enforcement:** Explicit mapping of Hexagonal Architecture or Domain-Driven Design (DDD).

- **Anti-Pattern Catalog:** A “How Not To” section listing legacy patterns that the AI must never imitate.  

### Data Modeling & Stakeholder Autonomy

- **Natural Language Modeling:** Every data field and relationship described in natural language.

- **Mermaid Integration:** Markdown-compatible Mermaid diagrams for visualization.

- **Non-Technical Autonomy:** Enables stakeholders to query business logic using their own AI tools.  

### Design Patterns & Security by Design

- **Standard Adherence:** Alignment with Clean Code and SOLID principles; defined use of structural patterns (Factory, Decorator).

- **Defensive Programming:** Mandatory SQL Injection, XSS, and CORS checks.

- **Logging & Errors:** Prescriptive error handling and logging standards for observability.

## 3. The Workflow & SDLC Layer (The “How”)

The AI must adhere to a documented **SDLC Blueprint** to prevent premature coding.

- **Git Workflow:** Enforced branch naming, rebasing vs merging rules, and mandatory PR structures.

- **TDD Sequence:**
  1. Generate tests from requirements.

  2. Run tests to confirm failure.

  3. Implement code only after failure is verified.

- **Role Verbalization:** Explicit definitions of Product, Dev, and QA roles and output recipients.  

## 4. Definition of Done (DoD) Template

### AI Agent Completion Checklist

- [ ] **Self-Validation:** Cross-referenced with `backend-standards.md`, `frontend-standards.md`, `testing-standards.md`.

- [ ] **Technical Debt Avoidance:** No legacy patterns or anti-patterns used.

- [ ] **Documentation Freshness:** `README.md` and API Specifications updated.

- [ ] **Testing Suite:** 100% pass rate for Unit and Integration tests.

- [ ] **Coverage Metric:** Minimum 90% test coverage achieved.

- [ ] **QA Reporting:** Summary report delivered to Product role.

- [ ] **Security Protocol:** Input validation, SQLi/XSS checks, no secrets committed.

## 5. AI Quality Gates and Validation Procedures

| Requirement              | Validation Method                         | Mandatory Output                  |
|-------------------------|--------------------------------------------|-----------------------------------|
| Testing Standards       | Full suite execution (Unit/Integration)   | Pass/Fail Report + Coverage %     |
| API Compliance          | OpenAPI / Swagger Schema Validation       | Updated `.yaml` or `.json` Spec   |
| Security Validation     | Static analysis of inputs / SQL queries   | Security Check Confirmation       |
| Environment Consistency | Config and secret handling review         | Verified `.env.example` update    |
| Documentation           | README / Specs content verification       | Updated Documentation Index       |
| Architecture            | File location and dependency check        | Updated Directory Structure Map   |

## 6. Agent Implementation Guidelines (Prompting Strategy)

To achieve senior-level output, use **Index-Based Prompting** and **Model Context Protocols (MCPs)** to enforce Golden Standards.

### Prompting Techniques

- **Few-Shot / One-Shot Indexing:** Provide exact templates or indices for formatting consistency.

- **Command-Driven Execution:** Use commands such as `/plan` and `/develop` to enforce SDLC compliance.  

### Sample “Expert Architect” Persona Prompt

> “You are a Principal AI Solutions Architect. Your task is to [Task Description].

> You are strictly forbidden from inferring standards from the existing codebase.

> You MUST refer to backend-standards.md and testing-standards.md as the source of truth.

> Follow the TDD workflow: generate tests, verify failure, then implement.

> Maintain 90% coverage. Upon completion, provide a Definition of Done checklist and a QA report for the Product role.”

## 7. Conclusion: Scaling Productivity

By standardizing context, teams achieve **Independence from Prompt** and **Independence from Seniority**.  
Code quality becomes a constant derived from organizational standards rather than user skill in prompting.

This framework empowers every team member to produce senior-level architecture by forcing AI systems to ignore legacy technical debt and adhere to **Golden Standards**.
