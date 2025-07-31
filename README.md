# [Claude Code Subagents](https://docs.anthropic.com/en/docs/claude-code/sub-agents)

A curated collection of specialized AI agents actively used by the Weaverse development team to enhance Claude Code's capabilities for every day software development tasks to improve productivity, code quality, and team collaboration.

## How to Use

There are two ways to add agents to your project:

### Method 1: Copy and Paste
1. Copy the agent file you want to use from this repository
2. Paste it into your project's `.claude/agents` folder
3. The agent will be immediately available for use in Claude Code

### Method 2: Create with /agent Command
1. Use the `/agent` command in Claude Code
2. Copy the agent description from this README
3. Paste the description when prompted - Claude will generate the rest of the agent configuration based on the description


## Available Agents

The following agents are actively used by Weaverse developers in our day-to-day work:

### [Code Explainer](./agents/code-explainer.md)
- **Purpose**: Breaks down complex code and architectural concepts into understandable explanations
- **Use Cases**: Code walkthroughs, onboarding, understanding algorithms, clarifying technical decisions

```text
Use this agent when you need to understand how code works, get explanations of complex logic, learn about feature implementations, or clarify technical concepts without making any code modifications. This agent excels at breaking down code structure, explaining algorithms, clarifying architectural decisions, and providing insights into why code is written a certain way. Perfect for code walkthroughs, onboarding, debugging understanding (not fixing), and learning sessions.
```

### [Solution Architect](./agents/solution-architect.md)
- **Purpose**: Provides strategic guidance for implementing features, fixing bugs, or refactoring code
- **Use Cases**: Architectural decisions, complex problem-solving, exploring implementation strategies

```text
Use this agent when you need strategic guidance for implementing new features, fixing bugs, or refactoring code. The agent will analyze your requirements, ask clarifying questions, and provide multiple solution approaches with trade-offs. Perfect for architectural decisions, complex problem-solving, or when you want to explore different implementation strategies before writing code.
```

### [Debug Specialist](./agents/debug-specialist.md)
- **Purpose**: Systematically diagnoses and resolves software issues
- **Use Cases**: Runtime errors, TypeScript errors, test failures, build issues, unexpected behavior

```text
Use this agent when you encounter errors, test failures, unexpected behavior, or need to diagnose issues in the codebase. This includes runtime errors, TypeScript errors, failed tests, build failures, or when code behaves differently than expected. The agent should be used proactively whenever an error or issue is detected.
```

### [Docs Writer](./agents/docs-writer.md)
- **Purpose**: Creates and maintains high-quality technical documentation
- **Use Cases**: API documentation, README files, user guides, architectural docs

```text
Use this agent when you need to create or improve documentation for code, features, APIs, or any technical concepts. This includes writing README files, API documentation, feature guides, setup instructions, or any explanatory content that needs to be clear and accessible to developers of all levels. The agent excels at transforming complex technical information into simple, digestible documentation with excellent developer experience.
```

### [Code Review Specialist](./agents/code-review-specialist.md)
- **Purpose**: Performs thorough code reviews with constructive feedback
- **Use Cases**: Pull request reviews, code quality assessment, best practices enforcement

```text
Use this agent when you need expert code review for recently written or modified code. This agent should be invoked immediately after completing code changes to ensure quality, security, and maintainability. The agent will analyze code for best practices, potential bugs, security vulnerabilities, performance issues, and adherence to project standards.
```

### [Feature Architecture Reviewer](./agents/feature-architecture-reviewer.md)
- **Purpose**: Reviews architectural decisions for new features
- **Use Cases**: Feature design validation, scalability assessment, integration planning

```text
Use this agent when you need to analyze and review feature implementations, understand how components are rendered, examine state management patterns, trace API integrations, or document the full architecture of a feature from frontend to backend. This agent provides comprehensive technical analysis of feature implementations and their architectural patterns.
```

### [PR Review Analyst](./agents/pr-review-analyst.md)
- **Purpose**: Specialized analysis of pull requests
- **Use Cases**: Change impact analysis, regression risk assessment, merge conflict resolution

```text
Use this agent when you need a comprehensive review of a pull request before merging. The agent analyzes either your latest PR or a specific PR by ID, evaluating code quality, identifying potential improvements, detecting possible code duplication across the application, and spotting potential bugs. It provides clear explanations of what the PR accomplishes, the reasoning behind changes, and delivers indexed, actionable suggestions without modifying code directly.
```
---
*The Weaverse Team 🤝*