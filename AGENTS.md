# CMZ Agent Configuration

## Overview

This repository is configured with the **CMZ (Context, Memory, Zenith)** agent - an advanced autonomous agent with self-healing, self-learning, and self-evolving capabilities.

## Structure

```
.opencode/
├── agent/
│   └── CMZ.json              # CMZ agent configuration
├── config/
│   └── oh-my-opencode.json   # OpenCode CLI configuration
└── skills/
    └── agent-framework/      # Framework skill documentation
        └── SKILL.md

supplementary-repos/
├── oh-my-opencode/           # Agent harness with orchestration
├── superpowers/              # Systematic debugging framework
├── UltraRAG/                 # MCP-based RAG framework
└── system_prompts_leaks/     # Prompt optimization reference
```

## Agent Models

CMZ is configured to use the following models:

- **Primary**: `opencode/kimi-k2.5-free` - Main orchestration
- **Secondary**:
  - `opencode/glm-4.7-free` - Exploration and librarian tasks
  - `opencode/minimax-m2.1-free` - Oracle and debugging

## Capabilities

CMZ can perform:
- Code analysis and bug detection
- Automated refactoring
- Test generation and execution
- Documentation maintenance
- Git operations and CI/CD management
- Multi-agent orchestration

## Workflow

1. **Discovery** - Analyze codebase and identify issues
2. **Planning** - Create detailed task plans
3. **Execution** - Implement changes
4. **Verification** - Validate changes work
5. **Reflection** - Optimize for future iterations

## Usage

To activate CMZ in your OpenCode CLI:

```bash
opencode run "Your task here" --agent CMZ
```

Or with ultrawork mode for maximum efficiency:

```bash
opencode run "ultrawork: Your complex task" --agent CMZ
```

## Supplementary Resources

### oh-my-opencode
The Best Agent Harness with Sisyphus orchestration. Provides:
- Multi-model orchestration
- Background task execution
- LSP and AST tools
- Claude Code compatibility

### superpowers
Agentic skills framework providing:
- Test-driven development workflow
- Systematic debugging methodology
- Subagent-driven development
- Brainstorming and planning tools

### UltraRAG
MCP-based RAG framework for:
- Low-code RAG pipeline orchestration
- Modular architecture
- Knowledge retrieval

## Anti-Patterns

Never:
- Create circular dependencies
- Build god classes
- Mix presentation with business logic
- Break existing functionality
- Over-engineer solutions

## Configuration Files

- `.opencode/agent/CMZ.json` - Agent behavior and capabilities
- `.opencode/config/oh-my-opencode.json` - Model and agent configurations
- `.opencode/skills/agent-framework/SKILL.md` - Framework documentation

## Updates

To update supplementary repositories:

```bash
cd supplementary-repos/<repo-name>
git pull origin main
```

## Support

For issues or questions:
1. Check the framework documentation in `.opencode/skills/`
2. Review the supplementary repository documentation
3. Create an issue in this repository
