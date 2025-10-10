---
description: Fetch and resolve unresolved PR comments
---

# Fix PR Comments

Fetch unresolved comments from this branch's pull request and address them systematically.

## Process

1. **Fetch PR Information**
   ```bash
   # Get PR number for current branch
   gh pr view --json number,url,title,reviews,comments
   ```

2. **List Unresolved Comments**
   - Use `gh pr view --comments` to see all comments
   - Filter for unresolved/pending comments
   - Identify line-specific code review comments

3. **Address Each Comment**
   For each unresolved comment:
   - Read the relevant file and context
   - Understand the reviewer's concern
   - Implement the requested fix
   - Add a reply comment confirming the fix

4. **Verify Changes**
   - Run formatters and linters
   - Ensure tests still pass
   - Commit changes with reference to comment

5. **Update PR**
   ```bash
   git push origin HEAD
   gh pr comment <pr-number> --body "Addressed review comments"
   ```

## Output Format

For each comment addressed:
```
✓ Comment #X (file:line): [brief description]
  - Issue: [what was requested]
  - Fix: [what was changed]
  - Files: [list of modified files]
```

## Error Handling

- If no PR exists for current branch, inform user
- If gh CLI not installed, suggest installation
- If unable to fetch comments, show error and suggest manual check
