# Architecture and Orchestration of Specialized Subagents in SDD

## Choosing the "Best" Agents in Spec-Driven Development (SDD)

In Spec-Driven Development (SDD), the most effective agents are not generic, off-the-shelf AI tools. Instead, they are **specialized subagents** customized with precise instructions (skills) and enriched project context.

The effectiveness of an agent depends on how well it is configured within the project’s technical contract.

## 1. Specialized Subagents

Rather than relying on a single general-purpose AI, SDD defines role-specific subagents with deep stack expertise.

### Backend Developer Agent

This subagent is configured with extensive instruction sets (often 120+ lines) that:

- Define it as an expert in the project’s backend technologies

- Enforce architectural discipline

- Mandate the use of design patterns

- Require adherence to SOLID and DRY principles

- Prevent repetitive or low-quality implementations

The backend agent operates with structured, senior-level engineering standards.

### Frontend Developer Agent

This subagent focuses on the presentation layer and user interaction logic.

It may include:

- React 18 expertise

- Clear guidelines on data-fetching strategies

- Rules for selecting appropriate libraries

- UI architecture conventions

Frontend-specific skills ensure modular, scalable, and standards-compliant implementation.

### Product Strategist Agent

This agent operates at the beginning of the development cycle.

Responsibilities include:

- Defining the “why” and “what” of a feature

- Aligning technical specifications with business goals

- Ensuring clarity before implementation begins

This prevents misalignment between engineering output and product intent.

## 2. Key Tools and Assistants

SDD is tool-agnostic, but certain environments are identified as particularly effective for managing structured subagents.

### Cursor and Claude Code

- Recognized as highly compatible with SDD frameworks such as OpenSpec

- Claude Code is noted for its structured, terminal-based workflow

- Support systematic command-driven processes

### Agnostic Compatibility

The SDD methodology can also operate with:

- Windsurf

- Antigravity

- Kleine

- Codex

The methodology matters more than the assistant itself.

## 3. Enhancing Agents with MCPs (Model Context Protocols)

Subagents become significantly more powerful when connected to external systems via MCPs.

### Frontend Enhancements

- Direct connection to Figma

- Accurate UI generation based on live design files

- Reduced interpretation errors

### Backend and Operations Enhancements

- Connection to Sentry for real-time production monitoring

- Automated bug detection and fix proposals

- Jira integration for enriching user stories into technical contracts

### Documentation Enhancements

- Integration with Notion or Confluence

- Automatic documentation updates

- Synchronization between code and written specifications

## 4. What Makes an Agent “Best”?

According to the SDD philosophy, the “best” agent is defined by the quality of its configuration.

An optimal setup includes:

- Detailed technical directives (architecture, conventions, standards)

- Clear workflow enforcement (TDD, CI/CD processes)

- Exhaustive, enriched user stories

- Live contextual integration through MCPs

When provided with this complete “recipe” of context, the AI behaves as a senior team member rather than a generic coding assistant.
