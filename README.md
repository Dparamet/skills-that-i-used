# Claude Code Skills Collection

> A curated personal archive of Claude Code skills and plugins actively used to augment AI-assisted development workflows.

---

## Overview

This repository is a snapshot of all Claude Code **skills** and **plugins** installed and used in my development environment. It serves as:

- A **backup** of the skill configurations under `~/.claude/skills/` and `~/.claude/plugins/marketplaces/`
- A **reference catalog** for onboarding or restoring the same environment on a new machine
- A **changelog** for tracking which skills are added, updated, or removed over time

Skills in Claude Code are instruction sets (stored as Markdown) that guide Claude's behavior for specific tasks — from animation engineering to systematic debugging to lazy-first development philosophy.

---

## Repository Structure

```
skills-that-i-used/
├── skills/                  # All installed skill directories
│   ├── ponytail/            # Lazy-first development philosophy
│   ├── hyperframes/         # HTML video composition engine
│   ├── systematic-debugging/
│   └── ... (51 skills total)
├── plugins/                 # Installed marketplace plugins
│   ├── claude-plugins-official/
│   ├── DietrichGebert-ponytail/
│   ├── hope1026-roblox-mcp/
│   └── skills-directory-skill-codex/
└── README.md
```

---

## Skills Catalog

### Animation & Creative Engineering

Skills for building deterministic, seek-driven animations inside [HyperFrames](https://hyperframes.dev) and the browser.

| Skill | Description | Source |
|-------|-------------|--------|
| `animejs` | Anime.js adapter patterns — registering animations on `window.__hfAnime`, seek-driven timelines, deterministic rendering | `claude-plugins-official` |
| `gsap` | GSAP `to()`, `from()`, `fromTo()`, easing, stagger, timelines, `quickTo`, `will-change` performance patterns | `claude-plugins-official` |
| `css-animations` | CSS keyframes, `animation-delay` timing, `animation-fill-mode`, `animation-play-state` — HyperFrames-compatible | `claude-plugins-official` |
| `waapi` | Web Animations API — `element.animate()`, `Animation.currentTime` seeking, `KeyframeEffect`, native browser animations | `claude-plugins-official` |
| `lottie` | Lottie / dotLottie adapter — `lottie-web` JSON, `.lottie` files, `@lottiefiles/dotlottie-web`, After Effects exports | `claude-plugins-official` |
| `three` | Three.js / WebGL — deterministic scenes, `AnimationMixer`, camera motion, shader visuals, `hf-seek` events | `claude-plugins-official` |
| `typegpu` | TypeGPU / raw WebGPU — WGSL shaders, compute pipelines, liquid glass, particle systems, GPU canvas layers | `claude-plugins-official` |

---

### HyperFrames Video Production

Skills covering the full HyperFrames video composition workflow.

| Skill | Description | Source |
|-------|-------------|--------|
| `hyperframes` | Core composition authoring — title cards, overlays, captions, voiceovers, audio-reactive visuals, scene transitions | `claude-plugins-official` |
| `hyperframes-cli` | Dev-loop CLI — `npx hyperframes init/lint/inspect/preview/render/doctor` | `claude-plugins-official` |
| `hyperframes-media` | Asset preprocessing — TTS (Kokoro), transcription (Whisper), background removal (u2net) | `claude-plugins-official` |
| `hyperframes-registry` | Install and wire registry blocks/components — `hyperframes add`, `hyperframes.json`, block wiring | `claude-plugins-official` |
| `contribute-catalog` | Author and ship new HyperFrames registry blocks or components as upstream PRs | `claude-plugins-official` |
| `remotion-to-hyperframes` | Port Remotion (React) video compositions to HyperFrames HTML | `claude-plugins-official` |
| `website-to-hyperframes` | Convert websites into HyperFrames compositions | `claude-plugins-official` |
| `tailwind` | Tailwind CSS v4.2 browser-runtime patterns inside HyperFrames — theme tokens, v3→v4 migration | `claude-plugins-official` |

---

### Code Quality & Engineering Practices

| Skill | Description | Source |
|-------|-------------|--------|
| `code-review-and-quality` | Multi-axis code review across correctness, design, and maintainability axes | `claude-plugins-official` |
| `code-simplification` | Refactor for clarity without behavior change — reduce accidental complexity | `claude-plugins-official` |
| `debugging-and-error-recovery` | Systematic root-cause debugging for test failures, build breaks, unexpected errors | `claude-plugins-official` |
| `systematic-debugging` | Disciplined debug loop: reproduce → minimise → hypothesise → instrument → fix → regression-test | `claude-plugins-official` |
| `diagnose` | Hard-bug diagnosis — structured investigation for regressions and performance issues | `claude-plugins-official` |
| `security-and-hardening` | Harden code against OWASP vulnerabilities — input validation, auth, session management | `claude-plugins-official` |
| `performance-optimization` | Core Web Vitals, profiling, load-time improvements, bottleneck analysis | `claude-plugins-official` |
| `tdd` | Test-Driven Development — write tests before implementation code | `claude-plugins-official` |
| `test-driven-development` | Drive all logic changes with tests that prove behavior | `claude-plugins-official` |

---

### Frontend & UI Engineering

| Skill | Description | Source |
|-------|-------------|--------|
| `frontend-ui-engineering` | Production-quality UIs — components, layouts, state, accessible and polished interfaces | `claude-plugins-official` |
| `impeccable` | UI design critique, visual hierarchy, UX review, typography, color, motion, micro-interactions | `claude-plugins-official` |
| `clone-website` | Reverse-engineer and clone any website — parallel section extraction, asset scraping, pixel-perfect rebuild | `claude-plugins-official` |

---

### Planning & Specification

| Skill | Description | Source |
|-------|-------------|--------|
| `spec-driven-development` | Create specs before writing code — requirements, acceptance criteria, implementation details | `claude-plugins-official` |
| `planning-and-task-breakdown` | Break large work into ordered implementable tasks, estimate scope, identify parallelism | `claude-plugins-official` |
| `incremental-implementation` | Deliver changes incrementally — one file at a time, regular commits, prevents large diffs | `claude-plugins-official` |
| `writing-plans` | Structured plan documents for multi-step tasks before touching code | `claude-plugins-official` |

---

### Ponytail — Lazy-First Development

A philosophy plugin enforcing YAGNI, stdlib-first, minimum-viable-code thinking.

> **Source:** [`DietrichGebert/ponytail`](https://github.com/DietrichGebert/ponytail) — third-party Claude Code plugin

| Skill | Description |
|-------|-------------|
| `ponytail` | Core mode — laziest solution that works; questions if the task needs to exist at all |
| `ponytail-audit` | Whole-repo audit for over-engineering; ranked list of what to delete or simplify |
| `ponytail-review` | Diff-focused review hunting only for complexity to remove |
| `ponytail-debt` | Harvest all `ponytail:` comments into a debt ledger |
| `ponytail-gain` | Scoreboard showing token/code savings from ponytail mode |
| `ponytail-help` | Quick-reference card for all ponytail modes and commands |

---

### Workflow & Productivity

| Skill | Description | Source |
|-------|-------------|--------|
| `caveman` | Ultra-compressed communication — ~75% token reduction, zero filler, full technical accuracy | `claude-plugins-official` |
| `handoff` | Compact the current conversation into a handoff document for a fresh agent to continue | `claude-plugins-official` |
| `grill-me` | Relentless design interview — stress-test a plan by resolving every branch of a decision tree | `claude-plugins-official` |
| `codex` | Run OpenAI Codex CLI (`codex exec`, `codex resume`) for code analysis and refactoring | [`skills-directory-skill-codex`](https://github.com/klaudworks/ralph-meets-rex) |

---

### Roblox / Game Development

> **Source:** [`hope1026/roblox-mcp`](https://github.com/hope1026/roblox-mcp) — WEPPY MCP server for Roblox Studio

| Skill | Description |
|-------|-------------|
| `weppy-roblox-mcp-guide` | Control a live Roblox Studio session via MCP — scripts, instances, terrain, lighting, audio, animations |
| `weppy-roblox-sync-guide` | Bidirectional sync between AI agent and Roblox Studio — conflict resolution, sync format, explorer workflow |

---

### Lightweight Custom Skills

Simple single-file skills for common day-to-day operations:

| Skill | Purpose |
|-------|---------|
| `fix` | Quick bug fix — diagnose, isolate, fix with minimal scope |
| `plan` | Strategic planning and step breakdown before coding |
| `review` | Code review and quality assessment for PRs |
| `spec` | Specification and requirements documentation |
| `test` | Test writing, QA, and validation |
| `safe` | Conservative, non-breaking, production-safe changes |
| `simple` | Single-file low-risk tasks — copy edits, icon swaps, minor tweaks |
| `incremental` | Build large features step-by-step with regular commits |
| `frontend` | Project-specific frontend component and styling work |

---

## Plugin Sources

| Plugin | Author | Description |
|--------|--------|-------------|
| [`claude-plugins-official`](https://github.com/anthropics/claude-code) | Anthropic | Official curated skill catalog for Claude Code |
| [`DietrichGebert-ponytail`](https://github.com/DietrichGebert/ponytail) | Dietrich Gebert | Lazy-first development philosophy plugin |
| [`skills-directory-skill-codex`](https://github.com/klaudworks/ralph-meets-rex) | klaudworks | OpenAI Codex CLI integration for Claude Code |
| [`hope1026-roblox-mcp`](https://github.com/hope1026/roblox-mcp) | hope1026 | MCP server for AI-driven Roblox Studio control |

---

## How to Restore This Environment

```bash
# 1. Install Claude Code CLI
npm install -g @anthropic-ai/claude-code

# 2. Copy skills into place
cp -r skills/* ~/.claude/skills/

# 3. Copy plugins into place
cp -r plugins/* ~/.claude/plugins/marketplaces/

# 4. Verify skills are available inside Claude Code
# Type /fix or /ponytail to confirm
```

---

## Maintenance

This repository is updated whenever skills are added, modified, or removed from the local environment. To sync:

```bash
# From the repo root
cp -r ~/.claude/skills/* ./skills/
cp -r ~/.claude/plugins/marketplaces/* ./plugins/
git add -A
git commit -m "sync: update skills snapshot $(date +%Y-%m-%d)"
```

---

## License

Each skill and plugin retains the license of its original author. See individual `plugins/<name>/` directories for licensing details.

---

*Last synced: 2026-06-24 | Environment: Windows 11 · Claude Code · claude-sonnet-4-6*
