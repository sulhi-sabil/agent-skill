---
name: agent-skill-framework
description: Framework for managing and orchestrating CMZ agent with supplementary repositories. Use when setting up, configuring, or managing agent skills and capabilities.
---

# Agent Skill Framework

This framework provides a structured approach to managing the CMZ agent and its supplementary repositories.

## CMZ Agent Configuration

The CMZ (Context, Memory, Zenith) agent is configured in `.opencode/agent/CMZ.json` with the following characteristics:

- **Self-healing**: Automatically detects and fixes issues
- **Self-learning**: Improves from past interactions
- **Self-evolving**: Adapts to new patterns and requirements

## Supplementary Repositories

The following repositories are integrated as supplements to CMZ:

### 1. oh-my-opencode
- **Purpose**: Agent harness with Sisyphus orchestration
- **Location**: `supplementary-repos/oh-my-opencode/`
- **Key Features**:
  - Multi-model orchestration
  - Background task execution
  - LSP and AST tools integration
  - Claude Code compatibility layer

### 2. superpowers
- **Purpose**: Agentic skills framework with systematic debugging
- **Location**: `supplementary-repos/superpowers/`
- **Key Features**:
  - Test-driven development workflow
  - Systematic debugging methodology
  - Subagent-driven development
  - Brainstorming and planning tools

### 3. UltraRAG
- **Purpose**: MCP-based RAG framework for knowledge retrieval
- **Location**: `supplementary-repos/UltraRAG/`
- **Key Features**:
  - Low-code RAG pipeline orchestration
  - Modular MCP server architecture
  - Unified evaluation system
  - Visual pipeline builder

### 4. system_prompts_leaks
- **Purpose**: Reference collection for prompt optimization
- **Location**: `supplementary-repos/system_prompts_leaks/`
- **Key Features**:
  - System prompt examples from major AI systems
  - Prompt engineering patterns
  - Reference for optimizing agent behavior

## Model Configuration

CMZ agents are configured to use the following models:

- **Primary**: `opencode/kimi-k2.5-free` - Main orchestration and complex tasks
- **Secondary**: 
  - `opencode/glm-4.7-free` - Fast exploration and librarian tasks
  - `opencode/minimax-m2.1-free` - Oracle and debugging tasks

## Skills Integration

Skills are loaded from multiple sources:
1. `.opencode/skills/` - Project-specific skills
2. `supplementary-repos/oh-my-opencode/skills/` - Oh-my-opencode skills
3. `supplementary-repos/superpowers/skills/` - Superpowers skills

## Workflow

1. **Phase 1**: Setup and configuration (current)
2. **Phase 2**: Execute tasks with CMZ agent
3. **Phase 3**: Review and optimize
4. **Phase 4**: Merge and deploy

## Anti-Patterns

Always avoid:
- Circular dependencies
- God classes
- Mixing presentation with business logic
- Breaking existing functionality
- Over-engineering
