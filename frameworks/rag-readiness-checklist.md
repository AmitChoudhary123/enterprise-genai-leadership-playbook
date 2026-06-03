# RAG Readiness Diligence Framework

This framework treats RAG as an enterprise knowledge product, not a retrieval feature. Use it before funding or scaling any RAG-based assistant, copilot, or agent.

## 1. Executive readiness question

Can the organization prove that answers are grounded in approved, current, and accessible knowledge, and that failures have an owner?

If not, the RAG system is not ready for scale.

## 2. Diligence dimensions

| Dimension | What to inspect | Red flag |
| --- | --- | --- |
| Knowledge ownership | Source owner, approval process, refresh cadence | Nobody owns the content after indexing |
| Source quality | Completeness, conflicts, obsolete versions | Multiple truths with no arbitration process |
| Metadata architecture | Domain, geography, product, entitlement, date, version | Retrieval cannot filter by business context |
| Retrieval design | Keyword, vector, hybrid, graph, reranking strategy | One retrieval method used for every question type |
| Grounding contract | Citation requirement, unsupported-answer behavior | Model allowed to answer without evidence |
| Evaluation set | Golden queries, edge cases, adversarial questions | Testing limited to demo questions |
| Access control | User entitlement and source restrictions | Sensitive content retrievable by wrong audience |
| Operations | Monitoring, feedback, failed-answer review | No owner for bad answers after launch |

## 3. Maturity scale

| Level | Description | Scale recommendation |
| --- | --- | --- |
| 1. Indexed | Documents loaded into a vector store | Exploration only |
| 2. Searchable | Retrieval works for known questions | Internal pilot |
| 3. Grounded | Answers cite approved sources and refuse when unsupported | Controlled production |
| 4. Governed | Ownership, access, evaluation, refresh, and monitoring are operational | Enterprise scale |
| 5. Learning | Feedback and failed-answer reviews improve context continuously | Strategic knowledge platform |

## 4. RAG architecture review board questions

- Which source is authoritative when documents conflict?
- How are new, changed, and retired documents handled?
- What metadata is mandatory before content enters the index?
- What is the retrieval benchmark and current score?
- Which questions should the system refuse?
- Can the answer cite source, version, and date?
- Who reviews failed answers weekly?
- What is the incident path for a harmful or wrong answer?

## 5. Implementation guidance

- Use hybrid retrieval for policy-heavy or terminology-variable domains.
- Add reranking when precision matters more than speed.
- Keep retrieval evaluation separate from generation evaluation.
- Require citations for factual enterprise answers.
- Add freshness filters for policy, legal, product, and compliance knowledge.
- Create a failed-query review loop with business source owners.

## 6. Investment decision

| Readiness profile | Decision |
| --- | --- |
| Strong source ownership, weak retrieval | Fund technical build |
| Weak source ownership, strong prototype | Pause and fix operating model |
| Strong retrieval, weak evaluation | Pilot only, do not scale |
| Strong grounding and governance | Scale as enterprise knowledge capability |

RAG failures are often blamed on AI engineering. In practice, many are knowledge-management failures exposed by AI.