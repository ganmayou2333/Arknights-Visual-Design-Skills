# 明日方舟视觉设计技能库（Arknights Visual Design Skills）

一套 AI Agent 技能（Skills）集合，用于生成或评估符合《明日方舟》官方美术调性的视觉内容。

> **English version**：[README.md](README.md)

---

## 仓库内技能

本仓库包含**两套深度不同的技能**，均覆盖三大品类：**UI 界面**、**海报/主视觉**、**动画/动态设计**。

| 技能 | 定位 | 内容 | 适用场景 |
|------|------|------|---------|
| [arknights-design-style-guide](arknights-design-style-guide/) | 完整版 · 严谨执行 | 三品类各 12 章完整规范，全量化参数 + 详细禁忌清单 | 需要精确落地的复杂任务：多界面系统、主视觉 KV、PV 分镜、联名宣传 |
| [arknights-visual-style](arknights-visual-style/) | 精简版 · 快速套用 | 三品类要点速查 + 核心禁忌 | 快速生成、轻量集成、简单改稿 |

> **选择建议**：追求细节完整、可对照执行的规范 → 用 `arknights-design-style-guide`；只需要快速得到"舟味"正确的产出 → 用 `arknights-visual-style`。两者也可并存，复合任务时互相补充。

### 1. arknights-design-style-guide（完整版设计风格指南）

覆盖三大品类的完整视觉设计规范：**UI 界面**、**海报/主视觉**、**动画/动态设计**。每个品类均有一份完整的 12 章参考手册，包含量化参数（十六进制色值、字重、间距、动画时长、透明度）与详细禁忌清单。

| 文件 | 说明 |
|------|------|
| [SKILL.md](arknights-design-style-guide/SKILL.md) | 主入口：YAML 元数据 + 工作流程 + 快速参考 |
| [README.md](arknights-design-style-guide/README.md) | 英文文档，含安装教程 |
| [readme_cn.md](arknights-design-style-guide/readme_cn.md) | 中文文档，含详细安装教程 |
| [references/ui-style.md](arknights-design-style-guide/references/ui-style.md) | UI 设计完整规范（12 章） |
| [references/poster-style.md](arknights-design-style-guide/references/poster-style.md) | 海报/主视觉完整规范（12 章） |
| [references/animation-style.md](arknights-design-style-guide/references/animation-style.md) | 动画/动态设计完整规范（12 章） |

### 2. arknights-visual-style（精简版风格参考）

面向明日方舟 UI、海报、动画设计的精简风格参考，适合快速查阅与轻量集成。

| 文件 | 说明 |
|------|------|
| [SKILL.md](arknights-visual-style/SKILL.md) | 主入口，含风格总览 |
| [README.md](arknights-visual-style/README.md) | 英文文档，含安装教程 |
| [readme_cn.md](arknights-visual-style/readme_cn.md) | 中文文档，含安装教程 |
| [references/ui-style.md](arknights-visual-style/references/ui-style.md) | UI 风格参考 |
| [references/poster-style.md](arknights-visual-style/references/poster-style.md) | 海报风格参考 |
| [references/animation-style.md](arknights-visual-style/references/animation-style.md) | 动画风格参考 |

---

## 仓库结构

```
Arknights-Visual-Design-Skills/
├── README.md                        # 本索引（英文）
├── readme_cn.md                     # 本索引（中文）
├── LICENSE                          # MIT 许可证
├── arknights-design-style-guide/    # 完整版技能
│   ├── SKILL.md                     # 主入口：YAML 元数据 + 工作流程 + 快速参考
│   ├── README.md                    # 英文文档，含安装教程
│   ├── readme_cn.md                 # 中文文档，含详细安装教程
│   ├── LICENSE                      # MIT 许可证
│   └── references/
│       ├── ui-style.md              # UI 设计完整规范（12 章）
│       ├── poster-style.md          # 海报/主视觉完整规范（12 章）
│       └── animation-style.md       # 动画/动态设计完整规范（12 章）
└── arknights-visual-style/          # 精简版技能
    ├── SKILL.md                     # 主入口，含风格总览
    ├── README.md                    # 英文文档，含安装教程
    ├── readme_cn.md                 # 中文文档，含安装教程
    ├── LICENSE                      # MIT 许可证
    └── references/
        ├── ui-style.md              # UI 风格参考
        ├── poster-style.md          # 海报风格参考
        └── animation-style.md       # 动画风格参考
```

---

## 快速开始

1. 克隆本仓库：
   ```bash
   git clone https://github.com/ganmayou2333/Arknights-Visual-Design-Skills.git
   ```
   或在仓库页面点击 **Code → Download ZIP** 下载并解压到本地。

2. 将所需的技能文件夹（如 `arknights-design-style-guide/`）复制到你的 Agent 技能目录。

3. 重启 Agent 会话。

4. 用类似指令测试：*"帮我设计一个明日方舟风格的干员档案界面"*

各技能的 `README.md` / `readme_cn.md` 内含详细安装教程（手动安装与 AI 提示词安装两种方式）。

---

## 设计哲学

所有明日方舟视觉设计的核心比喻：**想象你是一名随军纪录片摄影师，在泰拉大陆的战场上记录一切。** 你不修饰、不煽情，只是冷静地拍摄。偶尔，一个瞬间让你屏住呼吸。

| 原则 | 说明 |
|------|------|
| 克制 | 低饱和暗基底，仅 1–2 处点睛色 |
| 冷峻 | 冷灰色调、硬朗几何、无柔软圆角 |
| 战术终端感 | 每个元素都像罗德岛指挥终端的一部分 |
| 末世叙事感 | 废墟、沙尘、做旧纹理、沉重氛围 |
| 功能优先 | 元素无信息功能则删除 |
| 纪实写实感 | 胶片颗粒、自然光影、不完美构图 |

---

## 许可证

本项目采用 MIT 许可证，详见 [LICENSE](LICENSE) 文件。

## 版权声明

明日方舟（Arknights）是鹰角网络科技有限公司及 Yostar Limited 的商标。本项目为非官方粉丝创作的风格指南，与游戏开发商或发行商无隶属关系，也未获其认可或赞助。

所有游戏相关名称、角色及视觉元素的版权归各自所有者所有。MIT 许可证仅适用于本项目的原创内容（文档、规范和代码），不适用于其中引用的任何第三方知识产权。
