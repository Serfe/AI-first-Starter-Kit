# AI-first Starter Kit

A lightweight, open-source reference for exploring AI-first software development with shared agents, skills, rules, and project context.

## What’s included

- Canonical agent roles, rules, and reusable workflows in `.agents/`
- Project context, requirements, and architecture decisions in `.ai/`
- Small adapters for Codex, Claude Code, and OpenCode
- An intentionally empty application extension point in `app/`

## Getting started

1. Clone this repository.
2. Choose Codex, Claude Code, or OpenCode.
3. Read `AGENTS.md` and `.ai/README.md`.
4. Start with `.ai/requirements/r001-example.md` and use the implementation, verification, and review workflows as appropriate.

## Supported tools

| Tool | Integration |
| --- | --- |
| Codex | Reads `AGENTS.md`; shared workflows live in `.agents/skills/`. |
| Claude Code | `CLAUDE.md` imports `AGENTS.md`; `.claude/skills/` links to canonical workflows. |
| OpenCode | `opencode.json` loads the canonical agent prompts directly. |

## Repository structure

```text
.agents/   Shared roles, rules, and task workflows
.ai/       Product and technical context
.claude/   Claude Code adapter
.codex/    Optional local Codex configuration
.opencode/ Optional local OpenCode extensions
app/       Application extension point
tests/     Application tests
```

## Example workflow

1. Read a requirement and applicable context in `.ai/`.
2. Follow `implement-task` to make a focused change.
3. Follow `verify-change` to run relevant checks and report evidence.
4. Use `review-change` for an independent quality review.

## Scope and limitations

This repository is a lightweight, open-source reference for exploring AI-first software development using shared agents, skills, and project documentation. It is a practical starting point, not a complete production-ready development framework.

At Serfe, we use a more comprehensive internal approach based on years of software engineering and delivery experience. Its requirements management, project coordination, quality assurance, and delivery practices are intentionally outside the scope of this public starter kit.

The goal is to help developers understand the core concepts, experiment with supported AI coding tools, and adapt the structure to their own projects.

## Contributing

Keep shared guidance canonical in `.agents/`, avoid duplicating prompts across tool adapters, and do not contribute credentials, customer data, or internal URLs.

## License

MIT. See [LICENSE](LICENSE).
