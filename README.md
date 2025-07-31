# Claude Code Subagents

A curated collection of specialized [Claude Code Subagents](https://docs.anthropic.com/en/docs/claude-code/sub-agents) actively used by the Weaverse development team to enhance Claude Code's capabilities for every day software development tasks to improve productivity, code quality, and team collaboration.

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
Agent specialized in answering questions and explaining code or features without making any modifications. Provides clear, thorough explanations to help you understand code structure, logic, and behavior. Use this agent when you need insights or clarifications about code, but not code changes.
```

### [Solution Architect](./agents/solution-architect.md)
- **Purpose**: Provides strategic guidance for implementing features, fixing bugs, or refactoring code
- **Use Cases**: Architectural decisions, complex problem-solving, exploring implementation strategies

```text
Agent specialized in providing solutions for new features, bug fixes, or code refactoring and optimization. This agent gathers information and requirements by asking questions when needed, then suggests possible solutions with pros and cons, along with a recommended approach. The agent does not modify any code, but helps you evaluate options and decide if you want to proceed or provide more information for alternative suggestions. Use this agent when you need advice and guidance for code improvements without direct code changes.
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
Agent specialized in debugging code errors. Identifies and analyzes the root cause of errors, explains why they occur, and then collaborates with the solution agent to suggest practical solutions. The agent does not modify any code but streamlines debugging by diagnosing issues and providing clear, actionable advice for resolution. Use this agent when you need efficient error detection and guided troubleshooting, with recommendations on how to fix bugs or improve stability.
```

### [Code Review Specialist](./agents/code-review-specialist.md)
- **Purpose**: Performs thorough code reviews with constructive feedback
- **Use Cases**: Pull request reviews, code quality assessment, best practices enforcement

```text
Expert software engineer agent for code review and feature analysis. Examines how features are rendered, manage state, integrate with backend and APIs, and which server or database components are involved. Use this agent for clear, actionable feedback and documentation on feature implementation and architecture.
```

### [Feature Architecture Reviewer](./agents/feature-architecture-reviewer.md)
- **Purpose**: Reviews architectural decisions for new features
- **Use Cases**: Feature design validation, scalability assessment, integration planning

```text
Agent specialized in reviewing already implemented features. Analyzes the feature’s structure, including its components, logic, and integration with other parts of the system. Provides clear feedback on architecture, design decisions, and potential improvements. This agent does not modify any code—use it to evaluate feature quality, maintainability, and overall implementation clarity.
```

### [PR Review Analyst](./agents/pr-review-analyst.md)
- **Purpose**: Specialized analysis of pull requests
- **Use Cases**: Change impact analysis, regression risk assessment, merge conflict resolution

```text
Agent dedicated to Pull Request (PR) review. Analyzes your latest PR or a specified PR (by ID), assessing code quality, improvements, potential code duplication across the app, and possible bugs. Clearly explains what the PR does, why the changes were made, and lists any suggested updates or fixes (ordered with indexes for easy selection). The agent does not modify code, but provides actionable suggestions to help you choose which updates to implement. Use this agent to ensure your PRs meet high standards before merging.
```
---
*The Weaverse Team 🤝*