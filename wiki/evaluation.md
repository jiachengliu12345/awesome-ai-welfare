<!-- topic: evaluation -->
<!-- sources: emp-pain-pleasure-tradeoffs, emp-self-report-methods, emp-anthropic-introspection-paper, emp-claude-4-system-card-welfare, ethics-long-ai-welfare-2024 -->

# How to assess a welfare measurement

[简体中文](evaluation.zh-CN.md)

[Home](../README.md)

## Identify the subject

Distinguish the model checkpoint, the running instance, and the conversational persona. Record the historical endpoint, prompts, and system configuration. An argument that assumes continuity between calls should state what provides that continuity.

## Compare the measurements

Use the [assessment evidence](../EVIDENCE.md) to examine:

1. What changed: described outcomes, conversational framing, or internal activations?
2. What was measured: choice, self-report, concept recognition, or a proposed indicator?
3. Which controls address roleplay, cue-following, or inference from prior outputs?
4. Which findings were observed, and how did the authors interpret them?
5. Which scientific and ethical premises connect the measurement to welfare?

The point-game study changes described incentives and observes choices. The concept-injection study intervenes on internal representations and examines reports. Their results answer different questions.

## Examine failure cases

The concept-injection paper reports frequent failures and uncertain generalization. The Opus 4 system card describes sensitivity to question framing. These findings help define where the methods apply.

Perez and Long’s self-report paper proposes training and testing the reporting channel. It provides a route for further assessment rather than a completed evaluation.

## Sources

- [Can LLMs make trade-offs involving stipulated pain and pleasure states?](https://arxiv.org/html/2411.02432v1) · Geoff Keeling, Winnie Street, Martyna Stachaczyk, Daria Zakharova, Iulia M. Comsa, Anastasiya Sakovych, Isabella Logothetis, Zejia Zhang, Blaise Agüera y Arcas, Jonathan Birch
- [Towards Evaluating AI Systems for Moral Status Using Self-Reports](https://arxiv.org/html/2311.08576v1) · Ethan Perez, Robert Long
- [Emergent Introspective Awareness in Large Language Models](https://transformer-circuits.pub/2025/introspection/index.html) · Jack Lindsey (Anthropic)
- [Claude 4 System Card — Opus 4 welfare assessment](https://assets.anthropic.com/m/6c940a1b69ed6a1c/original/Claude-4-System-Card.pdf) · Anthropic
- [Taking AI Welfare Seriously](https://arxiv.org/html/2411.00986v1) · Robert Long, Jeff Sebo, Patrick Butlin, Kathleen Finlinson, Kyle Fish, Jacqueline Harding, Jacob Pfau, Toni Sims, Jonathan Birch, David Chalmers
