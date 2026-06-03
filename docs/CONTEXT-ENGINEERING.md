# Context Engineering: The Enterprise Discipline Behind RAG and Agents

Context engineering is the discipline of deciding what an AI system is allowed to know at the moment it acts.

For many enterprise systems, context quality matters more than model choice. A stronger model with weak, stale, or poorly governed context will still produce unreliable outcomes. A good context layer makes the system more accurate, explainable, and governable.

## Context is not just retrieval

RAG teams often reduce context engineering to vector search. That is too narrow.

Enterprise context includes:

- Source authority: which knowledge is approved
- Metadata: who owns it, when it expires, what domain it applies to
- Entitlements: who is allowed to see or use it
- Retrieval strategy: lexical, vector, hybrid, graph, or workflow-state lookup
- Ranking and compression: what evidence reaches the model
- Citation and grounding: how the output proves its basis
- Refresh and retirement: how old knowledge disappears
- Workflow state: what the user is doing and what action is allowed

## Context architecture decision table

| Situation | Recommended pattern |
| --- | --- |
| Policy or compliance answer | Hybrid retrieval, strict citations, freshness filter |
| Customer support knowledge | Metadata-rich RAG with feedback loop from unresolved cases |
| Analytical narrative | Query-backed context plus generated explanation |
| Agentic workflow | Tool state, user authority, process state, and policy context |
| Executive briefing | Curated source pack, date boundaries, and explicit assumptions |

## RAG readiness review

Before scaling a RAG system, ask:

- Are source owners named?
- Are documents current, approved, and classified?
- Is metadata rich enough to filter by domain, geography, policy version, and access level?
- Is retrieval tested independently from answer generation?
- Are citations mandatory for factual claims?
- Are failed retrievals reviewed by a business owner?
- Is there a process for retiring stale content?

## Agent context review

For agents, add these questions:

- What tools are available in this workflow?
- What is the user authorized to do?
- What prior actions have already occurred?
- Which actions require approval?
- What should the agent do when context is incomplete?
- What audit evidence is retained after tool use?

## Common failure patterns

- Uploading content without ownership or metadata
- Using one retrieval strategy for every knowledge type
- Ignoring stale or contradictory sources
- Evaluating final answers but not retrieval quality
- Giving agents tools without process state
- Passing excessive context and hoping the model resolves conflict

## Practical recommendation

Create a context map for every serious use case:

```text
Workflow step -> Required context -> Source owner -> Access rule -> Freshness rule -> Retrieval method -> Evaluation query -> Failure owner
```

This map is often the difference between an AI demo and an enterprise architecture.