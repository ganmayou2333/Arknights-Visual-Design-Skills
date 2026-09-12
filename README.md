# Arknights Visual Design Skills

> A collection of AI Agent Skills for creating and evaluating content in the official art style of *Arknights* (明日方舟) — covering **UI Interface**, **Poster / Key Art**, and **Animation / Motion Design**.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Skills](https://img.shields.io/badge/Skills-2-3F72AF.svg)](#skills)
[![Categories](https://img.shields.io/badge/Categories-UI%20%7C%20Poster%20%7C%20Animation-56B6C9.svg)](#design-philosophy)
[![Arknights](https://img.shields.io/badge/Style-Arknights%20%2F%20%E6%98%8E%E6%97%A5%E6%96%B9%E8%88%9F-E08E45.svg)](#quick-reference)

---

## Table of Contents

- [Overview](#overview)
- [Skills](#skills)
- [Quick Start](#quick-start)
- [Quick Reference — Core Design Tokens](#quick-reference--core-design-tokens)
- [Design Philosophy](#design-philosophy)
- [Repository Structure](#repository-structure)
- [Demo Showcase](#demo-showcase)
- [Contributing](#contributing)
- [License](#license)
- [Copyright Notice](#copyright-notice)

---

## Overview

This repository hosts **two complementary skills** that share the same three categories but differ in depth:

| Skill | Depth | Best For |
|-------|-------|----------|
| **arknights-design-style-guide** | Full — 12 chapters per category, fully quantified | Complex production: multi-screen systems, key visual KV, PV storyboards, IP collabs |
| **arknights-visual-style** | Concise — essential reference + core taboos | Fast generation, lightweight integration, quick retouches |

> **Which to use?** Pick `arknights-design-style-guide` when you need precise, auditable specifications. Pick `arknights-visual-style` when you just need reliably "on-brand" output fast. They can coexist — compound tasks benefit from both.

---

## Skills

### 1. arknights-design-style-guide (Full Specification)

Each category contains a complete **12-chapter reference manual** with quantified parameters — hex colors, font weights, spacing scales, animation durations, opacity values — plus detailed taboo checklists.

| File | Description |
|------|-------------|
| [SKILL.md](arknights-design-style-guide/SKILL.md) | Main entry: YAML frontmatter, workflow, quick reference |
| [README.md](arknights-design-style-guide/README.md) | English documentation with installation guide |
| [readme_cn.md](arknights-design-style-guide/readme_cn.md) | 中文文档，含手动安装 + AI 提示词安装教程 |
| [references/ui-style.md](arknights-design-style-guide/references/ui-style.md) | Complete UI design specification (12 chapters) |
| [references/poster-style.md](arknights-design-style-guide/references/poster-style.md) | Complete poster / key art specification (12 chapters) |
| [references/animation-style.md](arknights-design-style-guide/references/animation-style.md) | Complete animation / motion specification (12 chapters) |

### 2. arknights-visual-style (Concise Reference)

A lightweight style reference with essential parameters and core taboos for each category.

| File | Description |
|------|-------------|
| [SKILL.md](arknights-visual-style/SKILL.md) | Main entry with style overview |
| [references/ui-style.md](arknights-visual-style/references/ui-style.md) | UI style reference |
| [references/poster-style.md](arknights-visual-style/references/poster-style.md) | Poster style reference |
| [references/animation-style.md](arknights-visual-style/references/animation-style.md) | Animation style reference |

---

## Quick Start

### Install

```bash
# Clone the repository
git clone https://github.com/ganmayou2333/avs.git

# Or download: Code → Download ZIP
```

Copy the desired skill folder into your agent's skills directory:

| Environment | Typical Path |
|-------------|-------------|
| Doubao / Super Doubao | `~/.super_doubao/super-doubao-runtime/workspace/.user_skills/` |
| GitHub Copilot | `~/.codex/skills/` |
| Claude / Other Agents | `~/.agents/skills/` |

```bash
cp -r arknights-design-style-guide /path/to/your/skills/directory/
```

Restart your agent session, then test:

> *"Design an Arknights-style operator profile UI"*

See each skill's `README.md` / `readme_cn.md` for detailed installation instructions (manual + AI prompt methods).

---

## Quick Reference — Core Design Tokens

| Element | Value |
|---------|-------|
| **Base background** | `#1A1C20` (dark charcoal — never pure black) |
| **Panel** | `#2B2D31` |
| **Primary brand** | `#3F72AF` (Rhodes Island blue, ≤15% of screen) |
| **Accent / success** | `#56B6C9` (Originium cyan) |
| **Warning** | `#E08E45` (dark orange) |
| **Danger** | `#B84A4A` (dark red) |
| **Border** | `#3F4349` — 1px solid |
| **Primary text** | `#FFFFFF` |
| **Secondary text** | `#C9CDD4` |
| **Tertiary text** | `#8A8F98` |
| **Primary font** | Source Han Sans (Heavy / Bold / Regular / Light) |
| **Data font** | JetBrains Mono (monospace for numbers) |
| **Card corners** | 45° chamfer — top-left + bottom-right diagonal |
| **Icon style** | Linear, 1.5px stroke |
| **UI motion** | 150–300ms, linear / ease-out — no elastic |
| **Poster grain** | 10–15% monochrome noise |
| **Poster vignette** | 10–20% edge darkening |
| **Animation shot length** | ≥2s (fast cuts ≤10% of total) |
| **Animation camera** | 40% static, 25% slow push-in |

---

## Design Philosophy

> **Imagine you are a military documentary cameraman on the battlefield of Terra.** You do not embellish, you do not sensationalize — you record calmly. Occasionally, a moment takes your breath away.

| Principle | Description |
|-----------|-------------|
| **Restraint** | Low-saturation dark base, only 1–2 accent colors, never flashy |
| **Coldness** | Cool gray tones, hard geometry, no soft rounded shapes |
| **Tactical terminal** | Every element looks like part of a Rhodes Island command terminal |
| **Post-apocalyptic** | Ruins, dust, aging textures, heavy atmosphere |
| **Function first** | If an element serves no information purpose, remove it |
| **Documentary realism** | Film grain, natural lighting, imperfect composition |

---

## Repository Structure

```
avs/
├── README.md                              # This index (English)
├── LICENSE                                # MIT License
├── arknights-design-style-guide/          # Full specification skill
│   ├── SKILL.md                           # Main entry: frontmatter + workflow + quick ref
│   ├── README.md                          # English docs + installation guide
│   ├── readme_cn.md                       # 中文文档 + 安装教程
│   └── references/
│       ├── ui-style.md                    # UI spec (12 chapters, ~690 lines)
│       ├── poster-style.md                # Poster spec (12 chapters, ~620 lines)
│       └── animation-style.md             # Animation spec (12 chapters, ~700 lines)
└── arknights-visual-style/                # Concise reference skill
    ├── SKILL.md                           # Main entry with style overview
    └── references/
        ├── ui-style.md                    # UI quick reference
        ├── poster-style.md                # Poster quick reference
        └── animation-style.md             # Animation quick reference
```

---

## Demo Showcase

A live interactive demo built with these design specifications:

**Rhodes Island Terminal — Combat Performance Dashboard**
- Full Arknights-style admin dashboard with sidebar, KPI cards, ECharts visualizations, sortable operator table, and detail modals
- 45° chamfer corners, dark charcoal base, Rhodes Island blue accents, film grain texture
- Zero rounded corners, no glass-morphism, no neon glow

---

## Contributing

Contributions are welcome — submit a pull request or open an issue.

When contributing:
- All parameters must be quantified (use hex codes, not "dark color")
- New content follows the existing 12-chapter structure
- Taboo lists are updated when new forbidden patterns are identified

---

## License

This project is licensed under the **MIT License** — see [LICENSE](LICENSE) for details.

---

## Copyright Notice

Arknights (明日方舟) is a trademark of **Hypergryph Network Technology Co., Ltd.** and **Yostar Limited**. These skills are unofficial, fan-created style guides and are **not affiliated with, endorsed by, or sponsored by** the game's developers or publishers.

All game-related names, characters, and visual elements remain the property of their respective copyright holders. The MIT License applies only to the original content of these skills (documentation, specifications, and code), not to any third-party intellectual property referenced within.
