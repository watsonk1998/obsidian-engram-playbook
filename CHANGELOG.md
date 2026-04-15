# Changelog

All notable changes to this project will be documented in this file.

This project follows a simple human-maintained changelog style.

## [Unreleased]

### Evaluated
- Naming strategy deep-dive (2026-04-14): Scanned AGENTS.md, README, skills/, docs/ to assess whether to bind "DeepSeek" in the repo name. Finding: zero DeepSeek-related content exists in repo. Recommendation: keep `deepengram-harness` as the canonical name; `Deep-` prefix works as a coined term ("deep memory trace") without implying official DeepSeek integration. Alternative if explicit binding is desired: `engram-deepseek-harness` (requires adding DeepSeek integration content first).

### Fixed
- Prevented pipeline stalling during API burst limits (HTTP 429 single-day quota exhaustion) by implementing fail-fast termination and layer-segregation (routing bulk ingestion to `flash` and inference to `pro` models).

### Added
- GitHub Actions workflow for `doctor.sh` and `sanitize_scan.sh`
- Repository homepage architecture diagram (`assets/architecture-overview.svg`)
- Getting-started flow diagram (`assets/getting-started-flow.svg`)
- GitHub social preview asset (`assets/social-preview.png`)
- Issue templates and pull request template under `.github/`
- Two alternate social preview images: `social-preview-minimal.png` and `social-preview-system-map.png`

### Changed
- Added README badges and architecture overview section to both English and Chinese entry pages
- Added getting-started flow and project metadata section to both English and Chinese entry pages

### Planned
- Refine public examples
- Expand bilingual entry points where useful
- Add more polished visual assets and onboarding guidance

## [0.1.0] - 2026-03-18

### Added
- Initial public repository skeleton
- README homepage for the public project
- Simplified Chinese README entry point (`README.zh-CN.md`)
- Core Chinese docs under `docs/zh-CN/`
- `SECURITY.md`
- `CONTRIBUTING.md`
- Publishing-boundary guidance
- Sanitization checklist
- Sanitization scan script
- Doctor script
- Sanitized templates for daily / weekly / monthly workflows
- Sanitized skill examples for the Obsidian + Engram workflow
- Example vault skeleton and sample notes

### Changed
- README upgraded to a more open-source-friendly project homepage
- Added default-English language switch with a Simplified Chinese README entry point
