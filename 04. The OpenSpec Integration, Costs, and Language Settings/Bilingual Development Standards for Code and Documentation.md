# Bilingual Development Standards for Code and Documentation

While you can use Spanish for project specifications and documentation, there are several technical recommendations to ensure the quality and scalability of your project. The expert works interchangeably in both English and Spanish, and the system currently handles both languages without major issues.

However, the following best practices are recommended to optimize your development process:

- **Input in Spanish, Output in English:**

  You can interact with the AI agent in your natural language to increase your own speed. However, it is highly recommended to configure IDE rules (such as in Cursor settings) so that even if you speak to the agent in Spanish, it always responds, writes code, comments, and documentation in English. This prevents "language pollution," such as having parameters or comments in multiple languages within the same codebase.

- **Adhering to Global Standards:**

  Keeping technical documentation and code exclusively in English ensures the project remains global and can be maintained by any team in the future. This aligns with high-level quality standards expected by a CTO, regardless of the team's current nationality.

- **Systematic Commands:**

  By following the structured OpenSpec workflow (using commands like `/ff`, `/apply`, or `/commit`), you reduce the need for long conversational interactions. This makes the process more deterministic and predictable, making the specific language used for instructions less critical to the final outcome.

- **Successful Instructions:**

  Practical tests have shown that the system correctly processes complex instructions given in Spanish, such as: `"Fill the config.yaml file with the necessary information,"` without any problems.

In summary, while the system is capable of understanding Spanish for instructions, the professional recommendation is to keep the final code and documentation in English to ensure consistency and long-term project viability.
