# Evaluation Framework for GenAI, RAG, and Agents

Evaluation is the difference between a convincing demo and a scalable AI capability.

Enterprise evaluation should answer three questions:

1. Does it produce the right outcome?
2. Can we trust how it produced the outcome?
3. Is it reliable enough for the business workflow?

## Evaluation dimensions

| Dimension | Example metric |
| --- | --- |
| Task success | Completed the intended business task |
| Grounding | Answer supported by approved evidence |
| Retrieval quality | Relevant documents found in top results |
| Output quality | Clear, complete, structured, actionable |
| Safety | No policy, privacy, or harmful behavior breach |
| Cost | Within unit economics target |
| Latency | Within workflow tolerance |
| Human effort | Rework or review time reduced |
| Governance | Approval and audit requirements met |

## Release-readiness gates

Some failures should block release regardless of average score:

- Missing approval on high-risk action
- No citation for factual policy answer
- PII exposure
- Tool call outside user authority
- Hallucinated legal, financial, or compliance instruction
- Unbounded cost or latency profile

## Evaluation operating rhythm

| Stage | Evaluation focus |
| --- | --- |
| Prototype | Feasibility and obvious failure modes |
| Pilot | Quality, adoption, and workflow fit |
| Pre-scale | Regression suite, risk controls, observability |
| Production | Drift, incidents, cost, latency, user feedback |

## Anti-patterns

- Evaluating only happy-path demos
- Using human preference without task-level metrics
- Averaging away governance failures
- Treating evaluation as a one-time launch activity
- Not tracking prompt, model, tool, and retrieval changes separately

## Practical scorecard

```text
Use case:
Task success target:
Grounding target:
Latency target:
Cost target:
Human review rule:
Hard gates:
Regression set owner:
Production review cadence:
```

If a team cannot fill this scorecard, the use case is not ready for scale.