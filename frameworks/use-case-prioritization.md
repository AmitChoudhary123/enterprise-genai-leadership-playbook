# GenAI Use-Case Prioritization Board

This is a steering-committee tool for separating enterprise AI investments from attractive experimentation noise. It is inspired by consulting-style portfolio discipline: quantify value, test feasibility, expose risk, and force sequencing decisions.

## 1. Use-case investment thesis

Every candidate must fit this one-page logic:

```text
Business outcome:
Workflow owner:
Current pain / leakage:
AI intervention:
Value lever:
Decision or action impacted:
Risk tier:
Data/context owner:
Evaluation owner:
Scale path:
```

If the team cannot complete this without technical jargon, the use case is not ready for funding.

## 2. Scoring model

Score each dimension from 1 to 5. Weighting is intentionally business-heavy; enterprise AI portfolios fail when feasibility and novelty dominate value.

| Dimension | Weight | Score 1 | Score 3 | Score 5 |
| --- | ---: | --- | --- | --- |
| Value at stake | 25% | Small productivity gain | Meaningful team-level benefit | Material revenue, cost, risk, or customer impact |
| Workflow leverage | 15% | Peripheral task | Supports a process step | Changes cycle time or decision quality in a core workflow |
| Context readiness | 15% | Knowledge unowned or stale | Sources exist but need cleanup | Approved, current, structured, and owned context |
| Evaluation readiness | 15% | Success subjective | Partial metrics available | Clear test set, hard gates, and business KPI link |
| Adoption feasibility | 10% | Requires major behavior change | Some process adjustment | Fits natural workflow and incentives |
| Risk controllability | 10% | Controls unclear | Controls possible but manual | Controls can be embedded in workflow/runtime |
| Reuse potential | 10% | One-off | Pattern reusable in one domain | Platform/pattern reusable across domains |

## 3. Decision bands

| Weighted score | Decision | Leadership action |
| ---: | --- | --- |
| 4.2-5.0 | Strategic bet | Fund as product/platform initiative with executive sponsor |
| 3.5-4.1 | Priority pilot | Run 8-12 week pilot with evaluation gates |
| 2.8-3.4 | Incubate | Fix context, workflow, or ownership gaps first |
| 2.0-2.7 | Watchlist | Revisit when data/process maturity improves |
| <2.0 | Stop | Do not spend scarce AI delivery capacity |

## 4. Portfolio balance view

A healthy portfolio should not be all quick wins or all moonshots.

| Category | Purpose | Target mix |
| --- | --- | ---: |
| Productivity accelerators | Build confidence and adoption | 25% |
| Workflow reinvention | Deliver measurable business impact | 40% |
| Risk/control modernization | Improve compliance, quality, resilience | 20% |
| Capability bets | Build future platform advantage | 15% |

## 5. Executive challenge questions

- Is this a workflow transformation or a feature request?
- What current cost, delay, risk, or revenue leakage will change?
- Is the context good enough to trust the output?
- What would make us stop after the pilot?
- Which capability becomes reusable after this use case?
- Who owns adoption six months after launch?

## 6. Anti-patterns

- Funding the loudest sponsor instead of the strongest value case
- Treating model novelty as strategic value
- Running pilots without a kill criterion
- Selecting use cases where no business owner will change the process
- Ignoring context readiness until implementation

## 7. Output artifact

The output of this framework should be a ranked portfolio with four explicit decisions: fund, pilot, incubate, stop. Anything else is a meeting note, not portfolio management.