# Agentic AI Autonomy and Risk Matrix

Agent risk is not defined by whether a system uses an LLM. It is defined by what the agent can do, what can go wrong, and whether the enterprise can detect, approve, and reverse the action.

## 1. Autonomy ladder

| Level | Agent behavior | Example | Control posture |
| --- | --- | --- | --- |
| L0 | Observe | Summarize ticket history | Logging and feedback |
| L1 | Recommend | Suggest next best action | Human accepts/rejects |
| L2 | Prepare | Draft email, refund, contract clause | Human approval before execution |
| L3 | Execute reversible action | Create ticket, update CRM, send internal notification | Authorization, audit, rollback |
| L4 | Execute material action | Issue refund, change entitlement, submit vendor decision | Explicit approval gate, monitoring, incident path |
| L5 | Execute irreversible/high-impact action | Terminate access, release payment, legal/HR action | Block by default unless governed exception |

## 2. Risk scoring

Score 1-5.

| Risk factor | Question |
| --- | --- |
| Customer impact | Could a customer be harmed or misled? |
| Financial exposure | Could money, pricing, entitlement, or revenue be affected? |
| Regulatory exposure | Does the action touch regulated decisions or records? |
| Reversibility | Can the action be undone quickly? |
| Authority | Is user/agent authority clear and enforceable? |
| Evidence dependency | Does the action depend on retrieved or inferred facts? |
| Failure detectability | Would a bad action be detected quickly? |

## 3. Control mapping

| Risk score | Autonomy allowed | Required controls |
| ---: | --- | --- |
| 7-12 | L0-L2 | Logging, review path, basic evaluation |
| 13-20 | L0-L3 | Approval rules, entitlement checks, audit trail, rollback |
| 21-28 | L0-L2 only | Human approval, risk review, incident plan, strict evidence |
| 29+ | L0-L1 only | No autonomous execution; decision support only |

## 4. Design principles

- Autonomy should be earned through evaluation evidence.
- Tool access should be narrower than model capability.
- Approval should be captured in the workflow, not in email.
- High-risk agents should produce audit-ready run reports.
- Every material action needs an owner, rollback path, and monitoring signal.

## 5. Common failure patterns

- Giving agents broad tools during pilots because it is faster
- Confusing user approval with accountable approval
- Logging final outputs but not tool calls
- Missing entitlement checks before tool execution
- Allowing agents to act on weak context
- Scaling autonomy before incident handling is tested

## 6. Executive decision rule

If the organization cannot explain who authorized the action, what evidence was used, and how the action can be reversed, the agent should not execute the action.