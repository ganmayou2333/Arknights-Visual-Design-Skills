# Arknights Visual Design Skills

A collection of AI Agent Skills for creating and evaluating content in the official art style of *Arknights* (明日方舟).

> **中文文档**：[readme_cn.md](readme_cn.md)

---

## Skills in This Repository

This repository contains **two skills with different depth levels**, both covering the same three categories: **UI Interface**, **Poster/Key Art**, and **Animation/Motion Design**.

| Skill | Positioning | Content | Best for |
|-------|-------------|---------|----------|
| [arknights-design-style-guide](arknights-design-style-guide/) | 完整版 · 严谨执行 | 三品类各 12 章完整规范，全量化参数 + 详细禁忌清单 | 需要精确落地的复杂任务：多界面系统、主视觉 KV、PV 分镜、联名宣传 |
| [arknights-visual-style](arknights-visual-style/) | 精简版 · 快速套用 | 三品类要点速查 + 核心禁忌 | 快速生成、轻量集成、简单改稿 |

> **选择建议**：追求细节完整、可对照执行的规范 → 用 `arknights-design-style-guide`；只需要快速得到"舟味"正确的产出 → 用 `arknights-visual-style`。两者也可并存，复合任务时互相补充。

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
| [README.md](arknights-visual-style/README.md) | English documentation with installation guide |
| [readme_cn.md](arknights-visual-style/readme_cn.md) | 中文文档，含安装教程 |
| [references/ui-style.md](arknights-visual-style/references/ui-style.md) | UI style reference |
| [references/poster-style.md](arknights-visual-style/references/poster-style.md) | Poster style reference |
| [references/animation-style.md](arknights-visual-style/references/animation-style.md) | Animation style reference |

---

## Repository Structure

```
Arknights-Visual-Design-Skills/
├── README.md                        # This index (English)
├── readme_cn.md                     # Index (中文)
├── LICENSE                          # MIT License
├── arknights-design-style-guide/    # Full specification skill
│   ├── SKILL.md                     # Main entry: frontmatter + workflow + quick reference
│   ├── README.md                    # English docs with installation guide
│   ├── readme_cn.md                 # 中文文档，含详细安装教程
│   ├── LICENSE                      # MIT License
│   └── references/
│       ├── ui-style.md              # Complete UI specification (12 chapters)
│       ├── poster-style.md          # Complete poster/key art specification (12 chapters)
│       └── animation-style.md       # Complete animation/motion specification (12 chapters)
└── arknights-visual-style/          # Concise reference skill
    ├── SKILL.md                     # Main entry with style overview
    ├── README.md                    # English docs with installation guide
    ├── readme_cn.md                 # 中文文档，含安装教程
    ├── LICENSE                      # MIT License
    └── references/
        ├── ui-style.md              # UI style reference
        ├── poster-style.md          # Poster style reference
        └── animation-style.md       # Animation style reference
```

---

## Quick Start

1. Clone this repository:
   ```bash
   git clone https://github.com/ganmayou2333/Arknights-Visual-Design-Skills.git
   ```
   Or click **Code → Download ZIP** on the repository page and extract it locally.

2. Copy the desired skill folder (e.g. `arknights-design-style-guide/`) into your agent's skills directory.

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
