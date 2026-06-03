# Agentic AI Risk Matrix

Agent risk is driven less by the model and more by the action the agent can take.

| Agent capability | Example | Risk posture | Required control |
| --- | --- | --- | --- |
| Read and summarize | Summarize policy or ticket history | Low | Monitoring and feedback |
| Recommend | Suggest next best action | Medium | Human review or override |
| Prepare transaction | Draft refund, contract clause, or vendor response | Medium-high | Approval workflow and audit |
| Execute reversible action | Update CRM, create ticket, send internal notification | High | Authorization, logging, rollback |
| Execute irreversible/material action | Release payment, change customer entitlement, terminate access | Critical | Block by default or require explicit governed workflow |

## Design rule

Increase autonomy only when four things are true:

1. The task boundary is narrow.
2. The context is reliable.
3. Evaluation evidence is strong.
4. The action is reversible or controlled.

## Review questions

- What is the worst credible outcome?
- Who is accountable if the agent acts incorrectly?
- Can the action be reversed?
- Is the user authorized for the action?
- Is approval captured in the system?
- Is the audit trail sufficient for incident review?