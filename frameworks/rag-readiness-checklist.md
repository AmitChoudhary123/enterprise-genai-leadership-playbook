# RAG Readiness Checklist

A RAG system is not ready because documents were indexed. It is ready when evidence can be trusted, retrieved, cited, and maintained.

## Source readiness

- Source owner named
- Content approved for AI use
- Access classification defined
- Refresh frequency known
- Superseded content retired
- Sensitive fields identified

## Retrieval readiness

- Metadata supports filtering by domain, geography, policy version, date, and entitlement
- Test queries exist for common, edge, and ambiguous questions
- Retrieval is evaluated separately from generation
- Top-k evidence is reviewable by business owners
- Hybrid retrieval considered where terminology mismatch exists

## Answer readiness

- Citations required for factual claims
- Unsupported answers escalate or refuse
- Output format matches workflow need
- Confidence or uncertainty is operationally meaningful
- Human review path exists for low-confidence answers

## Operating readiness

- Failed retrievals are reviewed
- Content freshness is monitored
- Feedback loop exists from users to source owners
- Evaluation suite runs before material retrieval or prompt changes

## Red flags

- No source owner
- No metadata strategy
- No citation requirement
- No stale-content process
- No evaluation set
- No owner for failed answers