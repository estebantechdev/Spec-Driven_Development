# Automating Report Verification in Spec-Driven Development

Setting up the automated report verification process in Spec-Driven Development (SDD) is primarily handled through the OpenSpec framework (or similar tools) by following a systematic workflow that treats your documentation as a formal contract.

To set up and execute this process, follow these steps:

## 1. Initialization and Tool Configuration

First, initialize the framework within your repository:

```bash
openspec init
```

During this setup, you will select the AI assistants you use (such as Cursor, Cloud Code, or Winsurf). This process creates specific configurations so those tools can recognize and execute SDD commands properly.

## 2. Establishing the "Source of Truth"

The verification process relies on a clear benchmark. You must provide the AI with Technical Directives and Workflows stored as Markdown files directly in your repository.

This includes:

### Technical Specs

- Architecture definitions

- File structures

- Coding standards (e.g., React 18 conventions)

### Definition of Done (DoD)

- 90% test coverage threshold

- Mandatory security sanitization

- Any required performance or compliance constraints

### User Story Enrichment

Use a command like:

```bash
enrich
```

This transforms a simple ticket into an exhaustive technical contract.  

That enriched contract becomes the formal basis for the automated audit.

## 3. Running the Implementation (`apply`)

Before verification, the code must be generated.

Run:

```bash
apply
```

This command instructs the AI to implement the feature according to the previously defined design and task list.

During this phase, the AI will:

- Follow the defined specifications strictly

- Execute unit and integration tests automatically

- Log terminal results directly in real time

## 4. Executing the `verify` Command

Once implementation is complete, trigger the automated evaluation:

```bash
verify
```

This command audits the implementation based on three pillars:

### Completion

- Confirms all checklist tasks (often 100+ items) were completed

- Verifies that all requirements were implemented

### Coherence

- Detects deviations from the original design

- Validates architectural consistency

### Concreteness

- Ensures technical solidity

- Verifies adherence to defined standards

## 5. Reviewing the Automated Report

After verification, the system produces a natural language report summarizing the findings.

This replaces the need for an immediate manual, line-by-line code review.

The report includes:

### Test Results

- Summary of passed/failed unit tests

- Summary of E2E tests (including browser-based flows)

### Requirement Coverage

- Confirmation of functional requirements

- Validation of non-functional requirements (e.g., security protocols)

### Critical Warnings

- Specific feedback such as:

  - A controller failing to return a `400` error for invalid IDs

  - Missing validation layers

  - Incomplete error handling

## 6. Customization Through "Skills"

If the verification process is not strict enough or misses project-specific requirements, you can customize it by editing **skills** in Markdown.

For example, you can define a skill that mandates:

- Verification of database state consistency

- Manual-style endpoint testing via `curl`

- Additional security assertions before final approval

These custom skills extend the automated audit to match your exact project standards.

## Conclusion

By shifting effort to the "laterals"—defining the specification at the beginning and executing automated verification at the end—you ensure:

- Modular architecture

- Scalability

- Best-practice compliance

- Elimination of the traditional manual validation bottleneck

This structured approach transforms documentation into an enforceable technical contract and makes quality assurance systematic rather than reactive.
