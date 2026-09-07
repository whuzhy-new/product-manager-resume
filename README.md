# 产品经理简历 Skill

面向中文产品经理求职的 AI Skill：从真实项目材料中提炼能力故事，整理简历母版，并按具体岗位 JD 生成定向版本。

适用于 C 端、B 端 / SaaS、平台 / 基建、策略增长和 AI / Agent 产品方向。

## 能做什么

- **创建或重构简历母版**：梳理事实证据，确定能力主线，选择和组织项目。
- **维护已有简历**：增补新事实，持续维护同一套证据库和母版。
- **匹配具体 JD**：区分强证据、表达不足、待确认经历和真实缺口，只使用已确认事实生成定向版本。
- **审阅简历**：检查事实、个人职责、因果关系、语言和岗位匹配。

## 核心方法

按“事实证据 → 能力故事 → 项目取舍 → 简历表达”推进：

1. 建立证据库，标记已确认、待确认和缺失信息。
2. 选择目标方向，为每个保留项目确定一个主要能力故事。
3. 补齐业务背景、关键判断、本人动作、职责边界和验证结果。
4. 生成简历母版，再根据 JD 重排和改写已确认内容。
5. 检查事实依据、表达质量与岗位适配。

不编造指标，不把团队成果直接归为个人成果，不把“参与”升级为“主导”。缺少业务指标时，使用已有的交付、评测或用户反馈等可验证证据。

## 使用方式

将本仓库完整目录放到支持 `SKILL.md` 的工具所使用的 Skill 目录中，目录名保留为 `product-manager-resume`。入口为 [SKILL.md](SKILL.md)，引用文件需随目录一起保留。

在已加载该 Skill 的会话中，可以这样提出需求：

**创建母版**

```text
使用 $product-manager-resume，根据我提供的简历和项目复盘梳理事实证据，
生成面向 AI 产品经理岗位的简历母版。先读完材料，再追问缺失信息。
```

**按 JD 定向优化**

```text
使用 $product-manager-resume，基于现有简历母版和证据库，
按这份 JD 生成定向版本，并说明哪些能力已有证据、哪些存在缺口。
```

**只做审阅**

```text
使用 $product-manager-resume，审阅这份产品经理简历，
重点检查职责边界、项目取舍和语言表达，先给出问题与修改建议，不直接改文件。
```

建议提供现有简历、目标方向或 JD，以及可用于证明项目经历的 PRD、复盘、答辩材料或作品集。仅提供有权使用的材料，并提前处理敏感信息。

## 输出文件

要求维护文件时，使用同一套连续资产；只要求对话输出时，不自动创建文件。

```text
resume-workspace/
├── evidence-ledger.md       # 事实与证据库
├── ability-story-map.md     # 能力故事与项目取舍
├── resume-master.md         # 简历母版
└── targeted/
    └── company-role.md      # 岗位定向版本
```

## 仓库结构

```text
product-manager-resume/
├── SKILL.md                # 工作流程与使用规则
├── agents/openai.yaml      # 展示名称与默认提示词
├── references/             # 证据模型、岗位方向、语言规范与质量检查
├── templates/              # 证据库、故事地图和简历母版模板
└── examples/               # 改写对照与缺少指标时的表达示例
```

- [证据模型](references/evidence-model.md)
- [岗位方向](references/pm-archetypes.md) · [策略产品专项](references/strategy-pm.md) · [AI 产品专项](references/ai-pm.md)
- [项目取舍](references/story-selection.md)
- [写作规则](references/writing-rules.md) · [语言风格](references/language-style.md)
- [质量检查](references/quality-rubric.md)
- [弱表达与强表达对照](examples/weak-vs-strong-bullets.md) · [指标替代证据](examples/metric-alternatives.md)
- [小红书研究笔记](references/xiaohongshu-research.md)：收录 50 篇帖子的逐帖提炼、适用条件和风险边界；个体经验不代表招聘方官方规则。

## 适用边界

本 Skill 用于中文产品经理简历的事实整理与表达优化，不用于学术 CV，也不保证求职结果。岗位定向版本只能取舍和重写已确认事实；关键事实存在冲突时，应先核实再成稿。
