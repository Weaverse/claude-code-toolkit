---
description: Quick commit with auto-generated conventional commit message
---

# Fast Git Commit

I'll quickly analyze your changes and create a concise commit message, then commit immediately.

**Important**: This will commit changes when you ask me to commit - no confirmation needed.

## Quick Process:
1. Check git repository status
2. Stage modified files if nothing staged
3. Analyze changes (type, scope, files)
4. Generate one concise commit message
5. Commit immediately

```bash
# Quick git checks and staging
git status --short
if git diff --cached --quiet; then git add -u; fi
git diff --cached --name-status
```

## Commit Message Format:
- **Type**: feat|fix|docs|style|refactor|test|chore
- **Scope**: component (optional)
- **Subject**: concise description (max 50 chars)

**Conciseness Rules:**
- Under 50 characters for subject
- Imperative mood ("add" not "added")
- No unnecessary words ("this", "that", "the")
- Focus on essential change

**Example**: `fix(auth): resolve login timeout`

**Never Include:**
- AI/Claude attribution
- Co-authored-by signatures
- Tool references

The commit uses your git config and maintains full code ownership.