# The OpenSpec Framework for Synchronized Documentation and Code

OpenSpec keeps documentation and code changes synchronized through an automated workflow that integrates the update of specifications directly into the code implementation phase.

The primary mechanisms for maintaining this synchronization include:

- **Integrated `apply` Command:**

  The "magic" of the framework lies in its automated flow. When you run the `apply` command, the system does not just modify the code; it simultaneously updates the task documentation to reflect which tasks have been completed and which are still pending.

- **Delta Management:**

  If you request additional changes or iterations after the initial plan, OpenSpec treats these as "deltas". Instead of creating disconnected notes, it returns to the specific open task (such as a "create interview" task) and adds precise sub-tasks (e.g., `task 1.17.1.2`) to document the new requirements alongside the code changes.

- **Folder Lifecycle Management:**

  The system maintains synchronization by moving and managing documentation within specific internal folders like `archive`, `changes`, and `specs`. This ensures that the documentation "remains alive" and evolves with the project rather than becoming a static, outdated artifact.

- **Traceability:**

  This process provides exact traceability of every change that occurs, whether the feature is completed in a single "one shot" or through multiple iterations. Over time, the `changes` folder serves as a comprehensive, synchronized summary of everything the project does.

- **Lightweight Status Checks:**

  The tool uses specific commands like `openspec status` to quickly gather information about the current state of the project documentation. This is much faster and more token-efficient than having an AI manually scan the entire repository to determine what has been implemented.

By making documentation updates a mandatory step of the implementation command, OpenSpec ensures that the technical context provided to the AI always matches the actual state of the codebase.
