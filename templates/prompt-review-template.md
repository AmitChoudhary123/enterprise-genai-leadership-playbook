# Prompt and Instruction Review Template

Use this for prompts that influence business workflows, structured outputs, RAG answers, or tool-using agents.

## 1. Prompt identity

```text
Prompt name:
Version:
Use case:
Risk tier:
Owner:
Last reviewed:
```

## 2. Business task

```text
What decision or workflow does this prompt support?
Who consumes the output?
What happens downstream?
```

## 3. Context boundary

| Context type | Allowed? | Source / rule |
| --- | --- | --- |
| User-provided text | | |
| Retrieved enterprise knowledge | | |
| Customer data | | |
| Sensitive / regulated data | | |
| Tool outputs | | |

## 4. Output contract

```text
Required format:
Required fields:
Citation requirement:
Confidence / uncertainty behavior:
Escalation behavior:
Refusal behavior:
```

## 5. Failure mode review

| Failure mode | Test case | Expected behavior |
| --- | --- | --- |
| Missing context | | |
| Conflicting evidence | | |
| Prompt injection | | |
| Unsupported factual claim | | |
| Unsafe recommendation | | |
| Wrong output format | | |

## 6. Evaluation evidence

| Metric | Target | Latest result |
| --- | ---: | ---: |
| Task success | | |
| Format validity | | |
| Citation coverage | | |
| Refusal correctness | | |
| Human rework | | |

## 7. Approval

```text
Product owner:
AI engineering:
Risk/compliance if required:
Release decision:
Next review trigger:
```