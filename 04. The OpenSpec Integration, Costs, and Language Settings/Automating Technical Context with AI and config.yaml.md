# Automating Technical Context with AI and config.yaml

To update your project's technical context in the `config.yaml` file, you should utilize the AI agent within your IDE to automate the process rather than filling it out manually.

Follow these steps:

- **Initialize the file:**

  First, ensure you have run the `openspec init` command in your terminal. This creates the `open_spec` folder structure and a basic, often empty, `config.yaml` file.

- **Use an AI prompt to populate context:**

  Open the `config.yaml` file and use a prompt to instruct the AI to analyze your repository and generate the configuration.

  - *Recommended prompt:*  
    `"Review all the code and create the entire configuration in the config.yaml file"`

  - *Alternative prompt:*  
    `"Fill config.yaml with the necessary information from the technical context"`

- **Point to specific directories:**

  You can further refine the context by telling the agent where specific elements are defined, such as your commands or scripts (e.g., `"pointing everything to @ixs where I already have it defined"`).

- **Align with your tech stack:**

  Updating the technical context often requires ensuring your standard specification files (found in the `specs` folder) match your project's language.

  For example, you can prompt the agent to: `"update @backstandards"` knowing that I work with Python.

  The system will then analyze your project's existing structure and code to inherit the correct patterns and standards.

By using these automated prompts, the AI ensures that the `config.yaml` file accurately reflects your repository's structure, making the subsequent `/ff` and `/apply` commands more effective.
