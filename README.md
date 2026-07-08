# XHS IP Cover System

> 基于个人 IP 角色的小红书封面生成系统 —— 不是单张美图，而是可复用的视觉体系。

## 这是什么

一套面向 AI 助手（如 Claude、Codex）的 **Skill / Prompt 系统**，用于围绕一个**固定的 IP 角色**，持续产出高一致性、高识别度的小红书封面。

核心思路：封面 = 内容意图 × IP 角色 × 结构模板 × 风格变体。

## 文件结构

```
├── SKILL.md                                    # 主入口：Skill 定义与工作流
├── agents/
│   └── openai.yaml                             # OpenAI Agents 配置
├── assets/
│   ├── cover-brief-template.md                 # 封面需求简报模板（可直接复制使用）
│   └── ip-character-card-template.md            # IP 角色卡模板
└── references/
    ├── cover-production-sop.md                 # 完整 SOP：从需求到归档的全流程
    ├── replace-with-your-ip.md                 # 如何把示例角色替换成你自己的 IP
    ├── style-variants.md                       # 四套风格变体及其选择规则
    ├── prompt-templates.md                     # 可复用的提示词模块
    ├── quality-checklist.md                    # 封面质量校验清单
    └── examples.md                             # 实战案例
```

## 核心工作流

1. **收集需求简报** → 明确内容类型、主标题、受众承诺
2. **选择角色模式** → 专业模式 / 吉祥物模式
3. **选择或适配风格变体** → Cream Companion / Black Efficiency / Utility Fieldwork / Street Sprint
4. **构建视觉结构** → 标题 + 角色 + 信息块 + 贴纸
5. **撰写生成提示词**
6. **先生成一张方向稿**
7. **质量检查** → 缩略图可读性 / 角色一致性 / 信息密度 / 系列化潜力
8. **迭代或归档**

详细步骤见 `references/cover-production-sop.md`。

## 快速开始

### 1. 定义你的 IP 角色

复制 `assets/ip-character-card-template.md`，填写你的角色信息：

- 外貌特征（发型、服装、配饰）
- 性格气质
- 标志性动作/表情
- 色彩偏好

### 2. 用简报启动一次封面

复制 `assets/cover-brief-template.md`，填入本次内容的需求字段：

```text
Content type: 教知识
Main title: 3个公式搞定选题
Topic: 内容创作方法论
Reader promise: 学完就能用
Character mode: 专业模式
Style variant: Black Efficiency
Aspect ratio: 3:4
```

### 3. 交给 AI 生成

将 `SKILL.md` 和已填写的简报一起发送给 AI 助手，即可获得结构化的封面提示词和生成结果。

## 角色模式

| 模式 | 适用场景 |
|---|---|
| **专业模式** | 方法讲解、工具教程、案例拆解、产品/课程推广 |
| **吉祥物模式** | 新手科普、资源推荐、轻量种草、栏目系列封面 |

## 风格变体

四套内置友好吉祥物风格：

- 🎨 **Cream Companion** — 温暖陪伴感，适合情感类、成长类
- ⚡ **Black Efficiency** — 高效专业感，适合干货类、工具类
- 🔧 **Utility Fieldwork** — 实操现场感，适合教程类、案例类
- 🏃 **Street Sprint** — 活力行动感，适合激励类、挑战类

完整选择规则见 `references/style-variants.md`。

## 使用要求

- AI 助手支持 Skill / 自定义指令加载（Claude Code、OpenAI Codex 等）
- 图像生成能力（DALL-E、Midjourney 或其他图像模型）

## License

本项目内容采用 [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) 许可协议。
