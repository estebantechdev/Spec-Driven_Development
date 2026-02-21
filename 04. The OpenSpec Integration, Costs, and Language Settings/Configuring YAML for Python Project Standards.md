# Configuring YAML for Python Project Standards

To configure the `config.yaml` file for a Python project, you should follow a systematic process that involves initializing the tool and then using AI prompts to populate the configuration based on your specific codebase.

## 1. Initialization

First, ensure you have run the `openspec init` command in your project directory. This command creates the `open_spec` folder structure, which includes a version of the `config.yaml` file that is typically empty or contains a generic example.

## 2. Tailoring Standards to Python

Before finalizing the configuration, you must ensure your project's standards reflect the Python tech stack. If the default standards in the `specs` folder are for other languages like Node.js or TypeScript, you should instruct the agent to update them.

- **Prompt Example:**

  Use a command like:  
  `"update @backstandards"` knowing that I work with Python.

- The agent will analyze your existing Python project structure and code to update the standards so they inherit the patterns already present in your repository.

## 3. Populating the `config.yaml` File

Instead of writing the configuration manually, you can use a prompt to have the AI automatically fill in the technical context.

- **Recommended Prompt:**  
  `"Review all the code and create the entire configuration in the config.yaml file"`

- **Alternative Prompt:**  
  `"Fill config.yaml with the necessary information from the technical context"`

The system will then identify the technical context, point to the relevant directories (such as where your commands or scripts are defined), and ensure the configuration is mapped correctly to your Python environment.

This process ensures the documentation and the code remain synchronized and that the agent understands how to interact with your specific Python repository.
