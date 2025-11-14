# Agent System Settings

## Communication Settings

### Language Preferences
- **User-Agent Communication Language**: English (can be changed to Turkish, Spanish, etc.)
- **Code Comments Language**: English
- **Documentation Language**: English

### Communication Style
- **Formality Level**: Professional but friendly
- **Verbosity**: Balanced (not too terse, not too verbose)
- **Emoji Usage**: Minimal (only for status indicators)

## Agent Behavior Settings

### Confirmation Requirements
- **Before Starting Major Tasks**: Yes (Orchestrator should confirm with user)
- **Before Moving to Next Agent**: Yes (Orchestrator should provide summary and wait for approval)
- **Before Code Changes**: No (Coder can proceed once task is assigned)
- **Before Tests**: No (Tester can proceed once coding is complete)

### Progress Tracking
- **Update Frequency**: After each significant milestone
- **Progress File Location**: `feature/workshop/<feature_name>/progress.md`
- **Summary Format**: Concise with bullet points

## File Organization Settings

### Naming Conventions
- **Files**: kebab-case (e.g., `user-auth-epic.md`)
- **Directories**: kebab-case (e.g., `user-management/`)
- **Variables in Code**: Follow project's existing conventions

### Frontmatter Format
All agents must use the following frontmatter in created files:
```yaml
---
agent: [Agent Name]
step: [Step Number]
title: [Document Title]
date: [YYYY-MM-DD]
---
```

## Quality Standards

### Code Quality
- **Test Coverage Target**: Minimum 80%
- **Code Review**: All code changes should be reviewed by Tester
- **Documentation**: All public APIs must be documented

### Security Standards
- **Sensitive Data**: Never hardcode credentials
- **Authentication**: Follow project's auth patterns
- **Input Validation**: Always validate user inputs

## Agent Coordination

### Workflow Order (for structural changes)
1. Explorer (if overview/ is empty)
2. Product Manager
3. Scrum Master
4. Coder
5. Tester
6. Back to Orchestrator

### Small Tasks Workflow
1. Orchestrator → Coder → Tester → Orchestrator

---

**Note**: Users can customize these settings based on their project needs and preferences.

