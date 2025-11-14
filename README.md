# Specialized Agent Teams for Kilo Code (Suggested)

> **Transform your development workflow with specialized AI agent teams that work together seamlessly**

A sophisticated multi-agent system designed for Kilo Code, enabling coordinated software development through specialized AI agents. Each agent has a specific role, expertise, and responsibility, working together to deliver high-quality features from conception to deployment.

## 🎯 What is This?

This project provides a framework for organizing Kilo Code into specialized agent teams. Instead of using a single AI assistant for everything, you get a team of experts:

- 🎯 **Feature Orchestrator** - Manages workflow and coordinates the team
- 🔍 **Explorer (Expo)** - Analyzes codebases and creates documentation
- 📋 **Product Manager (Puma)** - Plans features and creates epics
- 📊 **Scrum Master (Scrummy)** - Breaks down work into stories and tasks
- 💻 **Coder (Cody)** - Implements features with quality code
- ✅ **Tester (Qua)** - Ensures quality through comprehensive testing

## 🚀 Why Use Agent Teams?

### Traditional Approach Problems
- Single AI tries to do everything (planning, coding, testing)
- Context gets mixed and confused
- Quality varies significantly
- Hard to track progress
- No clear workflow or process

### Agent Team Benefits
- ✅ **Specialized Expertise**: Each agent focuses on what it does best
- ✅ **Clear Workflow**: Structured process from idea to implementation
- ✅ **Better Quality**: Dedicated testing and review cycles
- ✅ **Progress Tracking**: Know exactly where you are in the process
- ✅ **Scalable**: Works for small bugs to large features
- ✅ **Documentation**: Automatic comprehensive documentation
- ✅ **Consistency**: Follows patterns and best practices

## 📦 Available Agent Teams

### Feature Development Team
**Location**: `/feature`

The complete team for building new features and fixing issues in existing projects.

**Use Cases**:
- Developing new features
- Fixing bugs
- Refactoring code
- Adding integrations
- Performance improvements

**Workflow**: Request → Analysis → Planning → Implementation → Testing → Delivery

[See detailed documentation](./feature/README.md)

### Future Teams (Coming Soon)
- **Greenfield Project Team** - Starting new projects from scratch
- **Migration Team** - Migrating codebases to new technologies
- **DevOps Team** - Infrastructure and deployment automation
- **Security Team** - Security audits and vulnerability fixes

## 🎨 How It Works

### 1. You Make a Request
```
"I want to add user password reset functionality"
```

### 2. Feature Orchestrator Takes Control
- Assesses task complexity
- Determines which agents are needed
- Coordinates the workflow
- Tracks progress

### 3. Agents Work in Sequence

**For Small Tasks**:
```
Orchestrator → Coder → Tester → Orchestrator
```

**For Medium/Large Features**:
```
Orchestrator → Explorer → Product Manager → Scrum Master 
→ Coder → Tester → Orchestrator
```

### 4. You Get Quality Results
- Working code that follows your project's patterns
- Comprehensive tests
- Full documentation
- Progress tracking throughout

## 🛠️ Setup

### Prerequisites
- **Kilo Code** (Recommended for best performance)
- **Grok Code Fast model** (Strongly suggested for optimal results)
- A project to work on

> **💡 Pro Tip**: For the best experience, use Kilo Code with the Grok Code Fast model. This combination provides optimal performance and agent coordination.

### Installation

1. **Clone this repository**:
```bash
git clone https://github.com/oceceli/specialized-agent-teams.git
cd specialized-agent-teams
```

2. **Extract `.kilocodemodes` to your project root**:
```bash
# Copy the .kilocodemodes file to your project root
cp feature/.kilocodemodes /path/to/your/project/.kilocodemodes
```

3. **Copy the feature team structure** (optional but recommended):
```bash
# Copy the entire feature directory to your project
cp -r feature /path/to/your/project/
```

4. **Configure for your project**:
```bash
cd /path/to/your/project/feature
# Edit settings.md to match your project
code rules/settings.md
```

### Quick Start

1. **Open Kilo Code** in your project
2. **Select Feature Orchestrator mode** from available custom modes
3. **Make your request**: "I want to add [your feature]"
4. **Follow the workflow**: The Orchestrator will guide you through the process

## 📖 Usage Guide

### Starting with Feature Orchestrator

The Feature Orchestrator is your entry point. Start by selecting it from Kilo Code's custom modes:

```
@feature-orchestrator I want to add user authentication
```

The Orchestrator will:
1. ✅ Assess task complexity
2. ✅ Check if codebase analysis is needed
3. ✅ Route to appropriate agents
4. ✅ Create workspace structure
5. ✅ Track progress throughout

### Understanding Task Complexity

**Small Tasks** (goes directly to Coder):
- Single endpoint additions
- Minor UI changes
- Simple bug fixes
- Small configuration changes

**Medium/Large Tasks** (full epic process):
- Multiple components involved
- Complex business logic
- New feature development
- Integration work
- Database changes

**Structural Changes** (entire team engaged):
- Architecture refactoring
- Technology stack changes
- Major optimizations
- Security implementations

### Working with Agents

Each agent knows when to:
- ✅ Read the necessary documentation
- ✅ Ask clarifying questions
- ✅ Perform their specific tasks
- ✅ Update progress tracking
- ✅ Hand off to the next agent

**You don't need to manage this** - the agents coordinate automatically!

## 📁 Project Structure

```
specialized-agent-teams/
├── README.md                    # This file - general overview
│
└── feature/                     # Feature development team
    ├── README.md               # Detailed feature team guide
    ├── .kilocodemodes          # Agent configurations for Kilo Code (EXTRACT TO YOUR PROJECT ROOT)
    │
    ├── agents/                 # Agent role definitions
    │   ├── feature-orchestrator.md
    │   ├── explorer.md
    │   ├── product-manager.md
    │   ├── scrum-master.md
    │   ├── coder.md
    │   └── tester.md
    │
    ├── rules/                  # Rules and configuration
    │   ├── common.md           # Common rules for all agents
    │   ├── settings.md         # Project-specific settings
    │   └── [agent-name]/       # Agent-specific custom rules
    │
    ├── overview/               # Created by Explorer
    │   ├── PRD.md              # Project requirements document
    │   └── feature_*.md        # Feature documentation
    │
    └── workshop/               # Active work directory
        └── [feature-name]/     # Per-feature workspace
            ├── progress.md     # Progress tracking
            ├── epics/          # Epic documentation
            └── stories/        # Story documentation
```

## 🎯 Key Features

### Automatic Progress Tracking
Every step is documented in `progress.md`:
```markdown
| Agent | Status | Progress |
|-------|--------|----------|
| Explorer (Expo) | ✅ Complete | Created PRD and feature docs |
| Product Manager (Puma) | 🔄 In Progress | Creating epics... |
| Scrum Master (Scrummy) | ⏳ Pending | Not started |
```

### Intelligent Codebase Analysis
Explorer analyzes your entire project once and creates documentation that all other agents reference, ensuring consistency.

### Epic-Driven Development
Product Manager creates detailed epics with:
- User value proposition
- Technical approach
- Risk assessment
- Integration points
- Testing requirements

### Story-Based Implementation
Scrum Master breaks epics into implementable stories with:
- Clear acceptance criteria
- Specific tasks for Coder
- Dependencies mapped
- Test requirements defined

### Quality Assurance Built-In
Tester verifies:
- ✅ Functionality meets requirements
- ✅ Edge cases handled
- ✅ Security considerations
- ✅ Performance acceptable
- ✅ Integration points work

## 🔧 Customization

### Project-Specific Configuration

Edit `feature/rules/settings.md`:
```markdown
## Project Information
project_name: "Your Project Name"
project_type: "web_application"
primary_language: "typescript"

## Communication Settings
user_language: "turkish"  # or "english"
documentation_language: "english"

## Workflow Settings
require_tests: true
require_documentation: true
```

### Adding Custom Rules

Create agent-specific rules:
```bash
# For Coder
echo "- Always use async/await" > feature/rules/coder/async_rules.md

# For Tester
echo "- Run E2E tests on staging" > feature/rules/tester/e2e_rules.md
```

### Extending Agent Behavior

Modify agent definition files in `feature/agents/` to customize:
- Role responsibilities
- Workflow steps
- Output formats
- Quality standards

## 💡 Best Practices

### 1. Start with Feature Orchestrator
Always begin your work by selecting the Feature Orchestrator agent. It will coordinate everything.

### 2. Keep Overview Updated
Let Explorer analyze your codebase periodically to keep documentation fresh.

### 3. Be Specific in Requests
```
❌ "Add login"
✅ "Add email/password login with password reset functionality"
```

### 4. Trust the Process
Let agents work through their workflow. Each step adds value and ensures quality.

### 5. Review Progress Regularly
Check `workshop/[feature-name]/progress.md` to see what's happening.

### 6. Provide Feedback
If something isn't right, tell the agent. They'll ask Product Manager or adjust the approach.

## 🤝 Contributing

Contributions are welcome! Here's how:

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/amazing-feature`
3. Make your changes
4. Test with real projects
5. Commit: `git commit -m 'Add amazing feature'`
6. Push: `git push origin feature/amazing-feature`
7. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments

- Built for Kilo Code
- Optimized for Grok Code Fast model
- Inspired by agile development practices
- Designed for real-world software development workflows

## 📞 Support

- **Issues**: [GitHub Issues](https://github.com/oceceli/specialized-agent-teams/issues)
- **Discussions**: [GitHub Discussions](https://github.com/oceceli/specialized-agent-teams/discussions)
- **Documentation**: See individual team READMEs
- **Kilo Code**: [Kilo Code Documentation](https://kilocode.dev)

## 🗺️ Roadmap

- [ ] Feature Development Team (✅ Complete)
- [ ] Greenfield Project Team
- [ ] Migration Team
- [ ] DevOps Team
- [ ] Security Audit Team
- [ ] Performance Optimization Team

---

**Made with ❤️ for better AI-assisted development**

Start building better software with specialized agent teams today!
