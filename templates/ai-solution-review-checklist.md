# AI Solution Review Pack

Use this before pilot launch, production release, or scale-up. The goal is to surface unresolved delivery, architecture, evaluation, and governance gaps.

## 1. Review context

```text
Use case:
Risk tier:
Business owner:
Technical owner:
Review stage: prototype / pilot / production / scale
Decision requested:
```

## 2. Architecture review

| Area | Evidence required | Status |
| --- | --- | --- |
| Workflow map | Current and future-state workflow | |
| Context architecture | Sources, metadata, retrieval, freshness | |
| Model/prompt design | Prompt contract, model choice, fallback | |
| Integration | Systems touched, APIs, tool authority | |
| Observability | Logs, traces, cost, latency, quality signals | |
| Resilience | Failure behavior, rollback, escalation | |

## 3. Evaluation review

| Question | Evidence |
| --- | --- |
| What test set was used? | |
| What are the top failure modes? | |
| Which hard gates must pass? | |
| How does quality compare to baseline? | |
| What human rework remains? | |
| What will be monitored after launch? | |

## 4. Governance review

| Control | Required? | Implemented? | Owner |
| --- | --- | --- | --- |
| Risk tier assigned | | | |
| Human approval gate | | | |
| Access control | | | |
| Audit trail | | | |
| Incident path | | | |
| Data retention / redaction | | | |

## 5. Adoption review

| Adoption question | Answer |
| --- | --- |
| What behavior changes for users? | |
| What work is removed, not added? | |
| Who handles exceptions? | |
| What training or enablement is required? | |
| How will feedback improve the system? | |

## 6. Decision

```text
Approve:
Approve with conditions:
Defer:
Stop:
Conditions / actions:
Decision owner:
Date:
```