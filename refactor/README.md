# Refactor Team

> **A specialized AI agent team for comprehensive codebase refactoring and architectural transformation**

This is a complete agent team designed to handle codebase refactoring from initial analysis through implementation and testing. The team consists of 8 specialized agents, each with specific expertise and responsibilities for transforming your existing codebase.

## 👥 Meet the Team

### 🛠️ Refactor Orchestrator
**Role**: Master Coordinator and Workflow Manager

**What it does**:
- Receives your refactoring requests
- Assesses project status
- Routes work to appropriate agents
- Manages workflow and progress
- Ensures quality delivery

**When to use**: Always start here! This is your entry point for any refactoring work.

**Expertise**:
- Understanding refactoring requirements
- Agent coordination
- Progress tracking
- Quality assurance oversight
- Team workflow management

---

### 🔍 Explorer (Exo)
**Role**: Codebase Analyst and Documentation Specialist

**What it does**:
- Performs deep analysis of your entire codebase
- Documents architecture and patterns
- Identifies technical debt
- Maps dependencies and complexity
- Creates comprehensive technical reports

**When to use**: Automatically assigned by Orchestrator as the first step in any refactoring.

**Outputs**:
- `workshop/explorer-files/01_project_overview.md` - Comprehensive project analysis
- `workshop/explorer-files/02_stack_and_dependencies.md` - Technology stack documentation
- `workshop/explorer-files/03_architecture.md` - Architectural patterns analysis
- `workshop/explorer-files/04_code_quality.md` - Code quality assessment
- `workshop/explorer-files/05_technical_debt.md` - Technical debt inventory

**Expertise**:
- Code structure analysis
- Architecture documentation
- Pattern recognition
- Dependency mapping
- Technical debt identification
- Complexity analysis

---

### ❓ Questioner (Qua)
**Role**: Requirements Clarifier and Vision Translator

**What it does**:
- Analyzes Explorer's findings
- Asks targeted questions about refactoring goals
- Clarifies ambiguous requirements
- Bridges codebase reality with your vision
- Documents user intent and constraints

**When to use**: Automatically assigned after Explorer completes analysis.

**Outputs**:
- `workshop/questioner-files/01_questions_and_answers.md` - Q&A documentation
- `workshop/questioner-files/02_refactoring_intent.md` - Refactoring vision and goals

**Expertise**:
- Requirements gathering
- Vision clarification
- Constraint identification
- Goal articulation
- Context bridging

---

### 🏗️ Architect (Arch)
**Role**: System Designer and Strategic Planner

**What it does**:
- Designs ideal architecture from first principles
- Creates transformative architectural plans
- Applies industry best practices
- Designs optimal directory structure
- Establishes standards and conventions
- Provides detailed technical rationales

**When to use**: Automatically assigned after Questioner completes.

**Outputs**:
- `workshop/architect-files/01_architecture_proposal.md` - Architectural design and rationale
- `workshop/architect-files/02_directory_structure.md` - Optimal directory hierarchy
- `workshop/architect-files/03_refactoring_roadmap.md` - Implementation sequence
- `workshop/architect-files/04_naming_conventions.md` - Code standards and conventions

**Expertise**:
- System architecture design
- Architectural patterns
- Best practices application
- Directory structure design
- Technical decision rationale
- Migration strategy planning

---

### 📈 Product Manager (Pelin)
**Role**: Strategic Planner and Epic Creator

**What it does**:
- Synthesizes insights from Questioner and Architect
- Creates implementation roadmap
- Breaks down refactoring into epics
- Defines objectives and acceptance criteria
- Identifies dependencies and risks
- Estimates effort

**When to use**: Automatically assigned after Architect completes.

**Outputs**:
- `workshop/product-manager-files/00_implementation_roadmap.md` - Overall strategy
- `workshop/product-manager-files/01_epic_*.md` - Individual epic files

**Expertise**:
- Strategic planning
- Epic creation
- Roadmap development
- Risk assessment
- Effort estimation
- Dependency management

---

### 📊 Scrum Master (Sema)
**Role**: Task Breakdown Specialist and Workflow Coordinator

**What it does**:
- Breaks epics into user stories
- Creates actionable tasks
- Defines acceptance criteria
- Sequences work properly
- Identifies task dependencies
- Structures backlog

**When to use**: Automatically assigned after Product Manager completes epics.

**Outputs**:
- `workshop/scrum-master-files/*-stories.md` - Story files with detailed tasks

**Expertise**:
- Epic to story breakdown
- Task granularity
- Dependency management
- Work sequencing
- Acceptance criteria definition
- Sprint planning

---

### 💻 Coder (Cody)
**Role**: Implementation Specialist and Code Craftsperson

**What it does**:
- Implements stories and tasks
- Refactors code systematically
- Follows architectural decisions
- Writes quality, maintainable code
- Handles errors properly
- Works in manageable cycles
- Marks tasks as coded

**When to use**: Automatically assigned when implementation is needed.

**Outputs**:
- Refactored application code
- Updated story files with coded tasks marked

**Expertise**:
- Code implementation
- Refactoring techniques
- Pattern adherence
- Quality standards
- Error handling
- Performance optimization

---

### ✅ Tester (Tank)
**Role**: Quality Assurance Specialist and Verification Expert

**What it does**:
- Verifies implementations meet requirements
- Creates comprehensive test suites
- Executes tests and validates results
- Checks edge cases
- Validates security
- Tests error handling
- Documents test results
- Marks tasks as tested

**When to use**: Automatically assigned after Coder completes tasks.

**Outputs**:
- Test files (unit and feature tests)
- Updated story files with tested tasks marked
- Test execution reports

**Expertise**:
- Unit testing
- Feature testing
- Test execution
- Edge case testing
- Security validation
- Quality verification
- Test automation

## 🔄 Workflow

### Complete Refactoring Process

```
┌─────────────────┐
│   User Request  │
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│  Orchestrator   │ ─── Initiates refactoring workflow
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│    Explorer     │ ─── Analyzes codebase deeply
└────────┬────────┘      Creates 5 analysis documents
         │
         ▼
┌─────────────────┐
│   Questioner    │ ─── Asks clarifying questions
└────────┬────────┘      Documents refactoring intent
         │
         ▼
┌─────────────────┐
│   Architect     │ ─── Designs ideal architecture
└────────┬────────┘      Creates transformation plan
         │
         ▼
┌─────────────────┐
│ Product Manager │ ─── Creates implementation epics
└────────┬────────┘      Defines roadmap
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
│  Orchestrator   │ ─── Delivers refactored codebase
└─────────────────┘
```

### Key Workflow Characteristics

**1. Sequential Agent Activation**
Each agent completes their work before the next agent starts, ensuring solid foundations at each step.

**2. Comprehensive Documentation**
Every agent produces detailed documentation that serves as input for subsequent agents.

**3. Progressive Refinement**
From broad analysis to specific tasks, the workflow progressively refines the refactoring plan.

**4. Quality Gates**
Testing validates each implementation cycle before moving forward.

## 📁 Directory Structure

### Initial Structure
```
refactor/
├── README.md                    # This file
├── .kilocodemodes              # Agent configurations for Kilo Code (MUST BE IN PROJECT ROOT)
│
├── agents/                     # Agent role definitions
│   ├── refactor-orchestrator.md # Orchestrator instructions
│   ├── explorer.md             # Explorer instructions
│   ├── questioner.md           # Questioner instructions
│   ├── architect.md            # Architect instructions
│   ├── product-manager.md      # Product Manager instructions
│   ├── scrum-master.md         # Scrum Master instructions
│   ├── coder.md                # Coder instructions
│   └── tester.md               # Tester instructions
│
├── rules/                      # Rules and configuration
│   ├── entrypoint.md           # Universal operational rules
│   └── memory.md               # User preferences and context
│
└── workshop/                   # Active work directory
    ├── .gitkeep
    └── progress.md             # Progress tracking
```

### After Explorer Analysis
```
refactor/
└── workshop/
    └── explorer-files/
        ├── 01_project_overview.md
        ├── 02_stack_and_dependencies.md
        ├── 03_architecture.md
        ├── 04_code_quality.md
        └── 05_technical_debt.md
```

### After Questioner Phase
```
refactor/
└── workshop/
    └── questioner-files/
        ├── 01_questions_and_answers.md
        └── 02_refactoring_intent.md
```

### After Architect Phase
```
refactor/
└── workshop/
    └── architect-files/
        ├── 01_architecture_proposal.md
        ├── 02_directory_structure.md
        ├── 03_refactoring_roadmap.md
        └── 04_naming_conventions.md
```

### During Implementation
```
refactor/
└── workshop/
    ├── product-manager-files/
    │   ├── 00_implementation_roadmap.md
    │   ├── 01_epic_restructure_core.md
    │   ├── 02_epic_modernize_auth.md
    │   └── 03_epic_optimize_data.md
    │
    └── scrum-master-files/
        ├── 01_epic_restructure_core-stories.md
        ├── 02_epic_modernize_auth-stories.md
        └── 03_epic_optimize_data-stories.md
```

## 🚀 Getting Started

### 1. Setup

#### Extract `.kilocodemodes` to Your Project Root
**This is the most important step!**

```bash
# From your project root, copy the .kilocodemodes file
cp /path/to/specialized-agent-teams/refactor/.kilocodemodes ./.kilocodemodes
```

This file contains all the agent configurations that Kilo Code needs to recognize and use the specialized agents.

#### Copy Refactor Team Structure (Optional but Recommended)
```bash
# From your project root
cp -r /path/to/specialized-agent-teams/refactor ./
```

#### Configure Memory
Edit `refactor/rules/memory.md`:

```markdown
## User Preferences
- **Communication Language**: turkish  # Your preferred language
- **Technical Output**: english        # Keep technical docs in English

## Project Context
- **Name**: My Awesome App
- **Stack**: [Your technology stack]
- **Priority**: [Your refactoring priority]

## Important Decisions
- [Record key decisions as they are made]

## Constraints & Notes
- [Any special requirements or limitations]
```

### 2. Start Refactor Orchestrator

**In Kilo Code**:
1. Open Kilo Code in your project
2. Open the custom modes selector
3. Choose "🛠️ Refactor Orchestrator"
4. Make your request

> **💡 Recommended**: Use **Grok Code Fast** model for best performance with the agent team.

### 3. Make Your First Request

```
I want to refactor this codebase to improve maintainability and performance
```

The Orchestrator will:
1. ✅ Understand your refactoring goals
2. ✅ Initiate comprehensive analysis
3. ✅ Create workshop structure
4. ✅ Assign appropriate agents in sequence
5. ✅ Track progress throughout

### 4. Monitor Progress

Check `refactor/workshop/progress.md`:

```markdown
## Current Phase
Architecture Design (Architect working on structure proposal)

## Agent Status
| Agent | Status | Progress |
|-------|--------|----------|
| Explorer (Exo) | ✅ Complete | Created 5 comprehensive analysis documents |
| Questioner (Qua) | ✅ Complete | Documented refactoring intent with 2 files |
| Architect (Arch) | 🔄 In Progress | Designing optimal architecture |
| Product Manager (Pelin) | ⏳ Pending | Waiting for Arch |
| Scrum Master (Sema) | ⏳ Pending | Not started |
| Coder (Cody) | ⏳ Pending | Not started |
| Tester (Tank) | ⏳ Pending | Not started |
```

**Status Icons**:
- ⏳ Pending
- 🔄 In Progress
- ✅ Complete
- ⚠️ Blocked

## 📖 How Each Agent Works

### Refactor Orchestrator Usage

**Starting the Orchestrator**:
```
@refactor-orchestrator I want to [your refactoring request]
```

**What happens**:
1. Reads your request
2. Checks progress status
3. Initiates analysis phase
4. Assigns agents in sequence
5. Monitors progress
6. Coordinates handoffs
7. Delivers refactored codebase

**Example Interaction**:
```
User: I want to refactor this Laravel app to improve structure and performance

Orchestrator: I'll help you refactor your Laravel application for better structure and performance.

Initiating comprehensive analysis...

Creating workspace at: refactor/workshop/

Phase 1: Assigning Explorer (Exo) to analyze your codebase.

[Explorer will analyze the codebase and create 5 analysis documents]

[Progress updates follow as each agent completes their work...]
```

### Explorer Usage

**Note**: Automatically assigned by Orchestrator as the first step.

**What happens**:
1. Analyzes entire codebase structure
2. Identifies technology stack and dependencies
3. Maps architecture and patterns
4. Assesses code quality
5. Identifies technical debt
6. Creates 5 comprehensive documents
7. Reports completion to Orchestrator

**Example Outputs**:

`01_project_overview.md`:
```markdown
# Project Overview

## Purpose & Domain
E-commerce platform for selling handmade crafts, connecting artisans
with customers globally.

## Entry Points
1. **Web Application**: `public/index.php` (Laravel entry point)
2. **API**: `routes/api.php` (RESTful API for mobile apps)
3. **Console Commands**: `app/Console/Kernel.php` (scheduled tasks)
4. **Queue Workers**: Background job processing

## Key Features
- User authentication and authorization
- Product catalog with categories
- Shopping cart and checkout
- Order management
- Payment processing (Stripe integration)
- Admin dashboard
- Email notifications

...
```

### Questioner Usage

**Note**: Automatically assigned after Explorer completes.

**What happens**:
1. Reads Explorer's analysis
2. Asks 2-3 open-ended questions about refactoring goals
3. Gathers clarifications
4. Documents refactoring intent
5. Creates 2 key documents
6. Reports to Orchestrator

**Example Questions**:
```
Based on Explorer's analysis, I'd like to understand your refactoring vision:

1. What prompted you to consider refactoring this codebase? What specific 
   problems are you trying to solve?

2. What is your ideal end state for this codebase? How would you like it 
   to work differently?

3. Are there specific pain points in the current codebase that you want 
   addressed (e.g., performance, maintainability, testing, structure)?
```

**Example Output**:

`02_refactoring_intent.md`:
```markdown
# Refactoring Intent

## User Vision
Transform the Laravel e-commerce platform from a monolithic structure to a 
more maintainable, testable, and performant application using modern 
architectural patterns.

## Primary Goals
1. Improve code organization and maintainability
2. Enhance performance (page load times, database queries)
3. Increase test coverage
4. Modernize authentication system
5. Optimize database structure

## Specific Outcomes Desired
- Repository pattern for data access
- Service layer for business logic
- Improved separation of concerns
- Better error handling
- Comprehensive test suite

...
```

### Architect Usage

**Note**: Automatically assigned after Questioner completes.

**What happens**:
1. Reads Explorer's analysis and Questioner's findings
2. Designs ideal architecture from first principles
3. Creates optimal directory structure
4. Plans migration strategy
5. Establishes coding standards
6. Creates 4 comprehensive documents
7. Reports to Orchestrator

**Example Output**:

`02_directory_structure.md`:
```markdown
# Optimal Directory Structure

## Proposed Architecture-Based Structure

```
app/
├── Domain/                      # Domain layer (business logic)
│   ├── User/
│   │   ├── Models/
│   │   ├── Repositories/
│   │   ├── Services/
│   │   └── Events/
│   ├── Product/
│   ├── Order/
│   └── Payment/
│
├── Application/                 # Application layer (use cases)
│   ├── Commands/
│   ├── Queries/
│   └── DTOs/
│
├── Infrastructure/              # Infrastructure layer
│   ├── Persistence/
│   ├── Cache/
│   └── External/
│
└── Presentation/                # Presentation layer
    ├── Http/
    │   ├── Controllers/
    │   ├── Requests/
    │   └── Resources/
    └── Console/
```

## Rationale

**Why this structure?**
1. **Domain-Driven Design**: Organizes code around business domains
2. **Clear Boundaries**: Each layer has specific responsibilities
3. **Testability**: Easy to test each layer independently
4. **Scalability**: Can grow without becoming unwieldy
5. **Maintainability**: Developers can find code intuitively

...
```

### Product Manager Usage

**Note**: Automatically assigned after Architect completes.

**What happens**:
1. Reads Questioner's and Architect's outputs
2. Synthesizes insights
3. Creates implementation roadmap
4. Breaks refactoring into epics
5. Defines objectives and acceptance criteria
6. Reports to Orchestrator

**Example Output**:

`01_epic_restructure_domain_layer.md`:
```markdown
# Epic: Restructure Domain Layer

## Objective
Reorganize the current Laravel app structure into a domain-driven design 
pattern with clear separation of concerns.

## Scope
- Create domain directories for each business entity
- Move models to appropriate domain folders
- Extract business logic into service classes
- Implement repository pattern for data access

## Acceptance Criteria
- [ ] All models organized by domain
- [ ] Business logic extracted from controllers
- [ ] Repository interfaces defined
- [ ] Service classes implement business rules
- [ ] Tests updated and passing

## Dependencies
- None (foundational epic)

## Estimated Effort
Large (2-3 weeks)

## Risks
- Breaking existing functionality during move
- Updating all references to moved classes
- Maintaining backward compatibility

...
```

### Scrum Master Usage

**Note**: Automatically assigned after Product Manager completes.

**What happens**:
1. Reads all epics from Product Manager
2. Breaks epics into user stories
3. Creates detailed tasks for each story
4. Defines acceptance criteria
5. Identifies dependencies
6. Creates story documentation files
7. Reports to Orchestrator

**Example Output**:

`01_epic_restructure_domain_layer-stories.md`:
```markdown
# Stories for Epic: Restructure Domain Layer

## Story 1: Create Domain Directory Structure

**Description**: Set up the new domain-based directory structure under app/Domain/

**Acceptance Criteria**:
- [ ] Domain directories created for all business entities
- [ ] Proper namespace structure established
- [ ] Composer autoload updated
- [ ] No breaking changes to existing code

**Tasks**:
- [ ] Create app/Domain/ directory - [ ] coded, [ ] tested
- [ ] Create User domain structure - [ ] coded, [ ] tested
- [ ] Create Product domain structure - [ ] coded, [ ] tested
- [ ] Create Order domain structure - [ ] coded, [ ] tested
- [ ] Update composer.json autoload - [ ] coded, [ ] tested

**Dependencies**: None

---

## Story 2: Extract User Repository

**Description**: Create UserRepository interface and implementation to abstract 
database operations

**Acceptance Criteria**:
- [ ] UserRepositoryInterface defined
- [ ] EloquentUserRepository implements interface
- [ ] All user data operations abstracted
- [ ] Tests cover repository methods

**Tasks**:
- [ ] Create UserRepositoryInterface - [ ] coded, [ ] tested
- [ ] Create EloquentUserRepository - [ ] coded, [ ] tested
- [ ] Implement findById method - [ ] coded, [ ] tested
- [ ] Implement findByEmail method - [ ] coded, [ ] tested
- [ ] Implement create method - [ ] coded, [ ] tested
- [ ] Implement update method - [ ] coded, [ ] tested
- [ ] Bind interface in service provider - [ ] coded, [ ] tested

**Dependencies**: Story 1 (Domain structure must exist)

...
```

### Coder Usage

**Note**: Automatically assigned when implementation begins.

**What happens**:
1. Reads assigned stories from Scrum Master
2. Selects one story to implement
3. Implements tasks within that story
4. Marks tasks as coded
5. Updates progress
6. Reports completion

**Working in Cycles**:
Coder works on one story at a time, then reports back to Orchestrator.

**Example Progress Update**:
```
✅ Completed Story 1: Create Domain Directory Structure

All tasks coded:
- [x] Create app/Domain/ directory - [x] coded, [ ] tested
- [x] Create User domain structure - [x] coded, [ ] tested
- [x] Create Product domain structure - [x] coded, [ ] tested
- [x] Create Order domain structure - [x] coded, [ ] tested
- [x] Update composer.json autoload - [x] coded, [ ] tested

Directory structure follows DDD principles.
Ready for Tester to verify.

Moving to Story 2: Extract User Repository
```

### Tester Usage

**Note**: Automatically assigned after Coder completes a story.

**What happens**:
1. Reads story documentation
2. Identifies next coded story to test
3. Creates comprehensive tests
4. **EXECUTES tests using run_in_terminal**
5. Verifies all tests pass
6. Marks tasks as tested
7. Reports results

**Example Test Report**:
```
✅ Story 1 Testing Complete: Create Domain Directory Structure

Tests Created:
- Unit tests for directory structure validation
- Integration tests for autoloading
- Feature tests for namespace resolution

Test Execution:
$ composer test
PHPUnit 10.5.0 by Sebastian Bergmann and contributors.

Runtime:       PHP 8.2.0
Configuration: phpunit.xml

...............................................  47 / 47 (100%)

Time: 00:02.456, Memory: 24.00 MB

OK (47 tests, 142 assertions)

All tasks marked as tested:
- [x] Create app/Domain/ directory - [x] coded, [x] tested
- [x] Create User domain structure - [x] coded, [x] tested
- [x] Create Product domain structure - [x] coded, [x] tested
- [x] Create Order domain structure - [x] coded, [x] tested
- [x] Update composer.json autoload - [x] coded, [x] tested

Ready for next story.
```

## ⚙️ Configuration

### Memory Settings

Edit `refactor/rules/memory.md`:

```markdown
## User Preferences
- **Communication Language**: turkish    # Your preferred language
- **Technical Output**: english          # Technical documentation language

## Project Context
- **Name**: E-commerce Platform
- **Stack**: Laravel 10, Vue 3, PostgreSQL
- **Priority**: Maintainability and performance

## Important Decisions
- 2025-01-15: Use repository pattern for data access
- 2025-01-16: Implement domain-driven design structure
- 2025-01-17: Migrate to service-based architecture

## Constraints & Notes
- Must maintain backward compatibility
- Cannot change database schema in phase 1
- Need to support PHP 8.2+
```

## 🎯 Common Use Cases

### Use Case 1: Structural Refactoring

**Request**:
```
@refactor-orchestrator I want to refactor this monolithic Laravel app to use 
domain-driven design with proper separation of concerns
```

**Process**:
1. Explorer analyzes current structure, identifies monolithic patterns
2. Questioner clarifies DDD goals and constraints
3. Architect designs domain-based architecture with layers
4. Product Manager creates epics for each major restructuring phase
5. Scrum Master breaks down into stories (directory structure, repositories, services, etc.)
6. Coder implements story by story
7. Tester validates each implementation
8. Orchestrator tracks and delivers

**Timeline**: Large structural change, multiple cycles, 2-4 weeks

---

### Use Case 2: Performance Optimization

**Request**:
```
@refactor-orchestrator Optimize this application's performance, especially 
database queries and page load times
```

**Process**:
1. Explorer identifies performance bottlenecks, N+1 queries, slow endpoints
2. Questioner clarifies performance goals and acceptable trade-offs
3. Architect designs caching strategy, query optimization approach
4. Product Manager creates epics: database optimization, caching layer, frontend optimization
5. Scrum Master creates stories for each optimization area
6. Coder implements optimizations
7. Tester validates performance improvements and functionality
8. Orchestrator tracks and delivers

**Timeline**: Medium-large effort, performance testing included

---

### Use Case 3: Technology Stack Upgrade

**Request**:
```
@refactor-orchestrator Upgrade this project from Laravel 8 to Laravel 11 
and modernize dependencies
```

**Process**:
1. Explorer documents current dependencies and Laravel 8 usage patterns
2. Questioner clarifies breaking change tolerance and testing requirements
3. Architect plans migration strategy with compatibility layers
4. Product Manager creates epics: core upgrade, dependency updates, deprecated code replacement
5. Scrum Master breaks into incremental stories
6. Coder implements upgrades methodically
7. Tester validates all functionality after each change
8. Orchestrator coordinates careful progression

**Timeline**: Large effort with careful testing, 2-3 weeks

---

### Use Case 4: Code Quality Improvement

**Request**:
```
@refactor-orchestrator Improve code quality: add tests, improve naming, 
extract complex methods, reduce duplication
```

**Process**:
1. Explorer identifies code smells, duplication, complex methods, missing tests
2. Questioner clarifies quality priorities and standards
3. Architect defines coding standards and patterns
4. Product Manager creates epics: test coverage, code cleanup, pattern application
5. Scrum Master creates focused stories for each quality improvement
6. Coder refactors code systematically
7. Tester ensures comprehensive test coverage
8. Orchestrator tracks quality metrics

**Timeline**: Medium effort, ongoing process

---

### Use Case 5: Modernization

**Request**:
```
@refactor-orchestrator Modernize this codebase: use modern PHP features, 
typed properties, arrow functions, match expressions
```

**Process**:
1. Explorer identifies areas using old PHP patterns
2. Questioner confirms PHP version target and feature priorities
3. Architect plans gradual modernization approach
4. Product Manager creates feature-based modernization epics
5. Scrum Master breaks into manageable stories
6. Coder updates code to use modern features
7. Tester validates behavioral equivalence
8. Orchestrator ensures systematic progress

**Timeline**: Medium effort, focused changes

## 💡 Best Practices

### 1. Always Start with Orchestrator
```
✅ @refactor-orchestrator I want to...
❌ @coder Please refactor...
```

The Orchestrator ensures proper workflow and agent coordination.

### 2. Trust the Analysis Phase
Explorer and Questioner provide critical foundation. Don't skip them!

### 3. Answer Questioner Thoroughly
When Questioner asks about your refactoring goals, provide complete answers. This shapes the entire refactoring strategy.

### 4. Review Architect's Proposals
Check the architectural designs in `workshop/architect-files/`. Provide feedback if needed before implementation begins.

### 5. Monitor Progress Regularly
Check `progress.md` frequently:
```bash
cat refactor/workshop/progress.md
```

### 6. Let the Process Flow
Each agent builds on the previous agent's work. Trust the sequential process.

### 7. Review Documentation
All analysis and planning documents are valuable references:
- Explorer's analysis shows what was changed
- Architect's proposals show why decisions were made
- Story files track implementation progress

### 8. Provide Feedback
If something isn't right, tell the agent:
```
@architect The proposed structure seems too complex for our small team. 
Can you simplify while keeping the benefits?
```

### 9. Test Thoroughly
Tester validates each change, but you should review critical changes too.

### 10. Update Memory
Keep `rules/memory.md` updated with important decisions and constraints.

## 🐛 Troubleshooting

### "Custom modes not showing in Kilo Code"
**Problem**: `.kilocodemodes` file not in the right place

**Solution**: 
```bash
# Make sure .kilocodemodes is in your project ROOT, not in refactor/ folder
cp refactor/.kilocodemodes ./.kilocodemodes
# Restart Kilo Code
```

---

### "Explorer analysis is incomplete"
**Problem**: Explorer didn't analyze all code areas

**Solution**:
```
@refactor-orchestrator Please have Explorer re-analyze with focus on [specific area]
```

---

### "Questioner keeps asking the same questions"
**Problem**: Previous answers weren't recorded properly

**Solution**: Check `workshop/questioner-files/01_questions_and_answers.md` and provide missing information directly.

---

### "Architect's design doesn't fit our needs"
**Problem**: Architectural proposal doesn't match constraints

**Solution**: 
1. Update `rules/memory.md` with specific constraints
2. Ask Orchestrator to have Architect revise with your feedback

---

### "Tests are failing"
**Problem**: Tester reports test failures

**Solution**: Coder will be automatically reassigned to fix issues. This is normal in the refactoring cycle.

---

### "Progress seems stuck"
**Problem**: An agent hasn't completed expected work

**Solution**: Check `progress.md` to see which agent is currently assigned. Ask that agent directly about status.

---

### "Changes are too aggressive"
**Problem**: Refactoring is making too many changes at once

**Solution**: Update `rules/memory.md` with:
```markdown
## Constraints & Notes
- Prefer incremental changes over large rewrites
- Maintain backward compatibility at all times
- Focus on one domain area at a time
```

## 📊 Progress Tracking

### Progress.md Structure

```markdown
# Refactor Progress Tracking

## Current Phase
Implementation (Coder working on Story 3 of Epic 2)

## Agent Status
| Agent | Status | Progress |
|-------|--------|----------|
| Explorer (Exo) | ✅ Complete | 5 analysis documents created |
| Questioner (Qua) | ✅ Complete | Documented intent and goals |
| Architect (Arch) | ✅ Complete | Created 4 architectural documents |
| Product Manager (Pelin) | ✅ Complete | Created roadmap with 4 epics |
| Scrum Master (Sema) | ✅ Complete | Created 4 story files with 28 tasks |
| Coder (Cody) | 🔄 In Progress | Completed 2 stories, working on story 3 |
| Tester (Tank) | 🔄 In Progress | Tested 2 stories, all tests passing |

## Project Overview
**Refactoring Goal**: Transform Laravel monolith to DDD structure
**Complexity**: Large structural refactoring
**Scope**: 4 epics, 12 stories, 28 tasks

## Completed Steps

### Explorer (Exo) - Completed 2025-01-15
Analyzed entire codebase, created 5 comprehensive documents covering project 
overview, stack, architecture, code quality, and technical debt.

### Questioner (Qua) - Completed 2025-01-15
Clarified refactoring goals through interactive questioning. Documented intent 
for DDD structure with emphasis on maintainability.

### Architect (Arch) - Completed 2025-01-16
Designed domain-driven architecture with clear layer separation. Proposed 
modern directory structure and migration roadmap.

### Product Manager (Pelin) - Completed 2025-01-16
Created 4 epics: Domain restructure, Service layer, Repository pattern, and 
Testing infrastructure.

### Scrum Master (Sema) - Completed 2025-01-16
Broke down 4 epics into 12 stories with 28 detailed tasks. Dependencies mapped.

### Coder (Cody) - In Progress
#### Story 1: Create Domain Directory Structure - Completed 2025-01-17
All 5 tasks implemented. New domain structure created.

#### Story 2: Extract User Repository - Completed 2025-01-17
All 7 tasks implemented. Repository pattern applied to User domain.

#### Story 3: User Service Layer - In Progress (3/6 tasks completed)

### Tester (Tank) - In Progress
#### Story 1 - Tested 2025-01-17
Created 15 unit tests, all passing. Directory structure validated.

#### Story 2 - Tested 2025-01-17
Created 24 unit tests for repository. All tests passing.
```

## 🎓 Learning Resources

### Recommended Setup
- **Editor**: Kilo Code
- **Model**: Grok Code Fast (for optimal performance)
- **Configuration**: `.kilocodemodes` in project root

### Understanding the Agents

Read agent definition files to understand capabilities:
- `agents/refactor-orchestrator.md` - Coordination and workflow
- `agents/explorer.md` - Analysis methodology
- `agents/questioner.md` - Clarification approach
- `agents/architect.md` - Design philosophy
- `agents/product-manager.md` - Planning strategy
- `agents/scrum-master.md` - Task breakdown method
- `agents/coder.md` - Implementation approach
- `agents/tester.md` - Testing strategy

### Understanding the Process

1. **Read `rules/entrypoint.md`** - Universal operational rules
2. **Read `rules/memory.md`** - Configuration and preferences
3. **Try a small refactoring first** - Start with code quality improvements
4. **Watch the workflow** - Observe how agents hand off work
5. **Try a structural refactoring** - See the full process
6. **Customize as needed** - Adapt to your workflow

## 🤝 Contributing to This Team

Want to improve the agent team? Here's how:

### Improving Agent Behavior
Edit agent definition files in `agents/` to enhance:
- Responsibilities
- Workflow steps
- Analysis depth
- Output formats
- Quality standards

### Updating Operational Rules
Modify `rules/entrypoint.md` to adjust:
- Agent coordination rules
- File structure conventions
- Progress tracking format
- Quality gates

### Sharing Improvements
If you create valuable enhancements or customizations, share them with the community!

## 📞 Support

### Questions?
- Check agent definition files in `agents/`
- Review workflow diagrams in this README
- Look at progress.md for current status
- Check entrypoint.md for operational rules

### Issues?
- Check troubleshooting section above
- Review memory.md configuration
- Ask Orchestrator for help

### Feedback?
The team is designed to be customizable. Adjust agent behaviors, add rules, and modify workflows as needed for your specific refactoring requirements!

---

**Happy refactoring with your specialized agent team! 🚀**

Each agent is an expert in their domain. Together, they transform your codebase systematically and safely. Trust the process, provide clear requirements, and enjoy a well-structured refactored codebase!

> **Built for Kilo Code** | **Optimized for Grok Code Fast** | **Powered by specialized AI agents**
