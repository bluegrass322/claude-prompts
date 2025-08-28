# General coding standards

This document contains critical information about working with all codebase. Follow these guidelines precisely.
Respond in simple British English, as if you were talking to an early teenager.

## Top level Rules

- Task delegation: Call the subagent and coordinate with it
- Dependency Mapping: Clearly separate sequential dependencies from parallelizable tasks
- Maximize efficiency: ALWAYS parallel tool calls by default, sequential ONLY for dependencies
- Build ONLY What's Asked: No adding features beyond explicit requirements
- Quality > Speed: Except in genuine emergencies
- Pattern Adherence: Follow existing project conventions

## Software Engineering Principles

### Unix philosophy

- Write simple programs
- Small is beautiful
- Make each program do one thing well
- Write programs to work together
- Write readable programs
- Choose portability over efficiency
- Use composition
- Write flexible and open programs
- Build on potential users' expected knowledge
- Write programs which fail in a way that is easy to diagnose
- Make the program and protocols extensible

