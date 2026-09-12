# Arknights Visual Style

A concise AI Agent Skill for creating or evaluating content in the official art style of *Arknights* (明日方舟), covering three categories: **UI Interface**, **Poster/Key Art**, and **Animation/Motion Design**.

> Looking for the full specification? See [arknights-design-style-guide](../arknights-design-style-guide/README.md) — a comprehensive 12-chapter manual per category with quantified parameters and detailed taboo checklists.

---

## Table of Contents

- [Overview](#overview)
- [Skill Structure](#skill-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Design Philosophy](#design-philosophy)
- [Quick Reference](#quick-reference)
- [License](#license)
- [Copyright Notice](#copyright-notice)
- [Disclaimer](#disclaimer)

---

## Overview

This Skill provides a compact, directly applicable visual specification for the recognizable "Arknights feel": restrained, cold, tactical-terminal aesthetic with a post-apocalyptic narrative tone. It is designed for quick lookups and lightweight integration — you get the essential parameters without loading a full manual.

## Skill Structure

```
arknights-visual-style/
├── SKILL.md                          # Main entry: frontmatter + workflow + quick reference
├── README.md                         # English documentation (this file)
├── readme_cn.md                      # Chinese documentation with installation tutorial
├── LICENSE                           # MIT License
└── references/
    ├── ui-style.md                   # UI style reference (colors, typography, components, motion)
    ├── poster-style.md               # Poster style reference (composition, color, lighting, text)
    └── animation-style.md            # Animation style reference (rhythm, camera, VFX, transitions)
```

## Installation

### Method 1: Manual Installation

1. **Download or clone** the repository:
   ```bash
   git clone https://github.com/ganmayou2333/Arknights-Visual-Design-Skills.git
   ```

2. **Locate your Agent's skills directory.** Common locations include:
   - `~/.super_doubao/super-doubao-runtime/workspace/.user_skills/`
   - `~/.codex/skills/`
   - `~/.agents/skills/`
   - Any directory configured as a skill root in your AI agent environment.

3. **Copy the entire `arknights-visual-style/` folder** into the skills directory:
   ```bash
   cp -r arknights-visual-style /path/to/your/skills/directory/
   ```

4. **Restart or reload** your AI agent session so it rescans the skills directory.

5. **Test it.** Ask the agent something like: *"Design an Arknights-style operator profile UI"* — the agent should automatically load this Skill and follow its specifications.

### Method 2: AI Prompt Installation

If your AI agent supports skill creation via natural language, paste the following prompt:

```
Create a new Skill named "arknights-visual-style" in your user skills directory. This Skill provides a concise visual style reference for Arknights (明日方舟) across three categories: UI interface, poster/key art, and animation/motion design.

The Skill must contain:
1. A SKILL.md with YAML frontmatter (name + description) that triggers when users request Arknights-style UI, posters, animations, or mention "舟味", "舟游风格", "鹰角风格", "方舟美术".
2. A references/ui-style.md with concise specs for: color system (dark charcoal #1A1C20 base, Rhodes Island blue #3F72AF, semantic colors #56B6C9/#E08E45/#B84A4A), typography (Source Han Sans, Heavy/Normal/Light), 45° chamfered cards, 1px borders (#3F4349), linear icons (1.5px), motion (150-300ms, no elastic easing), typical screens, and a taboo list.
3. A references/poster-style.md with concise specs for: documentary tactical poster composition (60-70% character ratio), three-layer depth, unified color tone, 10-15% film grain, vignette (10-20%), accent color ≤5%, IP collaboration rules (6:4 visual weight), and a taboo list.
4. A references/animation-style.md with concise specs for: slow pacing (shots ≥2 seconds, fast cuts ≤10%), static/slow-push camera, charge-hold-follow combat animation, cold-color VFX with physical smoke, black-fade/scanline/glitch transitions, restrained sound design, and a taboo list.

Write all content in Chinese. Include quantified parameters (hex colors, px values, durations, opacity) throughout.
```

> **Note:** Prompt-based installation depends on your agent's skill-creation capability. For best results, use manual installation (Method 1) to ensure all content is exactly as specified.

## Usage

Once installed, the Skill activates automatically when the user's request matches its trigger description. The agent will:

1. **Identify the category** — UI, poster, or animation (compound tasks load multiple references).
2. **Load the corresponding reference file(s)** — following the progressive disclosure principle, only relevant references are loaded.
3. **Apply quantified parameters** — directly using hex colors, font specs, spacing, and timing values.
4. **Self-check against taboos** — verifying no forbidden elements (rounded corners, rainbow gradients, elastic motion, chibi expressions) are present.

### Example Triggers

- *"Design an Arknights-style main menu UI"*
- *"Make a collaboration poster between Arknights and Battlefield"*
- *"Create a PV storyboard for a new operator, Arknights style"*
- *"Give this app interface an Arknights look"*
- *"舟味海报怎么设计？"*

## Design Philosophy

The core metaphor behind all Arknights visual design: **imagine you are a military documentary cameraman on the battlefield of Terra.** You do not embellish, you do not sensationalize — you record calmly. Occasionally, a moment takes your breath away.

1. **Restraint** — Low-saturation dark base, only 1–2 accent colors, never flashy
2. **Coldness** — Cool gray tones, hard geometry, no soft rounded shapes
3. **Tactical terminal feel** — Every element looks like part of a Rhodes Island command terminal
4. **Post-apocalyptic narrative** — Ruins, dust, aging textures, heavy atmosphere
5. **Function over decoration** — If an element serves no information purpose, remove it

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
| Combat animation | Charge → 1–2 frame hold → follow-through |

## License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

## Copyright Notice

Arknights (明日方舟) is a trademark of Hypergryph Network Technology Co., Ltd. and Yostar Limited. This project is an unofficial, fan-created style guide and is not affiliated with, endorsed by, or sponsored by the game's developers or publishers.

All game-related names, characters, and visual elements remain the property of their respective copyright holders. The MIT License applies only to the original content of this Skill (documentation, specifications, and code), not to any third-party intellectual property referenced within.

## Disclaimer

This is an unofficial, fan-created style guide. All visual specifications are derived from public observation of the game's art style and are intended as a creative reference. Official brand assets, logos, and character designs remain the property of their respective copyright holders.
