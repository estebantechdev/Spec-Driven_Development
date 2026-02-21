# Summary of The OpenSpec Integration

Integrating Open Spec into an existing project is a straightforward process, regardless of how much work has already been completed on the project. To begin, you must run the spec init command within your project directory. During this initialization process, you will be asked to select the development tools or IDEs you are using, such as Cursor or Cloud Code, and confirm your selection.

Once the initialization is finished, you need to restart your IDE so that the new commands and configurations can take effect. After restarting, you will see a new open spec folder in your project containing subdirectories for changes and specs, and the tool will have automatically integrated the necessary commands into your IDE.

The next phase of integration involves configuring the config.yaml file. You can do this by using a prompt to instruct the system to fill the configuration file with the technical context of your project. Finally, you should update the standard specification files (such as backend standards) to reflect your project's specific technology stack, such as Python or Node.js. You can simply prompt the agent to update these standards based on the existing project structure and code, allowing the tool to inherit the patterns already present in your repository.
