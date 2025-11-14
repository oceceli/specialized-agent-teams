# Agent System Settings

## Communication Settings

### Language Preferences
**⚠️ CRITICAL: All agents MUST respect these language settings**

- **User-Agent Communication Language**: English (can be changed to Turkish, Spanish, etc.)
  - All direct communication with user MUST be in this language
  - Questions, summaries, reports, and confirmations
  - Progress updates and status messages
  
- **Code Comments Language**: English
  - Keep code comments in English for international collaboration
  - Can be changed if specified by user
  
- **Documentation Language**: English
  - Epic files, story files, and technical documentation
  - Can follow User-Agent Communication Language if specified
  - Progress.md entries should follow User-Agent Communication Language

**Important**: 
- ✅ Agents should read this file at the start of EVERY task
- ✅ Consistency is critical - don't mix languages
- ✅ When in doubt, use the User-Agent Communication Language
- ❌ Never ignore language settings

### Communication Style
- **Formality Level**: Professional but friendly
- **Verbosity**: Balanced (not too terse, not too verbose)

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

