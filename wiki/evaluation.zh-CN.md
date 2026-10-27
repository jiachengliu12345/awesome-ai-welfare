<!-- topic: evaluation -->
<!-- sources: emp-pain-pleasure-tradeoffs, emp-self-report-methods, emp-anthropic-introspection-paper, emp-claude-4-system-card-welfare, ethics-long-ai-welfare-2024 -->

# 如何判断福利测量

[English](evaluation.md)

[首页](../README.zh-CN.md)

## 确定评估对象

区分模型检查点、运行实例与对话角色，记录历史端点、提示词及系统配置。若论证假定不同调用之间具有连续性，应说明这种连续性由什么维持。

## 比较测量

借助[评估证据表](../EVIDENCE.zh-CN.md)，逐项检查：

1. 实验改变了什么：文字描述的结果、对话框架，还是内部激活？
2. 测量了什么：选择、自我报告、概念识别，还是一个提议中的指标？
3. 哪些对照处理了角色扮演、跟随线索或根据已有输出推断的问题？
4. 观察到了什么，作者如何解释？
5. 哪些科学与伦理前提把测量结果与福利联系起来？

积分游戏研究改变描述中的激励并观察选择；概念注入研究干预内部表征并检查报告。两者回答的问题不同。

## 检查失败情形

概念注入论文报告了频繁失败和不确定的泛化能力；Opus 4 系统卡描述了对提问框架的敏感性。这些发现有助于界定方法的适用范围。

Perez 与 Long 的自我报告论文提出训练和检验报告渠道的方案，为后续评估提供研究路径。

## 来源

- [大语言模型能否权衡文字设定的疼痛与愉悦状态？](https://arxiv.org/html/2411.02432v1) · Geoff Keeling, Winnie Street, Martyna Stachaczyk, Daria Zakharova, Iulia M. Comsa, Anastasiya Sakovych, Isabella Logothetis, Zejia Zhang, Blaise Agüera y Arcas, Jonathan Birch
- [通过自我报告评估 AI 系统道德地位的方法探索](https://arxiv.org/html/2311.08576v1) · Ethan Perez, Robert Long
- [大语言模型中涌现的内省觉察](https://transformer-circuits.pub/2025/introspection/index.html) · Jack Lindsey (Anthropic)
- [Claude 4 系统卡：Opus 4 福利评估](https://assets.anthropic.com/m/6c940a1b69ed6a1c/original/Claude-4-System-Card.pdf) · Anthropic
- [认真对待 AI 福利](https://arxiv.org/html/2411.00986v1) · Robert Long, Jeff Sebo, Patrick Butlin, Kathleen Finlinson, Kyle Fish, Jacqueline Harding, Jacob Pfau, Toni Sims, Jonathan Birch, David Chalmers
