# Obsidian Engram Playbook

**Engram-first knowledge governance for Obsidian + LLM agents**

> A public, sanitized framework for running an Obsidian vault with durable memory, periodic review loops, and agent-friendly workflows.

## Why this exists

Most “Obsidian setups” focus on plugins, aesthetics, or note-taking tricks.

This project focuses on something else:

- how to make **Obsidian usable as an operating surface**
- how to keep **durable memory outside chat context**
- how to let **LLM agents work inside a vault without creating chaos**
- how to run **daily / weekly / monthly review loops** without file sprawl

This repository is a **playbook**, not a private vault export.

## What this repository contains

This repo packages a reusable approach for combining:

- **Obsidian** as the working knowledge surface
- **Engram** as reusable long-term memory
- **LLM agents** as operators for writing, synthesis, and maintenance
- **Daily / weekly / monthly reviews** as the main governance rhythm

## Core principles

### 1. Default-on Obsidian base layer

Users should not need to remember tool names.

When the task involves Obsidian content, the agent should automatically apply the right base capability:

- `obsidian-markdown` for `.md`
- `obsidian-engram-frontmatter` for metadata
- `obsidian-bases` for `.base`
- `json-canvas` for `.canvas`
- `defuddle` for web clipping
- `obsidian-cli` for vault/plugin automation

### 2. Engram-first memory

Reusable lessons, rules, handoffs, and patterns belong in Engram.  
Obsidian remains the readable workspace and review surface.

### 3. Evidence-first writing

Notes, reviews, and summaries should be grounded in:

- source notes
- linked artifacts
- changed files
- explicit user facts

If evidence is missing, say so.

### 4. Minimal file proliferation

Do not create extra files just to feel structured.

Prefer:

- the daily journal as the default sink
- weekly/monthly synthesis as periodic outputs
- Engram for reusable knowledge
- standalone notes only when they add long-term value

## Who this is for

This repo may be useful if you want to combine:

- Obsidian as a serious working environment
- AI agents as note operators and synthesizers
- periodic review workflows
- durable memory beyond a single chat window

## Quick start

1. Read `docs/architecture.md`
2. Review `docs/publishing-boundary.md`
3. Copy templates from `templates/`
4. Study the sanitized examples in `skills/`
5. Run `scripts/doctor.sh`
6. Run `scripts/sanitize_scan.sh` before publishing anything derived from this repo

## Repository tour

```text
docs/        architecture, governance, publishing boundaries, sanitization guidance
templates/   reusable note / report / Base / Canvas templates
skills/      sanitized skill examples for agents
scripts/     generic maintenance and sanitization helpers
examples/    safe vault skeleton and sample notes
assets/      public-safe diagrams and screenshots
```

## What is intentionally excluded

This public repository does **not** include:

- real journals
- real weekly/monthly reviews
- real Engram memories
- private MCP configs
- secrets, tokens, API keys
- employer/client/project-sensitive data
- device-specific absolute paths from a real machine

## Publishing boundary

Before publishing your own derivative version, review:

- absolute paths
- people / org / project names
- screenshots and attachments
- metadata fields
- scripts with hard-coded values
- git history

See:

- `docs/sanitization-checklist.md`
- `docs/publishing-boundary.md`
- `SECURITY.md`

## Current contents

Included in v1:

- public repo structure
- sanitization checklist
- publishing-boundary guidance
- first-pass architecture docs
- note and report templates
- sanitized skill examples
- generic helper scripts

## Suggested adaptation path

1. Copy the templates into your own vault
2. Replace placeholder paths with your local paths
3. Adjust frontmatter conventions for your workflow
4. Keep private notes and memory stores outside this repo
5. Treat this repo as a framework, not as a vault dump

## Status

Early public skeleton.  
The goal is clarity and safety first, not completeness.

## License

MIT for framework docs, templates, and scripts unless otherwise noted.
