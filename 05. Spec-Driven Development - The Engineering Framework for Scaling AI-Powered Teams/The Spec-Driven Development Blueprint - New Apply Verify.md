# The Spec-Driven Development Blueprint: New Apply Verify

**The Spec-Driven Development Cycle**

This cycle shifts the developer's effort to the “laterals”—spending time at the beginning to define the spec and at the end to validate the result—while the AI handles the complex implementation in the middle.

## 1. NEW / PREPARE (The "Source of Truth")

In this phase, you establish the *technical contract* that the AI must follow.

**Commands:**

- `new` → initializes the folder structure

- `ff` (fast forward) or `continue` → generates the necessary artifacts

### The Four Artifacts

- **Proposal**

  Defines the *why* and the overall objective of the feature.

- **Specs**

  Exhaustive requirements and behavioral scenarios (using BDD *Given/When/Then* logic).

- **Design**

  Outlines the technical approach, architectural decisions, and why certain alternatives were discarded.

- **Tasks** 

  A hyper-detailed checklist (often 100+ items) covering every unit test, mock, and implementation step.

## 2. APPLY / IMPLEMENT (The "AI Execution")

This is where the actual coding happens, guided strictly by the artifacts created in the first step.

**Command:**

- `apply`

### Workflow

- The AI follows **Test-Driven Development (TDD)**.

- It creates tests first.

- Verifies they fail.

- Implements the code until the terminal logs show they pass.

### Real-Time Tracking

As the AI works, it checks off items from the **Tasks** list, making the progress visible and traceable.

## 3. VERIFY / VALIDATE (The "Automated Audit")

Before any code is merged, the system performs a rigorous check to ensure quality.

**Command:**

- `verify`

### The Three Pillars of Verification

- **Completion**

  Checks if every item in the task checklist was finished.

- **Coherence**

  Identifies any deviations from the original design or architecture.

- **Concreteness**

  Evaluates the solidity of the implementation and checks if it hits the 90% test coverage threshold.

### The Report

You receive a natural language summary detailing:

- Passed tests

- Remaining warnings

- Any critical bugs (e.g., a controller not returning the correct error code)

# Finalization

- **Archive**

  Once verified, the `archive` command moves the feature from a *"change"* status into the project's permanent, formal documentation.

- **Commit**

  A specialized `commit` command prepares the code for a Pull Request, complete with:

  - An AI-generated summary

  - An automated code review for your teammates
