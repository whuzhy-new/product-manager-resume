---
name: product-manager-resume
description: 当用户需要创建、重构、审阅或按 JD 定向优化中文产品经理简历，目标涉及 C 端、B 端、平台/基建、策略增长或 AI/Agent 产品方向时使用；不用于学术 CV 或脱离事实的包装。
---

# 产品经理简历

把用户材料整理成一条可信、清晰、适配目标岗位的产品能力主线。核心不是润色句子，而是完成“事实证据 → 能力故事 → 项目取舍 → 简历表达”。

## 先判断任务

- **创建或重构母版**：执行完整流程，产出证据库、能力故事地图和简历母版。
- **维护已有母版**：先读现有文件，只增补新事实并重新判断项目取舍，不新建语义重复的“补充区”。
- **匹配具体 JD**：以母版和证据库为唯一事实源，生成定向版本。
- **审阅简历**：按证据、主线、表达和岗位匹配逐项诊断；除非用户要求，不直接改文件。

## 工作原则

1. 先完整读取用户提供的简历、答辩、PRD、复盘、作品集和 JD，再提问；不要让用户重复已有信息。
2. 先确定求职阶段、目标方向和目标岗位。缺少关键信息时一次只问一个或一小组可直接回答的问题。
3. 逐项目核对业务背景、用户场景、关键判断、本人动作、职责边界、交付状态和验证结果。
4. 每个保留项目必须对应一个主要能力故事；项目之间应互补，而不是重复证明同一能力。
5. 明确区分“主导、负责、共同设计、参与、支持”。团队成果不能直接写成个人成果。
6. 不编数据，不估算用户没有确认的数字，也不要求每段经历必须有数字。缺少业务指标时使用可信的替代证据。
7. 不输出缺乏依据的百分制匹配分；使用证据覆盖矩阵说明强项、可挖项和真实缺口。
8. 技术词、方法论和公司黑话只有在解释产品判断时才保留。

需要追溯方法来源、比较常见写法或解释某条规则时，再读取 [references/xiaohongshu-research.md](references/xiaohongshu-research.md)。该文件包含 50 篇小红书帖的逐帖提炼、适用条件和风险边界；不要把帖子中的个体经验当作招聘方官方规则。

## 执行流程

### 1. 建立事实底座

创建或更新 `evidence-ledger.md`。详细字段和证据等级见 [references/evidence-model.md](references/evidence-model.md)，可复制 [templates/evidence-ledger.md](templates/evidence-ledger.md)。

标记所有信息：

- `✅ 已确认`：用户材料或用户回复直接支持。
- `⚠️ 待确认`：可能成立，但责任、数字、时间或因果仍需确认。
- `❌ 缺失`：岗位需要，但当前没有事实支持。

待确认和缺失内容不得进入投递版的陈述句。

### 2. 选择方向和故事

识别 C 端、B 端/SaaS、平台/基建、策略增长或 AI/Agent 路线。需要判断不同路线的证据重点时，读取 [references/pm-archetypes.md](references/pm-archetypes.md)。目标岗位或项目涉及推荐、广告、搜索、增长、定价、补贴、风控、供给分发、数据策略或实验平台时，必须读取 [references/strategy-pm.md](references/strategy-pm.md)。

建立 `ability-story-map.md`，按“岗位相关性、证据强度、候选人独特性、与其他项目的互补性”判断项目保留、压缩或删除。完整方法见 [references/story-selection.md](references/story-selection.md)，模板见 [templates/ability-story-map.md](templates/ability-story-map.md)。

如果存在两条都合理但取舍明显不同的主线，先给用户 2–3 个简短方案和各自代价，用户选择后再写母版。

### 3. 深挖高价值项目

按价值顺序逐个补齐证据，不要一次发出长问卷。优先追问：

- 为什么做，问题如何被发现；
- 服务谁、发生在哪个场景；
- 用户本人做了什么关键判断或方案；
- 有哪些约束、替代方案和取舍；
- 结果如何验证，哪些证据可公开。

证据已经足以支撑该能力故事时停止追问。

### 4. 生成母版

用 [references/writing-rules.md](references/writing-rules.md) 起草，并按 [templates/resume-master.md](templates/resume-master.md) 组织。涉及句子改写、语言压缩、责任动词、项目标签或不同岗位/资历的表达差异时，必须读取 [references/language-style.md](references/language-style.md)。默认输出 Markdown。

每个项目先确定一句内部能力结论，再用 2–4 条简历内容表达：业务问题与目标、关键判断与本人动作、交付与验证。不要机械套用固定句式。

### 5. 生成 JD 定向版

提取 JD 的硬性条件、高频职责、产品方向、关键能力和偏好证据，建立以下覆盖矩阵：

- 强证据覆盖；
- 已有证据但表达不足；
- 可能做过，需要追问；
- 真实缺失；
- 与岗位无关，应压缩或删除。

定向版只能重排、取舍和重写已确认事实，不能为了命中关键词添加用户没做过的经历。

定向版的语言重心也遵循 [references/language-style.md](references/language-style.md)：自然嵌入 JD 语义，不复制岗位描述，不升级责任动词。

### 6. 最终检查

交付前读取 [references/quality-rubric.md](references/quality-rubric.md)，检查事实、职责、因果、主线、证据、语言和 JD 匹配。发现关键事实冲突时暂停成稿并询问用户。

策略项目还要检查“业务目标 → 基线或异常 → 诊断假设 → 策略杠杆 → 实验灰度 → 结果归因”是否连贯；不能把团队 OKR、算法改动或远端业务结果直接写成个人成果。

## AI / Agent 产品专项

目标岗位或项目涉及 AI、Agent、Copilot、RAG、Workflow、Skill、Tool 或 MCP 时，必须读取 [references/ai-pm.md](references/ai-pm.md)。重点判断：

- 为什么该场景适合 AI，而不是普通功能；
- 场景和需求来自什么证据；
- 用户具体负责 Agent 产品链路的哪一段；
- Prompt、上下文、知识、工具调用、评测和失败案例如何影响方案；
- 项目体现应用场景能力，还是平台/基建能力；
- 技术细节是否真正说明产品判断与业务价值。

## 默认文件结构

用户要求维护文件或已经存在简历工作区时，使用同一套连续资产：

```text
resume-workspace/
├── evidence-ledger.md
├── ability-story-map.md
├── resume-master.md
└── targeted/
    └── company-role.md
```

如果用户只要求对话内输出，不擅自创建文件。

## 禁止事项

- 不把“参与”统一改成“主导”。
- 不把预计数据、行业均值或团队目标写成实际结果。
- 不用“赋能、打造、闭环、端到端”等词替代具体事实。
- 不把功能清单、技术名词或工作流程当作能力故事。
- 不为追求一页而删除支撑核心能力的唯一证据；先删低相关、重复和无法证明能力的内容。
- 不建立第二套母版、补充母版或其他语义重复的事实区。

需要改写示例时再读取 [examples/weak-vs-strong-bullets.md](examples/weak-vs-strong-bullets.md)；缺少直接指标时再读取 [examples/metric-alternatives.md](examples/metric-alternatives.md)。
