# Master Knowledge Graph

This file is the stable mental map for the LLM Limitations Atlas course.
The course follows Stage 0 through Stage 6 in order. Topics may expand when the literature requires it, but no required stage is skipped.

## Root map

```text
LLM SYSTEM
|
+-- Stage 0: Mental framework
|   +-- How LLMs work
|   +-- Where limitations can arise
|   +-- How limitation claims are evaluated
|
+-- Stage 1: Historical foundations
|   +-- 2020
|   +-- 2021
|   +-- 2022
|   +-- Emergence of modern limitation research
|
+-- Stage 2: Core behavioral limitations
|   +-- Reasoning
|   +-- Generalization
|   +-- Hallucination / factuality
|   +-- Calibration / uncertainty
|   +-- Context / memory
|   +-- Grounding / causal understanding
|
+-- Stage 3: Interaction + learning/control
|   +-- Prompt sensitivity
|   +-- Multilingual / cultural
|   +-- Multimodal
|   +-- Alignment / controllability
|   +-- Knowledge editing
|   +-- Forgetting / unlearning
|
+-- Stage 4: Systems + safety
|   +-- Agents / planning
|   +-- RAG / tool use
|   +-- Bias / fairness
|   +-- Security / jailbreaks
|   +-- Privacy / memorization
|   +-- Efficiency / cost
|
+-- Stage 5: Evaluation
|   +-- Benchmark contamination
|   +-- Benchmark validity
|   +-- Shortcut success
|   +-- LLM judges
|   +-- Evaluation reliability
|
+-- Stage 6: Integrated synthesis
    +-- What was fixed?
    +-- What persists?
    +-- What is disputed?
    +-- What might be fundamental?
    +-- What remains unknown?
```

## Knowledge-graph dimensions

Every important limitation should eventually connect to the following dimensions:

1. **Definition** — what exactly is failing?
2. **Manifestation** — what observable behavior does it produce?
3. **Possible mechanism** — why might it happen?
4. **Evidence** — which experiments/papers support it?
5. **Counter-evidence** — which papers weaken, qualify, or contradict the claim?
6. **Measurement** — which benchmarks or evaluation methods expose it?
7. **Mitigation** — which methods reduce it?
8. **Model evolution** — what changed from earlier models to newer models?
9. **Persistence** — does it remain in 2025–2026 systems?
10. **Connections** — which other limitations interact with it?

## Allowed edge types

- `MANIFESTS_AS`
- `SUPPORTED_BY`
- `CHALLENGED_BY`
- `MEASURED_BY`
- `MAY_BE_CAUSED_BY`
- `MITIGATED_BY`
- `INTERACTS_WITH`
- `IMPROVED_IN`
- `PERSISTS_IN`
- `DISPUTED_BY`

## Confidence labels

Causal or broad claims must carry a confidence level:

- `ESTABLISHED`
- `STRONGLY_SUPPORTED`
- `PLAUSIBLE`
- `HYPOTHESIS`
- `DISPUTED`

Do not turn correlation, one benchmark result, or one model failure into a causal or universal statement.

## Evidence roles for each major topic

A topic is not considered mature until its evidence map includes, when available:

```text
Foundational / origin evidence
        -> Strong empirical demonstration
        -> Replication / extension
        -> Counter-evidence / qualification
        -> Modern-model reassessment
        -> 2025–2026 frontier evidence
        -> Current synthesis
```

The number of papers is not fixed. A topic is complete when the evidence graph is sufficiently supported and the learner can reconstruct it from memory.

## Final mental-model target

At the end of the course, the learner should be able to:

- draw the major limitation graph from memory;
- distinguish neighboring limitations;
- place a new failure or paper in the graph;
- explain the strongest evidence and counter-evidence;
- distinguish model limitations from system and evaluation problems;
- explain what scaling and newer methods improved;
- identify what remains persistent, disputed, or unknown.
