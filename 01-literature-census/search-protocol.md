# Literature Search Protocol

## Objective

Build a reproducible, high-recall census of papers relevant to limitations of LLMs from 2020 through 2026.

## Principle

Do not rely on one keyword such as "LLM limitations". Terminology changed across the period, especially in 2020–2021.

## Retrieval layers

### Layer 1 — Broad model-family retrieval

Retrieve papers related to large/pretrained/foundation language models and major model families.

### Layer 2 — Limitation concept retrieval

Search concepts including, but not limited to:

- limitation / failure / weakness
- robustness / brittleness
- generalization / compositionality
- hallucination / factuality / truthfulness
- calibration / uncertainty / self-correction
- memorization / privacy / leakage
- bias / fairness
- jailbreak / adversarial / prompt injection
- long context / memory / lost in the middle
- reasoning / logic / math / causal
- contamination / benchmark validity
- multilingual / cultural
- multimodal
- alignment / controllability
- knowledge editing / forgetting / unlearning
- agents / planning / tool use
- efficiency / compute / latency / energy

### Layer 3 — Seed-survey expansion

Collect all references and cited/citing papers from major limitation surveys and taxonomies.

### Layer 4 — Citation chaining

For each foundational paper:

- backward chaining: references it builds on;
- forward chaining: later work citing it;
- related-work reconciliation.

### Layer 5 — Venue reconciliation

Check important NLP/ML venues and proceedings for papers missed by generic retrieval.

## Deduplication

Prefer identifiers in this order:

1. DOI
2. arXiv ID
3. ACL Anthology ID
4. normalized title + first author + year

Keep preprint and published versions linked rather than counting them as unrelated papers.

## Reproducibility

Every retrieval run must store its query/configuration in `searches/` and append a coverage entry to `coverage-report.md`.
