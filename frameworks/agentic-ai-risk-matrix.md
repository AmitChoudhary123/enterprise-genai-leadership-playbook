# Agentic AI Risk Matrix

| Action type | Risk | Required control |
| --- | --- | --- |
| Summarize internal content | Low | Usage monitoring |
| Recommend next best action | Medium | Human override and evaluation set |
| Update enterprise system | High | Approval gate, audit log, rollback plan |
| Trigger financial or legal action | Critical | Block by default unless explicitly governed |

## Practical rule

The more irreversible the action, the less autonomy should be granted without explicit policy, approval, and monitoring.