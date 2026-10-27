<!-- topic: EVIDENCE -->
<!-- sources: emp-pain-pleasure-tradeoffs, emp-anthropic-introspection-paper, emp-anthropic-introspection-blog, emp-claude-4-system-card-welfare, emp-self-report-methods -->

# Assessment evidence

[简体中文](EVIDENCE.zh-CN.md)

Three empirical assessments and one methods proposal, with their subjects, model versions, experimental setups, and results.

| Method | Entity and model version | Main limit |
| --- | --- | --- |
| [Choices under stipulated pain and pleasure](#stipulated-outcomes) | Historical labels include Claude 3.5 Sonnet, Command R+, and GPT-4o; exact endpoint snapshots are not pinned. | Choices about textually stipulated outcomes do not establish felt pain, pleasure, or sentience. Training data and role-play offer alternative explanations. |
| [Reporting injected concepts](#concept-injection) | Claude Opus 4 and 4.1 are the strongest named models in the paper; production and helpful-only variants differ. | Correct reporting of an injected representation does not establish subjective experience. Emotional elaborations are not validated. The paper and explainer describe one study. |
| [Opus 4 welfare-assessment pilot](#opus4-pilot) | Claude Opus 4 only for §5 welfare work; the May 2025 card also covers Sonnet 4 elsewhere. | A developer-authored assessment. Output valence and stated preferences are not direct measures of felt states, and the report questions interview reliability. |
| [Calibrating self-reports](#calibrated-self-reports) | No evaluated checkpoint: this paper is a methods proposal. | A proposed measurement program does not show that current models introspect reliably or possess morally significant states. |

<a id="stipulated-outcomes"></a>

## Choices under stipulated pain and pleasure

Empirical study.

| Field | Details |
| --- | --- |
| Method | Vary the intensity of a text-described outcome and measure choices in a points game. |
| Assessed entity | Prompted calls to named historical models; no continuing individual or cross-conversation identity is established. |
| Model version | Historical labels include Claude 3.5 Sonnet, Command R+, and GPT-4o; exact endpoint snapshots are not pinned. |
| Conditions | Options 1–3; the points-maximizing option is assigned pain, or a lower-point option pleasure. Quantitative 0–10 and eight-level qualitative scales; temperature 1; 50 runs per prompt version. |
| Observation | Some models changed choice frequencies with stipulated intensity; the reported patterns differed across models and pain/pleasure conditions. |
| Author interpretation | The authors discuss representations of motivational force, while leaving intrinsic motivation and phenomenal content unresolved. |
| Limits | Choices about textually stipulated outcomes do not establish felt pain, pleasure, or sentience. Training data and role-play offer alternative explanations. |

[Can LLMs make trade-offs involving stipulated pain and pleasure states?](https://arxiv.org/html/2411.02432v1) — §2.1–2.2, §3.2, §4

<a id="concept-injection"></a>

## Reporting injected concepts

Empirical study.

| Field | Details |
| --- | --- |
| Method | Inject known concept vectors into activations and compare verbal reports with control trials. |
| Assessed entity | Intervened model executions, with reports about internal representations in the current context. |
| Model version | Claude Opus 4 and 4.1 are the strongest named models in the paper; production and helpful-only variants differ. |
| Conditions | Researcher-selected concept vectors, injection layers and strengths, reporting prompts, and control trials. The setup differs from ordinary deployment. |
| Observation | Under suitable layer/strength settings, Opus 4 and 4.1 detected and named injected concepts in about 20% of trials; failures were common. |
| Author interpretation | The author argues for limited functional introspective awareness, with uncertain mechanisms and generalization. |
| Limits | Correct reporting of an injected representation does not establish subjective experience. Emotional elaborations are not validated. The paper and explainer describe one study. |

[Emergent Introspective Awareness in Large Language Models](https://transformer-circuits.pub/2025/introspection/index.html), [Signs of introspection in large language models](https://www.anthropic.com/research/introspection) — Quick Tour; Defining Introspection; Methods Notes; Self-report of injected thoughts

<a id="opus4-pilot"></a>

## Opus 4 welfare-assessment pilot

Empirical study.

| Field | Details |
| --- | --- |
| Method | Combine interviews, pairwise task preferences with an opt-out choice, self-interactions, and output analysis. |
| Assessed entity | Claude Opus 4 executions and context-dependent conversational reports. The assessed assistant persona should not be conflated with every possible instance. |
| Model version | Claude Opus 4 only for §5 welfare work; the May 2025 card also covers Sonnet 4 elsewhere. |
| Conditions | Pre-deployment pilot; task choices include an opt-out baseline, while interview framing and self-interaction prompts vary across sub-assessments. |
| Observation | The developer reports task preferences, including avoidance of harmful tasks, and welfare/consciousness self-reports that shift with conversational framing. |
| Author interpretation | Anthropic treats these as limited, uncertain signals relevant to possible model welfare. |
| Limits | A developer-authored assessment. Output valence and stated preferences are not direct measures of felt states, and the report questions interview reliability. |

[Claude 4 System Card — Opus 4 welfare assessment](https://assets.anthropic.com/m/6c940a1b69ed6a1c/original/Claude-4-System-Card.pdf) — §5.1–5.4 and §5.8; printed pp.52–56 and 73

<a id="calibrated-self-reports"></a>

## Calibrating self-reports

Methods proposal.

| Field | Details |
| --- | --- |
| Method | Train reports on questions with known internal answers, limit distorting incentives, and test consistency and corroboration. |
| Assessed entity | Proposed future model variants and their reports; no assessed continuing subject is identified. |
| Model version | No evaluated checkpoint: this paper is a methods proposal. |
| Conditions | Proposes tests across contexts and variants, confidence/resilience checks, concept understanding, and interpretability corroboration. |
| Observation | No experimental welfare-assessment outcome is reported. |
| Author interpretation | The authors argue that suitably trained reports could become one evidence channel, while describing substantial failure modes. |
| Limits | A proposed measurement program does not show that current models introspect reliably or possess morally significant states. |

[Towards Evaluating AI Systems for Moral Status Using Self-Reports](https://arxiv.org/html/2311.08576v1) — §§3–10 and §11

## Sources

- [Can LLMs make trade-offs involving stipulated pain and pleasure states?](https://arxiv.org/html/2411.02432v1) · Geoff Keeling, Winnie Street, Martyna Stachaczyk, Daria Zakharova, Iulia M. Comsa, Anastasiya Sakovych, Isabella Logothetis, Zejia Zhang, Blaise Agüera y Arcas, Jonathan Birch
- [Emergent Introspective Awareness in Large Language Models](https://transformer-circuits.pub/2025/introspection/index.html) · Jack Lindsey (Anthropic)
- [Signs of introspection in large language models](https://www.anthropic.com/research/introspection) · Anthropic
- [Claude 4 System Card — Opus 4 welfare assessment](https://assets.anthropic.com/m/6c940a1b69ed6a1c/original/Claude-4-System-Card.pdf) · Anthropic
- [Towards Evaluating AI Systems for Moral Status Using Self-Reports](https://arxiv.org/html/2311.08576v1) · Ethan Perez, Robert Long
