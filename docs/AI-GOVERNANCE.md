# AI Governance: Controls That Travel with the Work

AI governance fails when it becomes a document review at the end of delivery. It works when controls travel with the use case from intake to production.

The objective is not to slow delivery. The objective is to make delivery repeatable, explainable, and safe enough to scale.

## Governance layers

| Layer | Leadership question |
| --- | --- |
| Portfolio | Are we funding the right AI work? |
| Use case | Is there a business owner and measurable outcome? |
| Data/context | Is the knowledge approved, current, and access-controlled? |
| Model/prompt | Is behavior versioned, tested, and monitored? |
| Workflow/action | What can the system do, and who approves it? |
| Operations | How are failures, drift, cost, and incidents handled? |

## Risk-tiered control model

| Risk tier | Example | Minimum controls |
| --- | --- | --- |
| Low | Internal summarization | Usage monitoring and feedback path |
| Medium | Customer support recommendation | Evaluation set, citations, human override |
| High | Contract, HR, finance, regulated workflow | Approval gate, audit trail, risk review, incident path |
| Critical | Autonomous high-value or irreversible action | Block by default until explicitly governed |

## Governance artifacts that matter

- AI use-case register
- Risk tier and rationale
- Context ownership map
- Evaluation scorecard
- Prompt/model/tool version history
- Human approval matrix
- Audit and monitoring plan
- Incident response path

## Anti-patterns

- Governance board reviews without technical evidence
- Risk classification after solution design
- Model governance that ignores tools and workflow actions
- Manual approvals that are not captured in the system
- No owner for post-launch monitoring
- Treating open-source or vendor tools as automatically safe

## Practical operating recommendation

Create a lightweight AI control review for every material use case:

```text
Business owner present?
Risk tier agreed?
Context sources approved?
Evaluation scorecard reviewed?
Hard gates passed?
Monitoring owner assigned?
Incident path confirmed?
Scale decision recorded?
```

Good governance should make good teams faster because it removes ambiguity before scale.