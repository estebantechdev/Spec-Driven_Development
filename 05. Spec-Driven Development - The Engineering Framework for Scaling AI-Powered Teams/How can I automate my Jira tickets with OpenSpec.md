# How can I automate my Jira tickets with OpenSpec

To automate your Jira tickets with OpenSpec, you utilize the **"enrich user story"** command in conjunction with a Model Context Protocol (MCP). This process transforms brief, non-technical Jira issues into exhaustive technical contracts without manual documentation effort.

The automation workflow follows these steps:

1. Connecting to Jira via MCP

    The automation relies on an MCP to bridge your development environment (like Cursor or Cloud Code) with the Jira API.

    - In your AI assistant's settings, you must configure the Jira MCP and authenticate it so the agent has permission to read from and write to your project boards.

    - If the connection fails or needs a refresh, you can disconnect and reconnect the MCP to trigger the authentication window.

2. Executing the "Enrich" Command

    Once connected, you do not need to copy-paste information. You simply provide the Jira ticket ID (e.g., "SCRUM-24") to the enrich command.

    - The agent uses the MCP to pull the original description from Jira, which is often just a few sentences.

    - It then applies prompt engineering and project context to generate a hyper-detailed version of the task.

3. Automated Ticket Enhancement

   The agent automatically updates the Jira ticket with a comprehensive technical specification that includes:

    - API Contracts: URI structures, request/response JSON schemas, and error codes.

    - Implementation Details: A list of specific files to be modified and the business logic to follow.

    - Security & Performance: Non-functional requirements like sanitizing fields to prevent SQL injection and XSS.

    - Definition of Done: Mandatory standards, such as achieving at least 90% test coverage.

4. Board State Automation

    Beyond just updating text, the OpenSpec automation can manage the ticket's lifecycle.

   - Version History: The agent saves both the original and the "improved" version within the Jira ticket for transparency.

    - Phase Transition: The system can automatically move the ticket to the next phase in your workflow, such as moving it from "Pending" to "Pending Refinement Validation".

By using this automation, every member of the team —from juniors to architects— works from the same systematic and exhaustive technical contract, ensuring that the AI has the exact "recipe" it needs to implement the code correctly in the next phases of the Spec-Driven Development cycle.
