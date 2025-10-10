---
description: Create PR from current or specified branch
---

# Create Pull Request Command

Create a pull request from one branch to another.

## Usage
- `create-pr` - Create PR from current branch changes (creates new feature branch)
- `create-pr dev main` - Create PR from dev branch to main branch
- `create-pr feature/xyz dev` - Create PR from feature/xyz branch to dev branch

## Behavior
### Default (Feature Branch Mode)
- Creates a new branch based on current uncommitted changes
- Formats modified files using Biome
- Analyzes changes and automatically splits into logical commits when appropriate
- Each commit focuses on a single logical change or feature
- Creates descriptive commit messages for each logical unit
- Pushes branch to remote
- Creates pull request with proper summary and test plan

### Branch-to-Branch Mode
When specifying source and target branches (e.g., `create-pr dev main`):
- Uses existing source branch instead of creating new one
- Ensures source branch is up to date: `git pull origin <source-branch>`
- Reviews all changes: `git diff <target-branch>...<source-branch>`
- Creates PR with comprehensive summary of all changes
- For dev→main PRs specifically:
  - Include release notes section in PR description
  - List all breaking changes if any
  - Ensure all tests pass before creating PR

## Guidelines for Automatic Commit Splitting
- Split commits by feature, component, or concern
- Keep related file changes together in the same commit
- Separate refactoring from feature additions
- Ensure each commit can be understood independently
- Multiple unrelated changes should be split into separate commits