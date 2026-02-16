# Spec-Driven Development Tools and Techniques

| Tool or Technique Name | Category | Primary Function | Key Features | Recommended Use Case | Compatibility |
|------------------------|----------|------------------|-------------|---------------------|--------------|
| Cursor | IDE / Code Editor | AI-First Code Editor | Composer 1 model, high speed, background agents, and memory rules. | Rapid spec-driven development and complex project context management. | Fork of VS Code. |
| GitHub Copilot | IDE / Code Editor | AI Pair Programming | Code completion, agent interface, and auto-mode for model selection. | Standard AI-assisted coding and development. | Integrated with VS Code and other major IDEs. |
| Claude Code | Terminal Tool | Terminal-based AI Assistant | Command-line interface for AI interaction. | Developers preferring terminal-based workflows. | CLI / Terminal. |
| Metaprompt | Prompt Engineering Technique | Prompt Optimization | The AI acts as a prompt expert to generate a more complex, specific prompt based on a basic goal. | Generating unit tests or complex technical specifications. | Universal (LLMs). |
| Expert Inquiry (Question the Expert) | Prompt Engineering Technique | Consultative Analysis | The AI asks the user exhaustive questions to clear ambiguities before proposing a solution. | Database modeling, architecture design, or tasks outside the user's main expertise. | Universal (LLMs). |
| Jira MCP | MCP (Model Context Protocol) | Context Integration | Connects user stories and technical documentation directly to the AI. | Importing tasks and requirements for development. | Atlassian Suite. |
| Confluence / Notion MCP | MCP (Model Context Protocol) | Knowledge Base Integration | Accesses information flows, use cases, and product specs. | Providing broad project context and background documentation. | Notion, Confluence. |
| Context.dev | MCP (Model Context Protocol) | Documentation Management | Keeps documentation for specific library/framework versions up to date. | Ensuring the AI uses the correct syntax for specific versions (deprecated methods, etc.). | Web-based documentation. |
| Figma MCP | MCP (Model Context Protocol) | Design Integration | Translates layers, RGB colors, and SVG data for the LLM. | Achieving Pixel-Perfect front-end or mobile implementations. | Figma design files. |
| Playwright | MCP / Testing Tool | QA Automation | Generates automated tests and allows headless browser navigation. | Manual or automatic QA testing (login flows, endpoints) at zero cost. | Web browsers. |
| Sentry | MCP / Monitoring Tool | Error Tracking | Identifies production errors and provides context for fixes. | Guaranteeing error-free code before production. | Application monitoring. |
| Snyk | MCP / Security Tool | Security Analysis | Scans directories for vulnerabilities and dependency flaws. | Identifying and fixing cybersecurity vulnerabilities in background agents. | Development directories. |
| Auto Mode | Configuration Setting | Token and Model Management | Automatically selects the best model for the response to balance cost and quality. | Standardizing usage across different models. | Cursor, GitHub Copilot, Cloud Code. |
| Privacy Mode | Configuration Setting | Data Security | Ensures user code is not used to train the LLM or improve the product. | Handling sensitive or proprietary codebases. | Found in General Settings of AI editors. |
| WARP | Terminal Tool | AI-Enhanced Terminal | Integrated AI capabilities within the terminal emulator. | Terminal-centric development tasks. | Terminal. |
| Codexcli | Terminal Tool | Terminal AI Interface | Accessing LLM capabilities directly from the command line. | Scripting and terminal commands. | CLI / Terminal. |
| Windsurf | IDE / Code Editor | AI-Powered Editor | Contextual understanding and similar functionality to Cursor/Copilot. | General development with AI context. | Not in source. |
