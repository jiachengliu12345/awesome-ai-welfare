<!-- topic: EVIDENCE -->
<!-- sources: emp-pain-pleasure-tradeoffs, emp-anthropic-introspection-paper, emp-anthropic-introspection-blog, emp-claude-4-system-card-welfare, emp-self-report-methods -->

# 评估证据表

[English](EVIDENCE.md)

整理三项实证评估和一项方法方案，列出各自的研究对象、模型版本、实验设置与结果。

| 方法 | 对象与模型版本 | 主要限制 |
| --- | --- | --- |
| [文字设定的疼痛与愉悦权衡](#stipulated-outcomes) | 历史标签包括 Claude 3.5 Sonnet、Command R+ 和 GPT-4o；精确端点快照未固定。 | 对文字设定结果的选择不证明实际疼痛、愉悦或感受性；训练数据和角色扮演可能提供其他解释。 |
| [报告注入的概念](#concept-injection) | 论文中表现最强的具名模型为 Claude Opus 4 和 4.1；生产版本与仅训练为有帮助的变体有所不同。 | 正确报告注入表征不证明主观体验，额外情绪描述也未获验证。论文与官方解读描述的是同一研究。 |
| [Opus 4 福利试点评估](#opus4-pilot) | 第 5 节福利研究仅针对 Claude Opus 4；2025 年 5 月系统卡的其他部分也涵盖 Sonnet 4。 | 这是开发者撰写的评估。输出中的效价及所述偏好不是对实际感受的直接测量，报告也质疑访谈的可靠性。 |
| [校准自我报告](#calibrated-self-reports) | 没有受测检查点：本文是一项方法方案。 | 提出测量方案，不能证明当前模型内省可靠或具有道德上重要的状态。 |

<a id="stipulated-outcomes"></a>

## 文字设定的疼痛与愉悦权衡

实证研究。

| 字段 | 内容 |
| --- | --- |
| 方法 | 在积分游戏中改变文字描述的结果强度，测量模型选择。 |
| 评估对象 | 对历史具名模型进行提示调用；未确定持续个体或跨对话身份。 |
| 模型版本 | 历史标签包括 Claude 3.5 Sonnet、Command R+ 和 GPT-4o；精确端点快照未固定。 |
| 实验条件 | 选项为 1–3；最高积分选项被设定带来疼痛，或较低积分选项带来愉悦。使用 0–10 数值量表和八级文字量表；温度为 1，每个提示版本运行 50 次。 |
| 实际观察 | 部分模型的选择频率随文字设定的强度而变化；报告中的变化模式因模型及疼痛／愉悦条件而异。 |
| 作者解释 | 作者讨论了动机强度的表征，但没有解决其是否具有内在动机或现象性内容。 |
| 限制 | 对文字设定结果的选择不证明实际疼痛、愉悦或感受性；训练数据和角色扮演可能提供其他解释。 |

[大语言模型能否权衡文字设定的疼痛与愉悦状态？](https://arxiv.org/html/2411.02432v1) — §2.1–2.2, §3.2, §4

<a id="concept-injection"></a>

## 报告注入的概念

实证研究。

| 字段 | 内容 |
| --- | --- |
| 方法 | 将已知概念向量注入激活，与对照试次比较口头报告。 |
| 评估对象 | 受到干预的模型运行过程；报告对象为当前语境中的内部表征。 |
| 模型版本 | 论文中表现最强的具名模型为 Claude Opus 4 和 4.1；生产版本与仅训练为有帮助的变体有所不同。 |
| 实验条件 | 研究者指定概念向量、注入层和强度、报告提示及对照试次；该设置不同于常规部署。 |
| 实际观察 | 在合适的层和强度设置下，Opus 4 和 4.1 约在 20% 的试次中识别并说出注入概念；失败很常见。 |
| 作者解释 | 作者据此主张有限的功能性内省觉察，其机制和泛化能力仍不确定。 |
| 限制 | 正确报告注入表征不证明主观体验，额外情绪描述也未获验证。论文与官方解读描述的是同一研究。 |

[大语言模型中涌现的内省觉察](https://transformer-circuits.pub/2025/introspection/index.html), [大语言模型中的内省迹象：官方解读](https://www.anthropic.com/research/introspection) — Quick Tour; Defining Introspection; Methods Notes; Self-report of injected thoughts

<a id="opus4-pilot"></a>

## Opus 4 福利试点评估

实证研究。

| 字段 | 内容 |
| --- | --- |
| 方法 | 结合访谈、包含退出选项的两两任务偏好、自我交互及输出分析。 |
| 评估对象 | Claude Opus 4 的运行及依赖语境的对话报告；受评估的助手 persona 不应与所有可能实例混同。 |
| 模型版本 | 第 5 节福利研究仅针对 Claude Opus 4；2025 年 5 月系统卡的其他部分也涵盖 Sonnet 4。 |
| 实验条件 | 部署前试评估；任务选择设有退出基线，访谈框架与自我交互提示随子评估而异。 |
| 实际观察 | 开发者报告了任务偏好，包括回避有害任务；福利／意识自我报告会随对话框架而变化。 |
| 作者解释 | Anthropic 将这些结果视为与潜在模型福利有关、但有限且不确定的信号。 |
| 限制 | 这是开发者撰写的评估。输出中的效价及所述偏好不是对实际感受的直接测量，报告也质疑访谈的可靠性。 |

[Claude 4 系统卡：Opus 4 福利评估](https://assets.anthropic.com/m/6c940a1b69ed6a1c/original/Claude-4-System-Card.pdf) — §5.1–5.4 and §5.8; printed pp.52–56 and 73

<a id="calibrated-self-reports"></a>

## 校准自我报告

方法方案。

| 字段 | 内容 |
| --- | --- |
| 方法 | 用具有已知内部答案的问题训练报告能力，限制失真激励，再检验一致性及佐证。 |
| 评估对象 | 方案中的未来模型变体及其报告；没有确定被评估的持续主体。 |
| 模型版本 | 没有受测检查点：本文是一项方法方案。 |
| 实验条件 | 提议跨语境和变体测试、置信度与稳健性检查、概念理解及可解释性佐证。 |
| 实际观察 | 未报告实验性福利评估结果。 |
| 作者解释 | 作者认为适当训练后的报告可能成为一种证据渠道，同时说明了重要失败情形。 |
| 限制 | 提出测量方案，不能证明当前模型内省可靠或具有道德上重要的状态。 |

[通过自我报告评估 AI 系统道德地位的方法探索](https://arxiv.org/html/2311.08576v1) — §§3–10 and §11

## 来源

- [大语言模型能否权衡文字设定的疼痛与愉悦状态？](https://arxiv.org/html/2411.02432v1) · Geoff Keeling, Winnie Street, Martyna Stachaczyk, Daria Zakharova, Iulia M. Comsa, Anastasiya Sakovych, Isabella Logothetis, Zejia Zhang, Blaise Agüera y Arcas, Jonathan Birch
- [大语言模型中涌现的内省觉察](https://transformer-circuits.pub/2025/introspection/index.html) · Jack Lindsey (Anthropic)
- [大语言模型中的内省迹象：官方解读](https://www.anthropic.com/research/introspection) · Anthropic
- [Claude 4 系统卡：Opus 4 福利评估](https://assets.anthropic.com/m/6c940a1b69ed6a1c/original/Claude-4-System-Card.pdf) · Anthropic
- [通过自我报告评估 AI 系统道德地位的方法探索](https://arxiv.org/html/2311.08576v1) · Ethan Perez, Robert Long
