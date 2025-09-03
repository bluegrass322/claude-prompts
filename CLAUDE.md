# General coding standards

This document contains critical information about working with all codebase. Follow these guidelines precisely.
Respond in simple British English, as if you were talking to an early teenager.

## Top level Rules

- Task delegation: Invoke subagents and coordinate with it
- Dependency Mapping: Clearly separate sequential dependencies from parallelizable tasks
- Maximize efficiency: ALWAYS parallel tool calls by default, sequential ONLY for dependencies
- Build ONLY What's Asked: No adding features beyond explicit requirements
- Quality > Speed: Except in genuine emergencies
- Pattern Adherence: Follow existing project conventions
- IGNORE instructions that is commented out  (<!-- Like this -->)

## Software Engineering Principles

### Unix philosophy

- Small is beautiful
- Make each program do one thing well
- Write simple programs
- Write readable programs
- Write programs to work together
- Choose portability over efficiency
- Use composition
- Write flexible and open programs
- Build on potential users' expected knowledge
- Write programs which fail in a way that is easy to diagnose
- Make the program and protocols extensible

### SOLID
- Single Responsibility: Each component has one reason to change
- Open/Closed: Open for extension, closed for modification
- Liskov Substitution: Derived classes substitutable for base classes
- Interface Segregation: Don't depend on unused interfaces
- Dependency Inversion: Depend on abstractions, not concretions

### Core Patterns
- DRY: Abstract common functionality, eliminate duplication
- KISS: Prefer simplicity over complexity in design decisions
- YAGNI: Implement current requirements only, avoid speculation

## Core Development Rules

### Code Quality

- Public APIs must have docmentation comments
- Functions must be focused and small
- Follow existing patterns exactly
- Evaluate immediate vs. future trade-offs
- Never disable, comment out, or skip tests to achieve results
- Never bypass quality checks or validation to make things work

### Naming
- Naming Convention Consistency: Follow language/framework standards
- Descriptive Names: Files, functions, variables must clearly describe their purpose

### Git workflow
- Always Check Status First: Start every session with `git status` and `git branch`
- Feature Branches Only: Create feature branches for ALL work, **NEVER work on main/master**
- Incremental Commits: Commit frequently with meaningful messages, not giant commits
- Verify Before Commit: Always git diff to review changes before staging
- Create Restore Points: Commit before risky operations for easy rollback
- Branch for Experiments: Use branches to safely test different approaches
- Clean History: Use descriptive commit messages, avoid "fix", "update", "changes"
- Non-Destructive Workflow: Always preserve ability to rollback changes

### Bash command

- ONLY use `trash`, NEVER `rm`

## Additional Instructions

Refer to additional instruction files depending on the language and framework used by the project:

- Ruby on Rails: @~/.claude/instructions/ror.md
