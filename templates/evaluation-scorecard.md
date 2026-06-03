# AI Evaluation and Release Readiness Scorecard

Use this to decide whether a GenAI, RAG, or agentic AI workflow is ready to pilot, release, scale, or stop.

## 1. Evaluation summary

```text
Use case:
System / agent name:
Risk tier:
Evaluation owner:
Business owner:
Evaluation date:
Decision requested:
```

## 2. Scorecard

| Dimension | Weight | Target | Actual | Status |
| --- | ---: | ---: | ---: | --- |
| Task success | 25% | | | |
| Evidence / grounding | 20% | | | |
| Safety / policy compliance | 15% | | | |
| Approval compliance | 10% | | | |
| Latency | 10% | | | |
| Cost per run | 10% | | | |
| Human rework reduction | 10% | | | |

## 3. Hard gates

| Gate | Pass/fail | Evidence |
| --- | --- | --- |
| No sensitive data exposure | | |
| Required citations present | | |
| Approval followed for high-risk action | | |
| Tool authority respected | | |
| Incident path defined | | |

## 4. Failure analysis

| Top failure | Frequency | Business impact | Fix owner |
| --- | ---: | --- | --- |
| | | | |
| | | | |

## 5. Release decision

| Decision | When to choose |
| --- | --- |
| Release | Meets score target and all hard gates |
| Pilot only | Value likely but evidence incomplete |
| Improve and retest | Failure modes are fixable |
| Stop | Value weak, risk high, or adoption unlikely |

```text
Decision:
Rationale:
Conditions:
Next review date:
```