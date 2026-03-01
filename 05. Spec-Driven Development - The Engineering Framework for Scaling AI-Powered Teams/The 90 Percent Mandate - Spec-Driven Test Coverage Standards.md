# The 90 Percent Mandate: Spec-Driven Test Coverage Standards

The 90% test coverage requirement in Spec-Driven Development (SDD) is a mandatory standard defined within the project's technical context configuration. It functions as a core element of the **Definition of Done (DoD)** for any task or feature.

## 1. Integration into the Technical Contract

When a user story is *enriched* into a fully detailed technical ticket, the 90% test coverage threshold is explicitly defined as a **non-functional requirement**.

This means:

- It is not optional.

- The AI agent must satisfy it.

- It becomes part of the formal technical contract governing implementation.

## 2. Verification Process

Before a feature can be archived or merged, the developer executes:

```bash
verify
```

This command generates a comprehensive automated report that:

- Evaluates implementation completeness

- Reviews architectural alignment

- Specifically confirms whether the 90% coverage threshold has been achieved

If the threshold is not met, the feature does not satisfy the Definition of Done.

## 3. Test-Driven Foundation

To reach such a high coverage requirement, SDD typically relies on **Test-Driven Development (TDD)** practices.

This includes:

- Unit tests

- Integration tests

- End-to-End (E2E) tests

Tests are created alongside—or before—the implementation, ensuring that coverage is intentional rather than retrofitted.

## 4. Ensuring Quality and Scalability

The 90% threshold is designed to guarantee that AI-generated code is:

- Modular

- Scalable

- Maintainable

By enforcing rigorous test coverage, SDD reduces the risk of:

- Hidden regressions

- Architectural drift

- Accumulated technical debt

This is particularly important when leveraging AI systems for rapid code generation.

## 5. Automated Reporting

The system produces a structured summary that clearly states:

- Whether the coverage goal was achieved

- Which tests passed or failed

- Any gaps preventing compliance

This shifts the developer’s role from pure implementer to validator and systems architect.

## 6. Source of Truth in Markdown

All these standards are defined in Markdown files within the repository.

This ensures:

- A transparent and version-controlled Definition of Done

- A clear benchmark for AI agents

- Prevention of low-quality or insufficiently tested code

## 7. Conclusion

By formalizing the 90% test coverage rule in the repository itself, the team creates a consistent, enforceable quality baseline for every feature.
