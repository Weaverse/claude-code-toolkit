---
description: Capture current work context for handoff to another agent/developer
---

# Work Context Handoff

Generate a comprehensive handoff document capturing the current state of work for seamless continuation by another agent or developer.

## Analysis Required

1. **Current State**
   - Active todo list items and their status
   - Current git branch and uncommitted changes
   - Recent commits (last 5) to understand work trajectory
   - Files currently being modified

2. **Work Completed**
   - Analyze recent git commits
   - Review completed todos
   - Identify patterns in changes made

3. **Work Remaining**
   - List pending todo items
   - Identify blockers or issues
   - Note any dependencies or prerequisites

4. **Context & Notes**
   - Current branch strategy
   - Important decisions made
   - Known issues or gotchas
   - Relevant file paths and line numbers

## Output Format

Create a markdown file at `./handoff-context-{timestamp}.md` with:

```markdown
# Handoff Context - {Date Time}

## Project
- Repository: {repo name if available}
- Branch: {current branch}
- Last Updated: {timestamp}

## Current Status

### What's Been Done
{List completed work, recent commits, changes made}

### What's In Progress
{Current todo items, ongoing work}

### What's Next
{Pending tasks, blockers, priorities}

## Technical Context

### Modified Files
{List files changed with brief description}

### Key Decisions
{Important architectural or implementation decisions}

### Known Issues
{Bugs, blockers, or things to watch out for}

## Dependencies & Prerequisites
{External dependencies, required setup, environment notes}

## Additional Notes
{Any other relevant context for continuation}
```

## Instructions

- Use `git status`, `git log`, and `git diff` to gather repository context
- Check for active todos in the todo system
- Include specific file paths with line numbers where relevant
- Be concise but comprehensive - focus on actionable information
- Save output to `./handoff-context-{YYYY-MM-DD-HHmmss}.md`
- After saving, display the file path and a brief summary

**Output the complete handoff document to the markdown file immediately.**
