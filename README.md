# Arknights Design Style Guide

A comprehensive AI Agent Skill that provides detailed visual design specifications for creating or evaluating content in the official art style of *Arknights* (明日方舟), covering three major categories: **UI Interface**, **Poster/Key Art**, and **Animation/Motion Design**.

---

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Skill Structure](#skill-structure)
- [Installation](#installation)
  - [Method 1: Manual Installation](#method-1-manual-installation)
  - [Method 2: AI Prompt Installation](#method-2-ai-prompt-installation)
- [Usage](#usage)
- [Design Philosophy](#design-philosophy)
- [Quick Reference](#quick-reference)
- [Contributing](#contributing)
- [License](#license)
- [Disclaimer](#disclaimer)

---

## Overview

This Skill transforms a general-purpose AI agent into an Arknights-style design specialist. It contains quantified, directly applicable parameters — color hex codes, font weights, spacing scales, animation durations, opacity values — so that generated UI, posters, and animations consistently achieve the recognizable "Arknights feel": restrained, cold, tactical-terminal aesthetic with a post-apocalyptic narrative tone.

Whether you are generating a game UI mockup, a character key visual, an IP collaboration poster, a PV storyboard, or a Live2D motion spec, this Skill provides a complete execution standard.

## Features

### Three Complete Style Manuals

| Category | Reference File | Coverage |
|----------|---------------|----------|
| **UI Interface** | `references/ui-style.md` | 12 chapters: color system, typography, layout grid, components, icons, textures, motion, screen recipes, interaction feedback, data visualization, taboos |
| **Poster / Key Art** | `references/poster-style.md` | 12 chapters: composition, color, lighting, character design, background, typography, grain/aging, IP collaboration, recipes, dimensions, taboos |
| **Animation / Motion** | `references/animation-style.md` | 12 chapters: rhythm & editing, camera language, character animation, VFX, UI transitions, skill performances, sound design, Live2D, recipes, tech specs, taboos |

### Quantified Parameters

Every specification includes concrete values:
- Exact hex color codes (`#1A1C20`, `#3F72AF`, `#56B6C9`, etc.)
- Font weights and letter-spacing values
- Spacing scales (4px base unit)
- Animation durations and easing functions
- Opacity percentages for textures and overlays
- Component dimensions and corner-cut sizes

### Universal Taboo Checklists

Each reference file ends with a detailed taboo list to prevent common style violations (e.g., rounded corners, rainbow gradients, elastic motion, chibi expressions).

## Skill Structure

```
arknights-design-style-guide/
├── SKILL.md                          # Main entry: frontmatter + workflow + quick reference
├── README.md                         # English documentation (this file)
├── readme_cn.md                      # Chinese documentation with installation tutorials
└── references/
    ├── ui-style.md                   # Complete UI design specification
    ├── poster-style.md               # Complete poster/key art specification
    └── animation-style.md            # Complete animation/motion specification
```

## Installation

### Method 1: Manual Installation

1. **Download or clone** this skill folder to your local machine.

2. **Locate your Agent's skills directory.** The exact path depends on your runtime environment. Common locations include:
   - `~/.super_doubao/super-doubao-runtime/workspace/.user_skills/`
   - `~/.codex/skills/`
   - `~/.agents/skills/`
   - Any directory configured as a skill root in your AI agent environment.

3. **Copy the entire `arknights-design-style-guide/` folder** into the skills directory:
   ```bash
   cp -r arknights-design-style-guide /path/to/your/skills/directory/
   ```

4. **Verify the structure.** Ensure the folder contains `SKILL.md` at its root and the `references/` subdirectory with all three markdown files.

5. **Restart or reload** your AI agent session so it rescans the skills directory.

6. **Test it.** Ask the agent something like: *"Design an Arknights-style operator profile UI"* or *"Create a poster in the Arknights art style"* — the agent should automatically load this Skill and follow its specifications.

### Method 2: AI Prompt Installation

If your AI agent supports skill creation via natural language, you can install this Skill by pasting the following prompt:

```
Create a new Skill named "arknights-design-style-guide" in your user skills directory. This Skill provides comprehensive visual design specifications for the Arknights (明日方舟) art style across three categories: UI interface, poster/key art, and animation/motion design.

The Skill must contain:
1. A SKILL.md with YAML frontmatter (name + description) that triggers when users request Arknights-style UI, posters, animations, or mention "舟味", "鹰角风格", "方舟美术", or "Arknights style".
2. A references/ui-style.md with detailed specs for: color system (dark charcoal #1A1C20 base, Rhodes Island blue #3F72AF), typography (Source Han Sans, Heavy/Normal/Light weights), 45° chamfered cards, 1px borders, linear icons, motion specs (150-300ms, no elastic easing), and a taboo list.
3. A references/poster-style.md with detailed specs for: documentary tactical poster composition (55-70% character ratio), three-layer depth, monochromatic color harmony, 10-15% film grain, vignette, IP collaboration rules, and a taboo list.
4. A references/animation-style.md with detailed specs for: slow pacing (shots ≥2 seconds), static/slow-push camera, three-phase combat animation (charge-hold-follow), cold-color VFX with physical smoke, fade-to-black transitions, sound design, Live2D parameters, and a taboo list.

Write all content in Chinese. Include quantified parameters (hex colors, px values, durations, opacity) throughout.
```

The agent will generate the complete Skill folder structure and files automatically. After generation, verify that all files exist and contain the expected content.

> **Note:** Prompt-based installation depends on your agent's skill-creation capability. For best results, use manual installation (Method 1) to ensure all content is exactly as specified.

## Usage

Once installed, the Skill activates automatically when the user's request matches its trigger description. The agent will:

1. **Identify the category** — UI, poster, or animation (compound tasks load multiple references).
2. **Load the corresponding reference file(s)** — following the progressive disclosure principle, only relevant references are loaded.
3. **Apply quantified parameters** — directly using hex colors, font specs, spacing, and timing values.
4. **Self-check against taboos** — verifying no forbidden elements (rounded corners, rainbow gradients, elastic motion, etc.) are present.

### Example Triggers

- *"Design an Arknights-style main menu UI"*
- *"Make a collaboration poster between Arknights and Battlefield"*
- *"Create a PV storyboard for a new operator, Arknights style"*
- *"Give this app interface an Arknights look"*
- *"What are the color specs for Arknights UI?"*
- *"舟味海报怎么设计？"*

## Design Philosophy

The core metaphor behind all Arknights visual design: **imagine you are a military documentary cameraman on the battlefield of Terra.** You do not embellish, you do not sensationalize — you record calmly. Occasionally, a moment takes your breath away.

This translates into six universal principles:

1. **Restraint** — Low-saturation dark base, only 1–2 accent colors, never flashy
2. **Coldness** — Cool gray tones, hard geometry, no soft rounded shapes
3. **Tactical terminal feel** — Every element looks like part of a Rhodes Island command terminal
4. **Post-apocalyptic narrative** — Ruins, dust, aging textures, heavy atmosphere
5. **Function over decoration** — If an element serves no information purpose, remove it
6. **Documentary realism** — Film grain, natural lighting, imperfect composition

## Quick Reference

| Element | Specification |
|---------|--------------|
| Base background | `#1A1C20` (dark charcoal, never pure black) |
| Primary brand color | `#3F72AF` (Rhodes Island blue, ≤15% of screen) |
| Success/benefit color | `#56B6C9` (fluorescent cyan) |
| Warning color | `#E08E45` (dark orange) |
| Danger color | `#B84A4A` (dark red) |
| Primary font | Source Han Sans (Heavy / Normal / Light) |
| Card corners | 45° chamfer (top-left + bottom-right diagonal) |
| Border width | 1px solid, `#3F4349` |
| Icon style | Linear, 1.5px stroke |
| UI motion | 150–300ms, linear/ease-out, no elastic |
| Poster grain | 10–15% opacity monochrome noise |
| Poster vignette | 10–20% edge darkening |
| Animation shot length | ≥2 seconds (fast cuts ≤10% of total) |
| Animation camera | 40% static, 25% slow push-in |
| Combat animation | Charge → 1–2 frame hold → follow-through |

## Contributing

Contributions are welcome. If you find inaccuracies, want to add new screen recipes, or expand the animation specifications, please submit a pull request or open an issue.

When contributing, ensure:
- All parameters are quantified (no vague descriptions like "dark color" — use hex codes)
- New content follows the existing chapter structure
- Taboo lists are updated when new forbidden patterns are identified

## License

This Skill is provided for educational and creative reference purposes. Arknights (明日方舟) is a trademark of Hypergryph / Yostar. This is an unofficial fan-created style guide and is not affiliated with or endorsed by the game's developers or publishers.

## Disclaimer

This is an unofficial, fan-created style guide. All visual specifications are derived from public observation of the game's art style and are intended as a creative reference. Official brand assets, logos, and character designs remain the property of their respective copyright holders.
