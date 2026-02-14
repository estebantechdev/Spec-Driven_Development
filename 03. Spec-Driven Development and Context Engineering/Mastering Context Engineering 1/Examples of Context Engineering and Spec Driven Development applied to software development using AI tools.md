# Examples of Context Engineering and Spec Driven Development applied to software development using AI tools

1. **Data Model Visualization with Mermaid**

    Documentation should go beyond simple installation steps. An example is the use of Mermaid diagrams within the code to represent the data model.

    • **Explanation:** By explaining each entity in plain language and providing a Mermaid script, the AI can generate a visual representation of the database. This makes the model easily understandable for both technical teams and non-technical stakeholders.

2. **Exhaustive Backend and Coding Standards**

    A detailed list of backend standards can act as a reference for the AI to ensure consistency.

    • **Explanation:** This list includes specific architectural principles like Domain Driven Design (DDD), SOLID, and DRY. It also defines naming conventions (such as camel case), error handling methods, API design patterns, and Git workflows. By having these 400–1000 line documents in the repository, the AI is forced to follow the team’s specific style rather than inventing its own patterns.

3. **Automated GitHub Workflows**

    Modern development tools integrate native features to speed up development.

    • **Explanation:** An example is the automatic launch of a Pull Request (PR) immediately after a commit is finished. This allows developers to interact with the PR directly from the GitHub interface, streamlining the transition from coding to review.

4. **Standardized Testing with Templates**

    A structured “recipe” can be used for high-quality testing with tools like Cypress or Playwright.

    • **Explanation:** Instead of letting the AI guess how to write a test, the developer provides a “few-shot prompting” template. This template specifies how to mock database calls and how to standardize demo data. This ensures that whether a junior or senior developer is working, the resulting tests are predictable and consistent.

5. **Technical Tickets and Pseudo-code (SDD)**

    A core practice of Spec Driven Development is transforming a standard user story into a highly detailed technical ticket.

    • **Explanation:** These tickets include pseudo-code, the specific steps to be taken, and the unit tests that must be passed. Because the instructions are explicit—including requirements to update documentation or format commits in a certain way—the AI can resolve in minutes tasks that would normally take a human days to complete.

6. **Full-Stack “Liquidity” and Role Expansion**

    A backend developer may need to work on a frontend task.  

    • **Explanation:** If frontend rules and standards are already documented in the repository, a backend developer can use the AI to navigate the frontend code effectively. This creates “liquid” teams where developers can support different areas of a project, enabling flexibility across roles.

7. **Security and Validation Consistency**

    Clear technical specifications help maintain API security practices.

    • **Explanation:** When requirements are explicit, the AI consistently performs validations on forms to prevent issues such as SQL injection. This demonstrates how AI-generated code can achieve strong consistency and quality because it does not rely on human memory.
