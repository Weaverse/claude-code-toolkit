# [Claude Code Subagents](https://docs.anthropic.com/en/docs/claude-code/sub-agents)

A collection of specialized AI agents designed to enhance Claude Code's capabilities for specific software development tasks.

## Available Agents

###
 **Code Explainer**
- **Purpose**: Breaks down complex code and architectural concepts into understandable explanations
- **Use Cases**: Code walkthroughs, onboarding, understanding algorithms, clarifying technical decisions
- **Model**: Opus
- **Key Features**:
  - Structured explanations with overview-first approach
  - Visual aids using ASCII diagrams when helpful
  - Progressive disclosure from simple to complex
  - Never modifies code, only explains

### **Solution Architect**
- **Purpose**: Provides strategic guidance for implementing features, fixing bugs, or refactoring code
- **Use Cases**: Architectural decisions, complex problem-solving, exploring implementation strategies
- **Model**: Opus
- **Key Features**:
  - Requirements gathering and clarification
  - Multiple solution proposals with trade-offs
  - Risk assessment and effort estimation
  - Phased implementation recommendations

### **Debug Specialist**
- **Purpose**: Systematically diagnoses and resolves software issues
- **Use Cases**: Runtime errors, TypeScript errors, test failures, build issues, unexpected behavior
- **Model**: Not specified
- **Key Features**:
  - Error classification and severity assessment
  - Root cause analysis with systematic investigation
  - Multiple solution approaches (quick fix vs. proper fix)
  - Prevention strategies and regression test suggestions

### **Docs Writer**
- **Purpose**: Creates and maintains high-quality technical documentation
- **Use Cases**: API documentation, README files, user guides, architectural docs
- **Model**: Available in agents directory

### **Test Engineer**
- **Purpose**: Designs and implements testing strategies for software applications
- **Use Cases**: Unit testing, integration testing, end-to-end testing, test automation
- **Model**: Available in agents directory
 **Code Review Specialist**
- **Purpose**: Performs thorough code reviews with constructive feedback
- **Use Cases**: Pull request reviews, code quality assessment, best practices enforcement
- **Model**: Available in agents directory

### **Feature Architecture Reviewer**
- **Purpose**: Reviews architectural decisions for new features
- **Use Cases**: Feature design validation, scalability assessment, integration planning
- **Model**: Available in agents directory

### **PR Review Analyst**
- **Purpose**: Specialized analysis of pull requests
- **Use Cases**: Change impact analysis, regression risk assessment, merge conflict resolution
- **Model**: Available in agents directory
