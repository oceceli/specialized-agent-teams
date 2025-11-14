# Feature Development Team

> **A specialized AI agent team for building features, fixing bugs, and enhancing existing projects**

This is a complete agent team designed to handle feature development from requirements gathering to implementation and testing. The team consists of 6 specialized agents, each with specific expertise and responsibilities.

## 👥 Meet the Team

### 🎯 Feature Orchestrator
**Role**: Master Coordinator and Task Manager

**What it does**:
- Receives your feature requests
- Assesses task complexity
- Routes work to appropriate agents
- Manages workflow and progress
- Ensures quality delivery

**When to use**: Always start here! This is your entry point for any work.

**Expertise**:
- Understanding user requirements
- Task complexity assessment
- Team coordination
- Progress tracking
- Quality assurance oversight

---

### 🔍 Explorer (Expo)
**Role**: System Analyst and Documentation Specialist

**What it does**:
- Analyzes your entire codebase
- Creates comprehensive PRD (Project Requirements Document)
- Documents features and architecture
- Identifies patterns and conventions
- Maps system dependencies

**When to use**: Automatically assigned by Orchestrator when codebase analysis is needed.

**Outputs**:
- `overview/PRD.md` - Complete project documentation
- `overview/feature_*.md` - Individual feature documentation

**Expertise**:
- Code structure analysis
- Architecture documentation
- Pattern recognition
- Dependency mapping
- Technology stack identification

---

### 📋 Product Manager (Puma)
**Role**: Strategic Planner and Requirements Analyst

**What it does**:
- Clarifies user requirements
- Validates against existing system
- Creates detailed epics
- Identifies potential conflicts
- Defines acceptance criteria
- Researches best practices

**When to use**: Automatically assigned for medium/large features.

**Outputs**:
- `workshop/[feature]/epics/` - Epic documentation files

**Expertise**:
- Requirements gathering
- System integration planning
- Risk assessment
- Technical approach definition
- API design
- Data modeling

---

### 📊 Scrum Master (Scrummy)
**Role**: Task Breakdown Specialist and Workflow Coordinator

**What it does**:
- Breaks epics into user stories
- Creates actionable tasks for Coder
- Sequences work properly
- Identifies dependencies
- Defines clear acceptance criteria
- Plans testing requirements

**When to use**: Automatically assigned after Product Manager completes epics.

**Outputs**:
- `workshop/[feature]/stories/` - Story documentation with tasks

**Expertise**:
- Epic to story breakdown
- Task granularity
- Dependency management
- Work sequencing
- Acceptance criteria definition

---

### 💻 Coder (Cody)
**Role**: Implementation Specialist and Code Craftsperson

**What it does**:
- Implements stories and tasks
- Follows existing code patterns
- Writes quality, maintainable code
- Respects architecture decisions
- Handles errors properly
- Adds appropriate comments
- Works in manageable cycles

**When to use**: Automatically assigned when implementation is needed.

**Outputs**:
- Working application code
- Updated story files with coded tasks marked

**Expertise**:
- Code implementation
- Pattern adherence
- Quality standards
- Error handling
- Testing setup
- Performance optimization

---

### ✅ Tester (Qua)
**Role**: Quality Assurance Specialist and Verification Expert

**What it does**:
- Verifies implementations meet requirements
- Tests functionality comprehensively
- Checks edge cases
- Validates security
- Tests error handling
- Verifies integration points
- Documents test results

**When to use**: Automatically assigned after Coder completes tasks.

**Outputs**:
- Updated story files with tested tasks marked
- Test result documentation in progress.md
- Bug reports if issues found

**Expertise**:
- Functional testing
- Edge case testing
- Security validation
- Performance testing
- Integration testing
- Error handling verification

## 🔄 Workflow

### Small Tasks (Quick Path)
**Use case**: Bug fixes, single endpoint additions, minor UI changes

```
┌─────────────────┐
│   User Request  │
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│  Orchestrator   │ ─── Assesses: "This is small"
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│     Coder       │ ─── Implements directly
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│     Tester      │ ─── Verifies functionality
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│  Orchestrator   │ ─── Delivers to user
└─────────────────┘
```

### Medium/Large Features (Epic Path)
**Use case**: New features, complex logic, multiple components

```
┌─────────────────┐
│   User Request  │
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│  Orchestrator   │ ─── Assesses: "This needs planning"
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│    Explorer     │ ─── Analyzes codebase (if needed)
└────────┬────────┘      Creates/updates PRD
         │
         ▼
┌─────────────────┐
│ Product Manager │ ─── Creates epics
└────────┬────────┘      Validates requirements
         │
         ▼
┌─────────────────┐
│  Scrum Master   │ ─── Breaks into stories/tasks
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│     Coder       │ ─── Implements in cycles
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│     Tester      │ ─── Tests each cycle
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│  Orchestrator   │ ─── Coordinates & delivers
└─────────────────┘
```

### Structural Changes (Full Team)
**Use case**: Architecture refactoring, tech stack changes, major optimizations

Same as medium/large but with more intensive Explorer analysis and Product Manager planning.

## 📁 Directory Structure

### Initial Structure
```
feature/
├── README.md                    # This file
├── .kilocodemodes              # Agent configurations for Kilo Code (MUST BE IN PROJECT ROOT)
│
├── agents/                     # Agent role definitions
│   ├── feature-orchestrator.md # Orchestrator instructions
│   ├── explorer.md             # Explorer instructions
│   ├── product-manager.md      # Product Manager instructions
│   ├── scrum-master.md         # Scrum Master instructions
│   ├── coder.md                # Coder instructions
│   └── tester.md               # Tester instructions
│
├── rules/                      # Rules and configuration
│   ├── common.md               # Common rules for all agents
│   ├── settings.md             # Project-specific settings
│   ├── coder/                  # Coder-specific rules
│   ├── explorer/               # Explorer-specific rules
│   ├── feature-orchestrator/   # Orchestrator-specific rules
│   ├── product-manager/        # Product Manager-specific rules
│   ├── scrum-master/           # Scrum Master-specific rules
│   └── tester/                 # Tester-specific rules
│
├── overview/                   # Created by Explorer
│   └── .gitkeep
│
└── workshop/                   # Active work directory
    └── .gitkeep
```

### After Explorer Runs
```
feature/
└── overview/
    ├── PRD.md                  # Project Requirements Document
    ├── feature_auth.md         # Authentication feature docs
    ├── feature_user.md         # User management docs
    └── feature_*.md            # Other feature docs
```

### During Feature Development
```
feature/
└── workshop/
    └── password-reset/         # Feature workspace
        ├── progress.md         # Progress tracking
        ├── epics/
        │   ├── 01_epic_email_flow.md
        │   ├── 02_epic_reset_ui.md
        │   └── 03_epic_security.md
        └── stories/
            ├── 01_epic_email_flow-stories.md
            ├── 02_epic_reset_ui-stories.md
            └── 03_epic_security-stories.md
```

## 🚀 Getting Started

### 1. Setup

#### Extract `.kilocodemodes` to Your Project Root
**This is the most important step!**

```bash
# From your project root, copy the .kilocodemodes file
cp /path/to/specialized-agent-teams/feature/.kilocodemodes ./.kilocodemodes
```

This file contains all the agent configurations that Kilo Code needs to recognize and use the specialized agents.

#### Copy Feature Team Structure (Optional but Recommended)
```bash
# From your project root
cp -r /path/to/specialized-agent-teams/feature ./
```

#### Configure Settings
Edit `feature/rules/settings.md`:

```markdown
## Project Information
project_name: "My Awesome App"
project_type: "web_application"
primary_language: "typescript"
framework: "Next.js"

## Communication Settings
user_language: "turkish"        # Your preferred language
documentation_language: "english"  # Keep docs in English

## Workflow Settings
require_tests: true
require_documentation: true
auto_update_progress: true
```

### 2. Start Feature Orchestrator

**In Kilo Code**:
1. Open Kilo Code in your project
2. Open the custom modes selector
3. Choose "🎯 Feature Orchestrator"
4. Make your request

> **💡 Recommended**: Use **Grok Code Fast** model for best performance with the agent team.

### 3. Make Your First Request

```
I want to add password reset functionality for users
```

The Orchestrator will:
1. ✅ Ask clarifying questions
2. ✅ Assess complexity
3. ✅ Create workspace structure
4. ✅ Assign appropriate agents
5. ✅ Track progress

### 4. Monitor Progress

Check `feature/workshop/[feature-name]/progress.md`:

```markdown
## Agent Status
| Agent | Status | Progress |
|-------|--------|----------|
| Explorer (Expo) | ✅ Complete | Created PRD with 5 features documented |
| Product Manager (Puma) | 🔄 In Progress | Created 2/3 epics |
| Scrum Master (Scrummy) | ⏳ Pending | Waiting for Puma |
| Coder (Cody) | ⏳ Pending | Not started |
| Tester (Qua) | ⏳ Pending | Not started |
```

**Status Icons**:
- ⏳ Pending
- 🔄 In Progress
- ✅ Complete
- ⚠️ Blocked

## 📖 How Each Agent Works

### Feature Orchestrator Usage

**Starting the Orchestrator**:
```
@feature-orchestrator I want to [your request]
```

**What happens**:
1. Reads your request
2. Asks clarifying questions
3. Checks `overview/` directory status
4. Assesses task complexity
5. Creates feature workspace
6. Initializes `progress.md`
7. Assigns first agent
8. Monitors progress
9. Coordinates handoffs
10. Delivers completed feature

**Example Interaction**:
```
User: I want to add email notifications when orders are shipped

Orchestrator: I'll help you add email notifications for shipped orders.

Let me ask a few questions:
1. Should this work for all users or only registered users?
2. What email service are you using (SendGrid, AWS SES, etc)?
3. Should users be able to opt out of these notifications?
4. Do you want to customize the email template?

[After getting answers]

Task assessed as MEDIUM complexity.

I'll assign:
1. Explorer - to analyze email infrastructure (if needed)
2. Product Manager - to create epic with email flow
3. Scrum Master - to break down into stories
4. Coder - to implement
5. Tester - to verify

Creating workspace at: feature/workshop/order-email-notifications/

[Progress updates follow...]
```

### Explorer Usage

**Note**: Usually assigned automatically by Orchestrator.

**Direct use**:
```
@explorer Please analyze the codebase and create documentation
```

**What happens**:
1. Checks `overview/` directory
2. Analyzes entire codebase structure
3. Identifies technology stack
4. Maps architecture
5. Documents patterns
6. Creates PRD.md
7. Creates feature_*.md files
8. Reports completion to Orchestrator

**Example Output**:

`overview/PRD.md`:
```markdown
# Project Requirements Document

## Project Overview
E-commerce platform built with Next.js, featuring user authentication,
product catalog, shopping cart, and order management.

## Technology Stack

### Frontend
- Framework: Next.js 14 (App Router)
- State Management: Zustand
- Styling: Tailwind CSS
- UI Components: Shadcn/ui

### Backend
- API: Next.js API Routes
- Database: PostgreSQL (Prisma ORM)
- Authentication: NextAuth.js
- Email: SendGrid

...
```

### Product Manager Usage

**Note**: Usually assigned automatically by Orchestrator.

**Direct use** (not recommended):
```
@product-manager Create epic for [feature]
```

**What happens**:
1. Reads PRD and relevant feature docs
2. Asks clarifying questions
3. Validates against existing system
4. Identifies potential conflicts
5. Creates epic documentation
6. Defines requirements
7. Plans technical approach
8. Assesses risks
9. Reports to Orchestrator

**Example Output**:

`workshop/order-email/epics/01_epic_notification_system.md`:
```markdown
---
epic: 01
title: Email Notification System
agent: Product Manager
date: 2025-11-14
status: complete
---

# Epic: Email Notification System

## User Value
Enable customers to receive automated email notifications when their
orders are shipped, improving transparency and customer satisfaction.

## Requirements

### Functional
1. Send email when order status changes to "shipped"
2. Include tracking number in email
3. Include order details (items, quantities)
4. Allow users to opt-out in preferences
5. Retry failed email sends

### Non-Functional
1. Email delivery within 5 minutes of status change
2. 99% email delivery rate
3. Mobile-responsive email template
4. GDPR compliant

...
```

### Scrum Master Usage

**Note**: Usually assigned automatically by Orchestrator.

**What happens**:
1. Reads all epics for feature
2. Breaks epics into user stories
3. Creates tasks for each story
4. Defines acceptance criteria
5. Identifies dependencies
6. Creates story documentation
7. Reports to Orchestrator

**Example Output**:

`workshop/order-email/stories/01_epic_notification_system-stories.md`:
```markdown
# Stories for Epic: Email Notification System

## Story 1: Database Setup for Email Preferences

**Description**: Add database schema to store user email preferences

**User Value**: Users can control which notifications they receive

**Acceptance Criteria**:
- [ ] Users can opt-out of order notifications
- [ ] Preference persists across sessions
- [ ] Default is opt-in for new users

**Tasks**:
- [ ] Create email_preferences table migration - [ ] coded, [ ] tested
- [ ] Add user_id foreign key - [ ] coded, [ ] tested
- [ ] Add notification_types JSON field - [ ] coded, [ ] tested
- [ ] Create indexes for performance - [ ] coded, [ ] tested

**Dependencies**: None

**Risks**: Migration on large user table may take time
```

### Coder Usage

**Note**: Usually assigned automatically by Orchestrator.

**What happens**:
1. Reads assigned stories
2. Understands acceptance criteria
3. Reviews related code
4. Implements tasks
5. Follows existing patterns
6. Writes quality code
7. Marks tasks as coded
8. Reports progress

**Working in Cycles**:
Coder works on 1-5 stories per cycle, then reports back to Orchestrator.

**Example Progress Update**:
```
✅ Completed Story 1: Database Setup for Email Preferences

All tasks coded:
- [x] Created email_preferences table migration - [x] coded, [ ] tested
- [x] Added user_id foreign key - [x] coded, [ ] tested
- [x] Added notification_types JSON field - [x] coded, [ ] tested
- [x] Created indexes for performance - [x] coded, [ ] tested

Code follows existing Prisma schema patterns.
Ready for Tester to verify.

Moving to Story 2: Email Template Creation
```

### Tester Usage

**Note**: Usually assigned automatically by Orchestrator.

**What happens**:
1. Reads story documentation
2. Reviews acceptance criteria
3. Examines coded implementation
4. Tests functionality
5. Tests edge cases
6. Tests error handling
7. Tests security
8. Marks tasks as tested
9. Reports results

**Example Test Report**:
```
✅ Story 1 Testing Complete: Database Setup for Email Preferences

Functional Tests:
✅ User can toggle notification preferences
✅ Preferences persist after logout/login
✅ New users default to opt-in
✅ Database migration runs successfully

Edge Cases:
✅ Handles invalid preference values gracefully
✅ Works with users having no preferences set
✅ Multiple rapid preference changes handled correctly

Security:
✅ Users can only modify their own preferences
✅ SQL injection attempts rejected
✅ Proper authorization checks in place

All tasks marked as tested:
- [x] Created email_preferences table migration - [x] coded, [x] tested
- [x] Added user_id foreign key - [x] coded, [x] tested
- [x] Added notification_types JSON field - [x] coded, [x] tested
- [x] Created indexes for performance - [x] coded, [x] tested

Ready for next story.
```

## ⚙️ Configuration

### Project Settings

Edit `feature/rules/settings.md`:

```markdown
## Project Information
project_name: "YourApp"
project_type: "web_application"  # or: mobile_app, api, cli_tool, library
primary_language: "typescript"    # or: javascript, python, go, etc
framework: "Next.js"             # Your main framework

## Communication Settings
user_language: "turkish"          # Language for agent<->user communication
documentation_language: "english" # Keep documentation in English

## Workflow Settings
require_tests: true               # Tester must verify everything
require_documentation: true       # Documentation is mandatory
auto_update_progress: true       # Agents update progress.md automatically

## Quality Standards
code_coverage_target: 80          # Minimum test coverage
max_cyclomatic_complexity: 10    # Code complexity limit
require_type_annotations: true   # Type safety required
```

### Agent-Specific Rules

Create custom rules for specific agents:

**Example**: `feature/rules/coder/api_standards.md`
```markdown
# API Standards for Coder

## Required Rules
1. All API routes must have rate limiting
2. All inputs must be validated with Zod
3. All errors must use standard error format
4. All endpoints must have JSDoc comments

## Error Format
```typescript
{
  success: false,
  error: {
    code: "ERROR_CODE",
    message: "User friendly message",
    details: {...}
  }
}
```
```

**Example**: `feature/rules/tester/security_checks.md`
```markdown
# Security Testing Checklist

## Always Test
- [ ] Authentication required where needed
- [ ] Authorization prevents unauthorized access
- [ ] Input validation prevents injection
- [ ] Rate limiting prevents abuse
- [ ] Sensitive data not exposed
- [ ] CORS configured properly
```

## 🎯 Common Use Cases

### Use Case 1: Adding a New Feature

**Request**:
```
@feature-orchestrator I want to add real-time chat functionality
```

**Process**:
1. Orchestrator assesses as LARGE (multiple components, real-time, database)
2. Explorer analyzes codebase for existing communication patterns
3. Product Manager creates epics:
   - Epic 1: WebSocket infrastructure
   - Epic 2: Chat UI components
   - Epic 3: Message persistence
   - Epic 4: Notifications
4. Scrum Master breaks into 15-20 stories
5. Coder implements in cycles (3-5 stories at a time)
6. Tester verifies each cycle
7. Orchestrator tracks and delivers

**Timeline**: Medium-large feature, multiple cycles

---

### Use Case 2: Fixing a Bug

**Request**:
```
@feature-orchestrator Users can't update their profile pictures
```

**Process**:
1. Orchestrator assesses as SMALL (single component issue)
2. Coder directly investigates and fixes
3. Tester verifies fix and tests edge cases
4. Orchestrator confirms completion

**Timeline**: Quick fix, single cycle

---

### Use Case 3: Refactoring

**Request**:
```
@feature-orchestrator Refactor authentication to use JWT instead of sessions
```

**Process**:
1. Orchestrator assesses as STRUCTURAL (major change)
2. Explorer analyzes all authentication touchpoints
3. Product Manager creates detailed migration epic
4. Scrum Master creates careful story sequence
5. Coder implements incrementally with feature flags
6. Tester performs comprehensive testing
7. Orchestrator coordinates rollout

**Timeline**: Large structural change, multiple cycles

---

### Use Case 4: Adding Integration

**Request**:
```
@feature-orchestrator Integrate Stripe payment processing
```

**Process**:
1. Orchestrator assesses as MEDIUM (external integration)
2. Explorer checks existing payment/API patterns
3. Product Manager researches Stripe best practices, creates epic
4. Scrum Master creates stories for: setup, checkout flow, webhooks, testing
5. Coder implements following Stripe docs
6. Tester verifies with Stripe test mode
7. Orchestrator tracks and delivers

**Timeline**: Medium feature, multiple cycles

## 💡 Best Practices

### 1. Always Start with Orchestrator
```
✅ @feature-orchestrator I want to...
❌ @coder Please add...
```

The Orchestrator ensures proper workflow and coordination.

### 2. Be Specific and Clear
```
❌ "Add login"
✅ "Add email/password authentication with password reset and email verification"
```

More detail = better planning and implementation.

### 3. Answer Questions Thoroughly
When agents ask questions, provide complete answers. They're gathering requirements to build exactly what you need.

### 4. Trust the Process
Each agent adds value:
- Explorer ensures understanding
- Product Manager prevents mistakes
- Scrum Master ensures clarity
- Coder implements quality
- Tester ensures reliability

Don't skip steps!

### 5. Review Progress Regularly
Check `progress.md` to see status:
```bash
cat feature/workshop/[feature-name]/progress.md
```

### 6. Keep Overview Updated
Run Explorer periodically (especially after major changes):
```
@feature-orchestrator Please have Explorer update the codebase documentation
```

### 7. Use Custom Rules for Team Standards
Document your team's coding standards in `rules/[agent]/` for consistency.

### 8. Provide Feedback
If something isn't right, tell the agent:
```
@tester The validation you added is too strict, users can't enter valid data
```

### 9. Let Agents Collaborate
Agents coordinate automatically. Don't micromanage the handoffs.

### 10. Archive Completed Features
Move completed feature workspaces to maintain clarity:
```bash
mkdir feature/workshop/_archive
mv feature/workshop/password-reset feature/workshop/_archive/
```

## 🐛 Troubleshooting

### "Custom modes not showing in Kilo Code"
**Problem**: `.kilocodemodes` file not in the right place

**Solution**: 
```bash
# Make sure .kilocodemodes is in your project ROOT, not in feature/ folder
cp feature/.kilocodemodes ./.kilocodemodes
# Restart Kilo Code
```

---

### "Overview directory is empty"
**Problem**: No codebase documentation exists

**Solution**: Orchestrator will automatically assign Explorer

---

### "Agent doesn't understand project structure"
**Problem**: PRD is outdated

**Solution**:
```
@feature-orchestrator Please have Explorer update the PRD
```

---

### "Code doesn't follow our patterns"
**Problem**: Coder isn't aware of your standards

**Solution**: Add custom rules in `feature/rules/coder/`

---

### "Tests aren't comprehensive enough"
**Problem**: Tester doesn't know your requirements

**Solution**: Add custom rules in `feature/rules/tester/`

---

### "Agent is confused about task"
**Problem**: Context may be missing or unclear

**Solution**: 
1. Check if agent read required files (they mention this in responses)
2. Provide additional context directly
3. Ask Orchestrator to clarify with Product Manager

---

### "Progress tracking is not updating"
**Problem**: Auto-update may be off

**Solution**: Check `feature/rules/settings.md`:
```markdown
auto_update_progress: true  # Ensure this is true
```

## 📊 Progress Tracking

### Progress.md Structure

```markdown
# [Feature Name] Progress

## Current Phase
Implementation (Coder working on Story 3 of 8)

## Agent Status
| Agent | Status | Progress |
|-------|--------|----------|
| Explorer (Expo) | ✅ Complete | Created PRD + 3 feature docs |
| Product Manager (Puma) | ✅ Complete | Created 3 epics with 8 stories total |
| Scrum Master (Scrummy) | ✅ Complete | Broke down 8 stories into 35 tasks |
| Coder (Cody) | 🔄 In Progress | Completed 2 stories, working on story 3 |
| Tester (Qua) | 🔄 In Progress | Tested 2 stories, all tasks passing |

## Feature Overview
**User Request**: Add password reset functionality with email verification
**Complexity**: Medium
**Estimated Scope**: 3 epics, 8 stories, 35 tasks

## Agent Summaries

### Feature Orchestrator
#### 2025-11-14 10:00 - Feature Initialized
Created workspace, assessed as medium complexity, assigned Explorer.

#### 2025-11-14 10:15 - Explorer Complete
PRD updated, relevant features documented. Assigned Product Manager.

### Explorer (Expo)
#### 2025-11-14 10:05 - Analysis Complete
Analyzed authentication system, documented in feature_auth.md.
Found existing email service setup (SendGrid).
Ready for Product Manager.

### Product Manager (Puma)
#### 2025-11-14 10:20 - Epics Created
Created 3 epics:
1. Email verification flow
2. Password reset UI
3. Security measures

All epics include detailed requirements and technical approach.

### Scrum Master (Scrummy)
#### 2025-11-14 10:45 - Stories Created
Broke down 3 epics into 8 stories with 35 tasks total.
Dependencies identified and sequenced.

### Coder (Cody)
#### 2025-11-14 11:00 - Story 1 Complete
Implemented database changes for token storage.
All 5 tasks coded and tested.

#### 2025-11-14 11:30 - Story 2 Complete
Implemented email sending service.
All 4 tasks coded and tested.

#### 2025-11-14 12:00 - Story 3 In Progress
Working on password reset UI components (3 of 6 tasks complete)

### Tester (Qua)
#### 2025-11-14 11:25 - Story 1 Tested
All functionality verified. Edge cases pass. Security checks pass.

#### 2025-11-14 11:55 - Story 2 Tested
Email sending verified. Error handling works. Rate limiting tested.
```

## 🎓 Learning Resources

### Recommended Setup
- **Editor**: Kilo Code
- **Model**: Grok Code Fast (for optimal performance)
- **Configuration**: `.kilocodemodes` in project root

### Understanding the Agents

Read agent definition files to understand capabilities:
- `agents/feature-orchestrator.md` - Coordination and workflow
- `agents/explorer.md` - Analysis and documentation
- `agents/product-manager.md` - Planning and requirements
- `agents/scrum-master.md` - Task breakdown and sequencing
- `agents/coder.md` - Implementation and quality
- `agents/tester.md` - Quality assurance and verification

### Understanding the Process

1. **Read `rules/common.md`** - Rules all agents follow
2. **Read `rules/settings.md`** - Configuration options
3. **Try small task first** - Start with a bug fix
4. **Watch the workflow** - Observe agent handoffs
5. **Try medium feature** - See full epic process
6. **Customize for your needs** - Add custom rules

### Example Walkthroughs

See `examples/` directory (coming soon) for complete walkthroughs:
- Adding authentication
- Building a REST API
- Creating admin dashboard
- Refactoring database layer

## 🤝 Contributing to This Team

Want to improve the agent team? Here's how:

### Improving Agent Behavior
Edit agent definition files in `agents/` to enhance:
- Responsibilities
- Workflow steps
- Quality standards
- Output formats

### Adding Custom Rules
Create project-specific rules in `rules/[agent]/` for:
- Coding standards
- Testing requirements
- Documentation format
- Quality metrics

### Sharing Improvements
If you create valuable custom rules or agent improvements, share them!

## 📞 Support

### Questions?
- Check agent definition files in `agents/`
- Review workflow diagrams in this README
- Look at progress.md for current status

### Issues?
- Check troubleshooting section above
- Review settings.md configuration
- Ask Orchestrator for help

### Feedback?
The team is designed to be customizable. Adjust as needed for your workflow!

---

**Happy coding with your specialized agent team! 🚀**

Each agent is an expert in their domain. Together, they deliver quality software efficiently. Trust the process, and enjoy the results!

> **Built for Kilo Code** | **Optimized for Grok Code Fast** | **Powered by specialized AI agents**
