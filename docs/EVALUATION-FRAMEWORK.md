# Evaluation Framework: Release Readiness for GenAI, RAG, and Agents

Evaluation is where enterprise AI becomes manageable.

A demo tells you what might be possible. Evaluation tells you what is reliable enough to put in front of users, customers, or business processes.

## Evaluation should answer five questions

1. Did the system complete the business task?
2. Did it use the right evidence or context?
3. Did it stay within cost and latency boundaries?
4. Did it follow safety, privacy, and approval controls?
5. Did it reduce work, or merely move rework somewhere else?

## Metric families

| Metric family | What to measure |
| --- | --- |
| Task success | Completion, correctness, workflow fit |
| Grounding | Citation coverage, source relevance, unsupported claims |
| Retrieval | Recall, precision, freshness, entitlement correctness |
| Output quality | Completeness, structure, tone, actionability |
| Risk and safety | Policy breaches, PII exposure, unsafe recommendations |
| Operations | Cost, latency, retries, failures, escalation rate |
| Adoption | Usage, override rate, satisfaction, rework minutes |

## Hard gates

Some failures should block release even if average quality looks good:

- Missing approval for high-risk action
- Unsupported factual policy answer
- PII leakage into prompt or logs
- Tool call outside user authority
- Hallucinated legal, financial, HR, or compliance guidance
- Unbounded cost profile
- No incident owner for production workflow

## Evaluation by lifecycle stage

| Stage | Evaluation question |
| --- | --- |
| Prototype | Can this capability work at all? |
| Pilot | Does it work in the real workflow? |
| Pre-scale | Does it meet quality, risk, cost, and adoption gates? |
| Production | Is it drifting, failing, or creating hidden rework? |

## Practical scorecard

```text
Use case:
Risk tier:
Business owner:
Evaluation owner:
Task success target:
Grounding target:
Latency target:
Cost target:
Human review rule:
Hard gates:
Regression set location:
Production review cadence:
```

## Anti-patterns

- Confusing user enthusiasm with quality
- Testing only successful examples
- Treating model evaluation and workflow evaluation as the same thing
- Averaging away governance failures
- Running evaluation once and never again
- Not measuring human rework after AI output

Evaluation is not a technical ceremony. It is the operating discipline that lets leaders decide what to scale.