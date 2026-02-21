# Lifecycle and Logic of the Archive Folder

In the Open Spec framework, finished tasks and their associated documentation are moved into internal folders like `archive` as part of an automated lifecycle that ensures project documentation stays "alive" and synchronized with the code.

The specific role of the `archive` folder includes:

- **Automated Movement:** The "magic" of the framework is that it automatically handles moving documentation through folders like `archive`, `changes`, and `specs` as the state of the code evolves.

- **Traceability:** Moving completed tasks to the `archive` provides exact traceability of everything that occurred during the development process. This record reflects whether a task was completed in a single step or required multiple iterations.

- **Historical Record:** By archiving finished work, the system maintains a comprehensive history of the project's evolution. Over time, these records help the `changes` folder serve as a complete summary of every action taken throughout the project's lifecycle.

This systematic management of finished tasks prevents documentation from becoming static or outdated, as the system constantly updates the status of tasks during the `apply` phase.
