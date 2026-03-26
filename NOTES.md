# Notes

Going fast is dangerous. (going slower than manual coding is discouraged)
Code requires domain knowledge.
Generated code is "cognitive debt" until it is understood by a human.
Core focus: Cognitive debt


## Buildable project scope

Add package.json to pre-define all dependencies, e.g. "state-of-the-art" frontend frameworks and tools.
Code style must be declared. Probably should include a .prettierrc out of the box.
Implement very simple outline code that sets up React with a baseline to start from.


# Process outline
1. Produce a set of tasks describing a feature or multiple features.
    - Includes interrogation session.
    - Label all tasks according to their domain, e.g. feature development, tests, bug fixes, etc.
2. Orchestrate a set of task completions using the programmer agent.
    - The programmer agent should work on only a single task at a time before the reviewer parses the change.
3. Parse all implementations with the reviewer agent to make sure quality is good and level of abstraction is acceptable.a
    - If it is not, new tasks will be produced to cover discrepancies.


## Beads tasks

Documentation is not planning and planning is not documentation.
Planning is a process in which we produce an outline of what should be written to file.
This can include implementation, documentation, data generation, etc.
Documentation is text that describes what was implemented after a planning phase.
These tasks should generally never block each other.
Documentation should not block implementation and implementation should not block documentation.

All tasks must be concrete and actionable. It is important that a task can be closed by solving the task.
Conceptual tasks containing broad outlines or general explanations should be reserved for epic scope.

You must NEVER close tasks with `--force`. If you think a task should be closed that is blocked by another task, consult the developer.

whether every bug fix must create a Beads issue first
naming conventions for issues
whether the agent may auto-close issues
whether to prefer bugs/tasks/epics in a certain way

Never carry out a plan in the same pass as creating a plan, unless specifically instructed.
- Tasks and plans should be produced in a single pass.
- They must then be verified, and ONLY then you will be explicitly instructed to implement them.
- This process can never implicitly be executed in full in a single prompt exchange.


## TODO

Include agent report outline for agents that should return work reports.
