# CODEX.md (codex-md)

CODEX.md is a project-level Markdown memory file that the OpenAI Codex CLI loads to bootstrap an AI coding agent with persistent project instructions, coding conventions, build and test commands, and team conventions. The OpenAI Codex CLI now standardizes on AGENTS.md as the canonical filename, with CODEX.md and codex.md historically used and still recognized as fallback configuration filenames. Files are discovered through a three-tier hierarchy spanning the user's home directory, the Git repository root, and the current working directory, with closer files overriding earlier guidance when concatenated into the model prompt.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/codex-md/refs/heads/main/apis.yml)

## Scope

- **Type:** Standard
- **Position:** Consuming
- **Access:** 3rd-Party

## Tags

- AI Agents
- AI Copilot
- Coding Standards
- Configuration
- Developer Workflow
- Memory
- OpenAI Codex

## Timestamps

- **Created:** 2025-01-01
- **Modified:** 2026-04-26

## Features

- Markdown-based freeform instruction format with no mandated schema
- Loaded automatically by Codex CLI before any task execution
- Three-tier discovery (home directory, Git repo root, current directory)
- Override file convention (AGENTS.override.md / CODEX.override.md)
- Concatenated merge order with closer files taking precedence
- Equivalent role to CLAUDE.md (Claude Code) and .cursorrules (Cursor)
- Designed to encode build commands, test commands, lint rules, and conventions
- Agentic memory primitive for persistent project context across CLI sessions

## Use Cases

- Pin a repository to specific package managers, formatters, and linters
- Document non-obvious build, test, or migration commands for the agent
- Establish project-wide coding standards (naming, error handling, imports)
- Capture team norms (PR descriptions, commit style, branch naming)
- Restrict the agent from touching protected files or directories
- Bridge organizational knowledge into AI-assisted development sessions

## Common Properties

- [Specification](https://developers.openai.com/codex/guides/agents-md)
- [Documentation](https://developers.openai.com/codex/cli)
- [GitHub](https://github.com/openai/codex)
- [Landing Page](https://developers.openai.com/codex)

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
