<div align="center">

# ✦ Claude Code Skills Collection ✦

**A curated personal archive of Claude Code skills & plugins**  
*actively powering AI-assisted development workflows*

---

![Skills](https://img.shields.io/badge/Skills-51-6366f1?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI+PHBhdGggZmlsbD0id2hpdGUiIGQ9Ik0xMiAyQzYuNDggMiAyIDYuNDggMiAxMnM0LjQ4IDEwIDEwIDEwIDEwLTQuNDggMTAtMTBTMTcuNTIgMiAxMiAyem0tMiAxNWwtNS01IDEuNDEtMS40MUwxMCAxNC4xN2w3LjU5LTcuNTlMMTkgOGwtOSA5eiIvPjwvc3ZnPg==)
![Plugins](https://img.shields.io/badge/Plugins-4-ec4899?style=for-the-badge)
![Platform](https://img.shields.io/badge/Platform-Windows%2011-0078D4?style=for-the-badge&logo=windows11)
![Claude](https://img.shields.io/badge/Claude%20Code-Sonnet%204.6-D97706?style=for-the-badge)
![Last Sync](https://img.shields.io/badge/Last%20Sync-2026--06--24-22c55e?style=for-the-badge)

</div>

---

## 📖 What Is This?

This repository is a **personal snapshot** of every Claude Code skill and plugin installed in my development environment. Think of it as a dotfiles repo — but for AI cognition.

Claude Code **skills** are Markdown instruction sets that guide Claude's behavior for specific tasks. Instead of repeating yourself every session, skills encode your workflow preferences, patterns, and constraints once — and activate on demand via `/skill-name`.

This repo exists to:

- 💾 **Back up** all skill configs from `~/.claude/skills/` and `~/.claude/plugins/marketplaces/`
- 📋 **Document** what each skill does and where it came from
- 🔄 **Restore** the same environment on any new machine in minutes
- 📈 **Track** skills added, updated, or retired over time

---

## 🗂️ Repository Structure

```
skills-that-i-used/
│
├── 📁 skills/                        # 51 installed skill directories
│   ├── ponytail/                     # Lazy-first development philosophy
│   ├── hyperframes/                  # HTML video composition engine
│   ├── systematic-debugging/         # Disciplined bug investigation
│   ├── frontend-ui-engineering/      # Production-quality UI building
│   └── ... (47 more)
│
├── 📁 plugins/                       # 4 marketplace plugin sources
│   ├── claude-plugins-official/      # Anthropic's official skill catalog
│   ├── DietrichGebert-ponytail/      # Lazy-first philosophy plugin
│   ├── hope1026-roblox-mcp/          # Roblox Studio MCP server
│   └── skills-directory-skill-codex/ # OpenAI Codex CLI integration
│
└── README.md
```

---

## 🎨 Skills Catalog

### 🎬 Animation & Creative Engineering

> Skills for deterministic, seek-driven animations in [HyperFrames](https://hyperframes.dev) and the browser.

| Skill | What It Does |
|-------|-------------|
| `animejs` | Anime.js adapter — `window.__hfAnime` registration, seek-driven timelines, deterministic rendering |
| `gsap` | GSAP `to()` / `from()` / `fromTo()`, easing, stagger, timelines, `quickTo`, performance patterns |
| `css-animations` | CSS keyframes, `animation-delay` timing, `fill-mode`, `play-state` — HyperFrames-compatible |
| `waapi` | Web Animations API — `element.animate()`, `currentTime` seeking, `KeyframeEffect`, native browser |
| `lottie` | Lottie / dotLottie — `lottie-web` JSON, `.lottie` files, After Effects exports, deterministic playback |
| `three` | Three.js / WebGL — deterministic scenes, `AnimationMixer`, camera motion, shader visuals |
| `typegpu` | TypeGPU / raw WebGPU — WGSL shaders, compute pipelines, liquid glass, particle systems |

---

### 🎥 HyperFrames Video Production

> Full workflow coverage for HTML-based video composition.

| Skill | What It Does |
|-------|-------------|
| `hyperframes` | Core authoring — title cards, overlays, captions, voiceovers, audio-reactive visuals, transitions |
| `hyperframes-cli` | Dev loop — `npx hyperframes init / lint / inspect / preview / render / doctor` |
| `hyperframes-media` | Asset preprocessing — TTS (Kokoro), transcription (Whisper), background removal (u2net) |
| `hyperframes-registry` | Install & wire registry blocks/components — `hyperframes add`, `hyperframes.json` wiring |
| `contribute-catalog` | Author new HyperFrames registry blocks or components and ship as upstream PRs |
| `remotion-to-hyperframes` | Port Remotion (React) video compositions into HyperFrames HTML |
| `website-to-hyperframes` | Convert any website into a HyperFrames composition |
| `tailwind` | Tailwind CSS v4.2 browser-runtime patterns, theme tokens, v3 → v4 migration guide |

---

### 🔍 Code Quality & Engineering Practices

| Skill | What It Does |
|-------|-------------|
| `code-review-and-quality` | Multi-axis review across correctness, design, and maintainability |
| `code-simplification` | Refactor for clarity without behavior change — kill accidental complexity |
| `debugging-and-error-recovery` | Systematic root-cause debugging for failures, breaks, and surprises |
| `systematic-debugging` | Full loop: reproduce → minimise → hypothesise → instrument → fix → regression-test |
| `diagnose` | Hard-bug investigation — structured tracing for regressions and perf issues |
| `security-and-hardening` | Harden against OWASP top 10 — input validation, auth, sessions, integrations |
| `performance-optimization` | Core Web Vitals, profiling, load-time improvements, bottleneck analysis |
| `tdd` | Test-Driven Development — write tests before writing implementation |
| `test-driven-development` | Drive all logic changes with tests that prove behavior, not just coverage |

---

### 🖥️ Frontend & UI Engineering

| Skill | What It Does |
|-------|-------------|
| `frontend-ui-engineering` | Production-quality UI — components, layouts, state, accessible and polished interfaces |
| `impeccable` | Design critique — visual hierarchy, UX review, typography, color, motion, micro-interactions |
| `clone-website` | Reverse-engineer and clone any website — parallel section extraction, pixel-perfect rebuild |

---

### 🗺️ Planning & Specification

| Skill | What It Does |
|-------|-------------|
| `spec-driven-development` | Specs before code — requirements, acceptance criteria, implementation details |
| `planning-and-task-breakdown` | Break large work into ordered tasks, estimate scope, identify parallelism |
| `incremental-implementation` | Deliver incrementally — one file at a time, regular commits, no giant diffs |
| `writing-plans` | Structured plan documents for multi-step tasks before touching any code |

---

### 🦥 Ponytail — Lazy-First Development

<div align="center">

*"The best code is the code never written."*

</div>

> **Source:** [`DietrichGebert/ponytail`](https://github.com/DietrichGebert/ponytail) — third-party Claude Code plugin  
> A philosophy plugin enforcing **YAGNI**, stdlib-first, minimum-viable-code thinking across every response.

| Skill | What It Does |
|-------|-------------|
| `ponytail` | Core mode — enforces the laziest solution that actually works; questions if the task needs to exist |
| `ponytail-audit` | Whole-repo audit — ranked list of everything to delete, simplify, or replace with stdlib |
| `ponytail-review` | Diff-focused review hunting only for complexity to remove |
| `ponytail-debt` | Harvest all `ponytail:` comments into a tracked debt ledger |
| `ponytail-gain` | Scoreboard showing measured token/code savings from ponytail mode |
| `ponytail-help` | Quick-reference card for all ponytail modes, skills, and commands |

---

### ⚙️ Workflow & Productivity

| Skill | What It Does |
|-------|-------------|
| `caveman` | Ultra-compressed comms — ~75% token reduction, zero filler, full technical accuracy |
| `handoff` | Compact the current session into a handoff doc for a fresh agent to continue seamlessly |
| `grill-me` | Relentless design interview — stress-test any plan by resolving every branch of a decision tree |
| `codex` | Run OpenAI Codex CLI (`codex exec`, `codex resume`) for code analysis and refactoring |

---

### 🎮 Roblox / Game Development

> **Source:** [`hope1026/roblox-mcp`](https://github.com/hope1026/roblox-mcp) — WEPPY MCP server for Roblox Studio

| Skill | What It Does |
|-------|-------------|
| `weppy-roblox-mcp-guide` | Control a live Roblox Studio session — scripts, instances, terrain, lighting, audio, animations |
| `weppy-roblox-sync-guide` | Bidirectional AI ↔ Studio sync — conflict resolution, sync format, explorer workflow |

---

### 🔧 Lightweight Custom Skills

> Simple single-file skills for common day-to-day operations.

| Skill | Purpose |
|-------|---------|
| `fix` | Quick bug fix — diagnose, isolate, resolve with minimal scope change |
| `plan` | Strategic planning and step breakdown before coding |
| `review` | Code review and quality assessment for PRs |
| `spec` | Specification and requirements documentation |
| `test` | Test writing, QA, and validation |
| `safe` | Conservative, non-breaking, production-safe changes only |
| `simple` | Single-file low-risk tasks — copy edits, icon swaps, minor tweaks |
| `incremental` | Build large features step-by-step with regular commits |
| `frontend` | Project-specific frontend component and styling work |

---

## 📦 Plugin Sources

| Plugin | Maintainer | Purpose |
|--------|-----------|---------|
| [claude-plugins-official](https://github.com/anthropics/claude-code) | Anthropic | Official curated skill catalog for Claude Code |
| [DietrichGebert-ponytail](https://github.com/DietrichGebert/ponytail) | Dietrich Gebert | Lazy-first development philosophy |
| [skills-directory-skill-codex](https://github.com/klaudworks/ralph-meets-rex) | klaudworks | OpenAI Codex CLI integration |
| [hope1026-roblox-mcp](https://github.com/hope1026/roblox-mcp) | hope1026 | AI-driven Roblox Studio control via MCP |

---

## 🚀 Restore This Environment

```bash
# 1. Install Claude Code
npm install -g @anthropic-ai/claude-code

# 2. Clone this repo
git clone https://github.com/Dparamet/skills-that-i-used.git
cd skills-that-i-used

# 3. Restore skills and plugins
cp -r skills/* ~/.claude/skills/
cp -r plugins/* ~/.claude/plugins/marketplaces/

# 4. Verify inside Claude Code — type /ponytail or /handoff to confirm
```

---

## 🔄 Keeping It in Sync

```bash
# Sync latest skills from your local environment
cp -r ~/.claude/skills/* ./skills/
cp -r ~/.claude/plugins/marketplaces/* ./plugins/
git add -A
git commit -m "sync: update skills snapshot $(date +%Y-%m-%d)"
git push
```

---

## 📄 License

Each skill and plugin retains the license of its original author.  
See individual `plugins/<name>/` directories for details.

---

<div align="center">

*Last synced: **2026-06-24** · Environment: **Windows 11** · **Claude Code** · **claude-sonnet-4-6***

</div>
