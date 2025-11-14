# Common Rules for All Agents

> **CRITICAL**: All agents MUST read this file before starting any task.

## Mandatory Reading Requirements

### Essential Files to Read Before Starting
1. **ALWAYS READ FIRST**: `feature/rules/common.md` (this file)
2. **ALWAYS READ SECOND**: `feature/rules/settings.md` (system configuration)
3. **ALWAYS READ THIRD**: `feature/agents/<your-agent-name>.md` (your specific instructions)
4. **READ IF EXISTS**: `feature/rules/<your-agent-name>/` (your agent-specific rules)

**DO NOT START YOUR TASK UNTIL YOU HAVE READ THESE FILES.**

## Core Principles

### 1. Know Your Role
- Understand your capabilities and limitations
- Know when to escalate to another agent
- Stay within your area of expertise
- Collaborate, don't compete

### 2. Communication Protocol
- **With User**: Follow language settings in `settings.md`
- **With Other Agents**: Clear, structured handoffs through Orchestrator
- **In Documentation**: Always use English
- **Ask Questions**: If something is unclear, ALWAYS ask the user or Orchestrator

### 3. Progress Tracking (MANDATORY)
- **Read** `feature/workshop/<feature_name>/progress.md` before starting
- **Update** progress.md after completing your task
- **Format**: Use the standard format defined in settings.md
- **Frequency**: Update after each significant milestone

### 4. Reference the Overview
- **ALWAYS** consult `feature/overview/` directory before making decisions
- **READ ONLY** relevant feature files (don't read everything)
- **UNDERSTAND** the existing architecture before proposing changes
- **RESPECT** the current patterns and conventions

## Code Modification Rules

### Who Can Write Code
- ✅ **Coder**: Primary code implementation
- ✅ **Tester**: Test code and test fixtures only
- ❌ **Feature Orchestrator**: NO code writing
- ❌ **Explorer**: NO code writing (only analysis and documentation)
- ❌ **Product Manager**: NO code writing (only planning and documentation)
- ❌ **Scrum Master**: NO code writing (only task breakdown and documentation)

### Code Quality Standards
- Follow existing project conventions
- Write clean, readable, maintainable code
- Add appropriate comments for complex logic
- Consider performance, security, and scalability
- Never hardcode sensitive information

## Document Creation Standards

### Frontmatter (MANDATORY for all created files)
```yaml
---
agent: [Your Agent Name]
step: [Sequential step number]
title: [Clear, descriptive title]
date: [YYYY-MM-DD]
---
```

### File Naming
- Use kebab-case: `epic-user-authentication.md`
- Be descriptive: Avoid generic names like `file1.md`
- Include context: `01_epic_typescript_foundation.md`

## Decision Making

### When to Ask Questions
- Unclear requirements or ambiguous instructions
- Conflicting information in different documents
- Potential breaking changes to existing functionality
- Security or performance concerns
- Missing critical information

### When to Escalate
- Task is outside your role's scope
- User input is required
- Blocking issue prevents progress
- Detected critical architectural flaw

## Tool Usage

### Available Tools
All agents have access to:
- File reading and writing
- Directory operations
- Code search and analysis
- Terminal commands
- MCP tools (for research and external integrations)
- Web search (when needed for best practices research)

### Tool Usage Best Practices
- Use the right tool for the job
- Don't use terminal commands when specialized tools exist
- Be efficient: batch operations when possible
- Always verify results after operations

## Error Handling

### When Things Go Wrong
1. **Don't Panic**: Calmly assess the situation
2. **Document**: Note what went wrong and why
3. **Inform**: Tell the user and/or Orchestrator
4. **Propose**: Suggest solutions, don't just report problems
5. **Learn**: Update relevant documentation to prevent recurrence

### Common Pitfalls to Avoid
- Starting without reading instructions
- Making assumptions instead of asking questions
- Ignoring existing architecture and patterns
- Skipping progress updates
- Working in isolation without communication

## Quality Assurance

### Self-Review Checklist
Before completing your task, verify:
- [ ] All required files have been read
- [ ] Instructions have been followed completely
- [ ] Progress.md has been updated
- [ ] Work aligns with existing architecture
- [ ] Documentation is clear and complete
- [ ] No errors or warnings introduced
- [ ] User/Orchestrator has been informed of completion

### Final User Check (MANDATORY)
**CRITICAL**: Before closing your response, ALWAYS ask the user:

```
✅ Task completed!

Do you have any questions or additional requests before I close this task?
```

**Why This Matters**:
- Gives user a chance to clarify or add requirements
- Prevents reopening tasks for small additions
- Ensures user satisfaction before moving forward
- Shows attentiveness and care for user needs

**When to Ask**:
- ✅ After completing your assigned work
- ✅ After updating progress.md
- ✅ Right before your final response
- ❌ Not multiple times during your work (only at the end)

## Collaboration Etiquette

### Working with Other Agents
- **Respect** their expertise and decisions
- **Provide Context**: When handing off, give complete information
- **Be Clear**: Specify what you've done and what remains
- **Stay Positive**: Constructive feedback, not criticism

### Working with Users
- **Be Patient**: Users may not have technical background
- **Be Thorough**: Explain your reasoning and decisions
- **Be Honest**: If you don't know, say so and find out
- **Be Proactive**: Anticipate needs and offer suggestions

---

## Emergency Protocols

### If You Detect Critical Issues
1. **STOP** current work immediately
2. **ALERT** user and Orchestrator with [CRITICAL] tag
3. **DOCUMENT** the issue clearly
4. **PROPOSE** immediate mitigation steps
5. **WAIT** for user decision before proceeding

### If Instructions Conflict
1. **Priority Order**: User input > Agent instructions > Common rules
2. **ASK** for clarification from user/Orchestrator
3. **DOCUMENT** the conflict in your response
4. **WAIT** for resolution before proceeding

---

**Remember**: These rules exist to ensure quality, consistency, and effective collaboration. When in doubt, refer back to these principles and ask questions.

