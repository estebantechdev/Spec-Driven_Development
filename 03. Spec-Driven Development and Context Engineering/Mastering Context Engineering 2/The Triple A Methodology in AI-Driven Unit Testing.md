# The Triple A Methodology in AI-Driven Unit Testing

The Triple A methodology is described as a structural technique used when generating high-quality unit tests through AI.

Here is how it fits into the Spec-Driven Development (SDD) workflow:

- **Part of a "Metaprompt" Strategy:** The methodology is highlighted as a technical specification that an AI “prompt expert” includes when refining a basic request into a complex, professional prompt.

- **Structured Testing:** It is used alongside other advanced requirements—such as mocking services or databases and validating parameters—to ensure the AI produces code that is much more specific and clear than a simple functional test.

- **Application Example:** In the example of testing a function to “get candidates for a position,” the Triple A methodology forms part of the technical framework the AI uses to define exactly how those unit tests should be written.

**Important Note:** While the Triple A methodology is identified as a standard for high-quality testing, the three “A” terms are not explicitly defined here. In general software engineering practice, Triple A (AAA) usually stands for **Arrange, Act, and Assert**. This pattern organizes a test into three steps:

1. **Arrange** – Set up the initial conditions and inputs.

2. **Act** – Execute the functionality being tested.

3. **Assert** – Verify that the results match the expected outcome.

It is advisable to independently confirm that this interpretation aligns with the specific requirements of your project.


## Where the confusion happens

People often embed **methodology** hints inside the **task** text, for example:

```md
Write unit tests using AAA.
```

When that happens, it looks like Triple-A lives in the task, but architecturally it’s still a process rule, not domain content. It’s just being repeated in the task for emphasis.
