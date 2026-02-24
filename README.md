# project-template

A universal project template providing two parallel document traceability chains
and a human-readable summary layer.

## What this is

This repository is a **starting point for any project** that wants structured,
traceable documentation. Clone or copy it, delete this README's "template" note,
and start writing.

It provides:

- **Decision Traceability Chain** (ADR → DR → EIR / TR) — records YOUR decisions
- **Analysis Traceability Chain** (AA → DA → TA) — records understanding of EXTERNAL systems
- **Summary Layer** — human-readable Chinese summaries for every document type

## Directory structure

```
docs/
  adr/              Architecture Decision Records — "what did we decide and why?"
    summary/         Chinese summaries
  dr/               Design Rationale — "why was it built this way?"
    summary/
  eir/              Engineering Investigation Records — "what did we explore?"
    summary/
  tr/               Test Rationale — "why does this test exist?"
    summary/
  ret/              After Action Records — "what happened and what did we learn?"
    summary/
  aa/               Architecture Analysis — "what did THEY build and why?"
    summary/
  da/               Design Analysis — "how does THEIR component work?"
    summary/
  ta/               Test Analysis — "how do THEY test and why?"
    summary/
  knowledge/        Distilled team knowledge entries
    summary/
  issues/           Structured issue documents
    summary/
```

## The two chains

### Decision Chain (forward-looking): "What shall we build?"

```
ADR-XXXX                          (Architecture Decision)
  └── DR-XXXX-YYYY                (Design Rationale)
        ├── EIR-XXXX-YYYY-ZZZZ   (Engineering Investigation Record)
        ├── TR-XXXX-YYYY-ZZZZ    (Test Rationale)
        └── RET-XXXX-YYYY-ZZZZ   (After Action Record)
```

### Analysis Chain (backward-looking): "What did they build and why?"

```
AA-XXXX                           (Architecture Analysis)
  └── DA-XXXX-YYYY                (Design Analysis)
        └── TA-XXXX-YYYY-ZZZZ    (Test Analysis)
```

The two chains are independent but may cross-reference each other.

## Summary layer

Every document type directory has a `summary/` sub-directory containing
human-readable Chinese summaries. Summaries are:

- Short (5–15 sentences)
- Storytelling tone (讲故事)
- 1:1 filename mapping with the parent document
- Not translations — they tell the story of what happened and why it matters

## Conventions

- IDs are immutable once assigned
- Documents are never deleted — supersede them instead
- Use `0000` as a placeholder when no parent exists at a given level
- Each directory has a README explaining its purpose and format
