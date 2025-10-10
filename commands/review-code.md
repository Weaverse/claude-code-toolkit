# Code Review

Review **ONLY** changed files from `git diff`. Focus: DRY, SOLID, CLAUDE.md guidelines.

**Process:**
1. Run `git diff --name-only` to identify changed files
2. Assess complexity and delegate to specialized agents if available:
   - **Many files (5+)** → Use specialized agent for overall architecture
   - **Security changes** → Deep security review (auth, validation, secrets)
   - **Performance critical** → Analyze time/space complexity, bottlenecks
   - **Database changes** → Review queries, indexes, migrations
   - **TypeScript heavy** → Deep type analysis, generics, inference
   - **Frontend changes** → UI/UX review, accessibility, responsiveness
   - **Backend changes** → API design, error handling, scalability
3. For simple changes (1-4 files), review directly:
   - **Code Quality** - DRY violations, SOLID principles, maintainability
   - **TypeScript** - No TS errors, proper typing, strict compliance  
   - **Linting** - No lint issues, consistent formatting
   - **Architecture** - File organization, separation of concerns
   - **Security** - No exposed secrets, proper validation
   - **CLAUDE.md** - Following repository guidelines and conventions

**Output:** Prioritized issues with file:line references for changed files only.

Focus exclusively on modified code - delegate complex reviews to specialized agents.