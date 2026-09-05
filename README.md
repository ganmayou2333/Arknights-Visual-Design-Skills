# Arknights Visual Design Skills

A collection of AI Agent Skills for creating and evaluating content in the official art style of *Arknights* (明日方舟).

---

## Skills in This Repository

### 1. arknights-design-style-guide

Comprehensive visual design specification covering three categories: **UI Interface**, **Poster/Key Art**, and **Animation/Motion Design**. Each category has a complete 12-chapter reference manual with quantified parameters (hex colors, font weights, spacing scales, animation durations, opacity values) and detailed taboo checklists.

| File | Description |
|------|-------------|
| [SKILL.md](arknights-design-style-guide/SKILL.md) | Main entry: YAML frontmatter, workflow, quick reference |
| [README.md](arknights-design-style-guide/README.md) | English documentation with installation guide |
| [readme_cn.md](arknights-design-style-guide/readme_cn.md) | 中文文档，含详细安装教程 |
| [references/ui-style.md](arknights-design-style-guide/references/ui-style.md) | Complete UI design specification (12 chapters) |
| [references/poster-style.md](arknights-design-style-guide/references/poster-style.md) | Complete poster/key art specification (12 chapters) |
| [references/animation-style.md](arknights-design-style-guide/references/animation-style.md) | Complete animation/motion specification (12 chapters) |

### 2. arknights-visual-style

A concise visual style reference for Arknights UI, poster, and animation design. Suitable for quick lookups and lighter-weight integration.

| File | Description |
|------|-------------|
| [SKILL.md](arknights-visual-style/SKILL.md) | Main entry with style overview |
| [references/ui-style.md](arknights-visual-style/references/ui-style.md) | UI style reference |
| [references/poster-style.md](arknights-visual-style/references/poster-style.md) | Poster style reference |
| [references/animation-style.md](arknights-visual-style/references/animation-style.md) | Animation style reference |

---

## Quick Start

1. Clone this repository:
   ```bash
   git clone https://github.com/ganmayou2333/avs.git
   ```
2. Copy the desired skill folder into your agent's skills directory.
3. Restart your agent session.
4. Test with a prompt like: *"Design an Arknights-style operator profile UI"*

See each skill's `README.md` / `readme_cn.md` for detailed installation instructions (manual installation and AI prompt installation methods).

---

## Design Philosophy

The core metaphor behind all Arknights visual design: **imagine you are a military documentary cameraman on the battlefield of Terra.** You do not embellish, you do not sensationalize — you record calmly. Occasionally, a moment takes your breath away.

| Principle | Description |
|-----------|-------------|
| Restraint | Low-saturation dark base, only 1–2 accent colors |
| Coldness | Cool gray tones, hard geometry, no soft rounded shapes |
| Tactical terminal | Every element looks like part of a Rhodes Island command terminal |
| Post-apocalyptic | Ruins, dust, aging textures, heavy atmosphere |
| Function first | If an element serves no information purpose, remove it |
| Documentary realism | Film grain, natural lighting, imperfect composition |

---

## License

MIT License — see [LICENSE](LICENSE) for details.

## Copyright Notice

Arknights (明日方舟) is a trademark of Hypergryph Network Technology Co., Ltd. and Yostar Limited. These skills are unofficial, fan-created style guides and are not affiliated with, endorsed by, or sponsored by the game's developers or publishers.

All game-related names, characters, and visual elements remain the property of their respective copyright holders. The MIT License applies only to the original content of these skills (documentation, specifications, and code), not to any third-party intellectual property referenced within.