# CODEX.md (codex-md)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
