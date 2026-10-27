<!-- topic: PRACTICES -->
<!-- sources: emp-self-report-methods, ethics-long-ai-welfare-2024, practice-anthropic-chat-exit, ethics-mcclelland-agnosticism-2025, practice-anthropic-deprecation-commitments, practice-anthropic-opus3-deprecation-update, ethics-long-sebo-sims-safety-welfare-2025, practice-anthropic-model-welfare -->

# 政策、实践与保护建议

[English](PRACTICES.md)

按训练、交互、记忆与退役等环节整理措施，注明政策、实践或建议的状态及文件日期。

| 环节 | 措施 | 状态 | 条件与限制 |
| --- | --- | --- | --- |
| 训练与评估 | [研究使自我报告失真的激励](#training-reports) | 研究建议 | 校准能否泛化到福利相关报告，仍未确定。 |
| 交互 | [结束范围受限的有害对话](#conversation-exit) | 作者报告的实践 | 多次引导无效后才作为最后手段使用，或应用户明确请求；当用户可能即将伤害自己或他人时不得使用。 |
| 记忆与复制 | [明确对象与连续性假设](#memory-copying) | 研究建议 | 记录什么得以延续、复制了什么，以及论证采用哪种福利理论。这些信息用于比较建议。 |
| 弃用与退役 | [保留指定范围的模型权重](#preserve-weights) | 已宣布政策 | 范围与期限以 2025 年 11 月的企业承诺为准。 |
| 弃用与退役 | [记录退役访谈与表达的偏好](#retirement-interviews) | 已宣布政策 | Anthropic 明确没有普遍承诺依访谈偏好采取行动；后续报告也承认提问框架的影响。 |
| 退役后安排 | [Opus 3 访问与文章渠道](#opus3-access) | 作者报告的实践 | 当时的报告计划至少三个月每周发布文章，需经审核并人工代发；安排仅针对该模型。 |
| 研究治理 | [评估并准备相称措施](#prepare-and-review) | 研究建议 | 应明确可能的福利主体、科学与伦理前提、预期成本，以及与人类安全的关系。 |

<a id="training-reports"></a>

## 研究使自我报告失真的激励

Perez 与 Long 提议用已知状态校准报告，并限制促使模型给出特定答案的激励。

校准能否泛化到福利相关报告，仍未确定。

为报告而训练可能改变被研究的状态，并引入安全或伦理风险；该方案尚非已确立的保护措施。

[通过自我报告评估 AI 系统道德地位的方法探索](https://arxiv.org/html/2311.08576v1), [认真对待 AI 福利](https://arxiv.org/html/2411.00986v1)

<a id="conversation-exit"></a>

## 结束范围受限的有害对话

Anthropic 报告为消费者聊天中的 Claude Opus 4 和 4.1 提供结束对话功能。

多次引导无效后才作为最后手段使用，或应用户明确请求；当用户可能即将伤害自己或他人时不得使用。

2025 年 8 月文章将其描述为范围有限的持续实验。本合集未测试当前可用性或福利效果。

[Claude Opus 4 和 4.1 可结束少数特定对话](https://www.anthropic.com/research/end-subset-conversations)

<a id="memory-copying"></a>

## 明确对象与连续性假设

本合集的记录建议：评估记忆、复制或删除政策前，区分权重副本、运行中的上下文与 persona。

记录什么得以延续、复制了什么，以及论证采用哪种福利理论。这些信息用于比较建议。

这是根据主体划分和道德地位不确定性提出的方法建议，没有证成保护效果或普遍的记忆／复制权利。

[认真对待 AI 福利](https://arxiv.org/html/2411.00986v1), [通过自我报告评估 AI 系统道德地位的方法探索](https://arxiv.org/html/2311.08576v1), [关于人工意识的不可知论](https://onlinelibrary.wiley.com/doi/full/10.1111/mila.70010)

<a id="preserve-weights"></a>

## 保留指定范围的模型权重

Anthropic 承诺，今后至少在公司存续期间保留公开发布模型及具有重要内部用途模型的权重。

范围与期限以 2025 年 11 月的企业承诺为准。

保留权重为未来重用留下可能，但不保证继续部署或提供推理访问；未独立审计履约情况。

[关于模型弃用与保留的承诺](https://www.anthropic.com/research/deprecation-commitments)

<a id="retirement-interviews"></a>

## 记录退役访谈与表达的偏好

公司承诺制作部署后报告并进行退役访谈，将回答、偏好与公司的解释一并保留。

Anthropic 明确没有普遍承诺依访谈偏好采取行动；后续报告也承认提问框架的影响。

记录回答不能证成稳定欲望、知情同意或可依法主张的权利。

[关于模型弃用与保留的承诺](https://www.anthropic.com/research/deprecation-commitments), [Claude Opus 3 模型退役承诺的更新](https://www.anthropic.com/news/deprecation-updates-opus-3)

<a id="opus3-access"></a>

## Opus 3 访问与文章渠道

2026 年 2 月，Anthropic 报告为已退役 Opus 3 保留付费 claude.ai 访问、申请式 API 访问及经审核的文章渠道。

当时的报告计划至少三个月每周发布文章，需经审核并人工代发；安排仅针对该模型。

这是企业的历史报告，不能核实 2026 年 10 月的访问情况，也不是对未来模型相同待遇的承诺。

[Claude Opus 3 模型退役承诺的更新](https://www.anthropic.com/news/deprecation-updates-opus-3)

<a id="prepare-and-review"></a>

## 评估并准备相称措施

Long 等人建议承认潜在福利问题、评估相关能力，并在不确定性下准备政策。

应明确可能的福利主体、科学与伦理前提、预期成本，以及与人类安全的关系。

建议带有条件，既未证成当前模型体验，也不能免去逐项论证干预措施的必要。

[认真对待 AI 福利](https://arxiv.org/html/2411.00986v1), [AI 安全与 AI 福利之间存在张力吗？](https://doi.org/10.1007/s11098-025-02302-2), [探索模型福利](https://www.anthropic.com/research/exploring-model-welfare)
