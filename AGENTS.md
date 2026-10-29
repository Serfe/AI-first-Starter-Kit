# AI-first Starter Kit

This repository keeps shared AI development guidance in `.agents/` and project context in `.ai/`.

## Working agreement

- Read the relevant requirement in `.ai/requirements/` before implementing work.
- Consult `.ai/project-overview.md`, business rules, and architecture decisions when they apply.
- Follow the shared rules in `.agents/rules/`.
- Load a skill from `.agents/skills/` only when its workflow matches the task.
- Keep changes scoped, testable, and free of credentials or private information.
- Use [Conventional Commits](https://www.conventionalcommits.org/) for commit messages, such as `feat: add health endpoint` or `docs: clarify setup`.
- When a changelog is introduced, maintain it according to [Keep a Changelog](https://keepachangelog.com/); do not create or update a changelog unless the task explicitly requires it.

## Workflows

- Implement a scoped requirement: `.agents/skills/implement-task/SKILL.md`
- Verify a change: `.agents/skills/verify-change/SKILL.md`
- Review a change: `.agents/skills/review-change/SKILL.md`
