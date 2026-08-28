# Course Management Protocol

This file defines how the LLM Limitations Atlas course starts, continues, and finishes without losing quality or continuity.

## Source of truth

- **Chat = classroom.** Teaching, questions, exercises, and discussion happen in chat.
- **GitHub = course memory and scientific knowledge base.** Course state, summaries, evidence maps, and progress live here.

A long or restarted chat must never be the only place where course state exists.

## Fixed course sequence

The learning path is sequential:

`Stage 0 -> Stage 1 -> Stage 2 -> Stage 3 -> Stage 4 -> Stage 5 -> Stage 6`

A stage is completed before the next stage becomes the main teaching focus.
Earlier stages may later receive new papers or updated evidence, but the learner does not jump randomly between stages.

## Required stages

### Stage 0 — Mental framework
How LLMs work, where limitations can arise, and how limitation claims are evaluated.

### Stage 1 — Historical foundations
2020–2022 and the emergence of modern LLM limitation research.

### Stage 2 — Core behavioral limitations
Reasoning, generalization, hallucination/factuality, calibration, context/memory, grounding/causal understanding.

### Stage 3 — Interaction + learning/control
Prompt sensitivity, multilingual/cultural, multimodal, alignment, knowledge editing, forgetting/unlearning.

### Stage 4 — Systems + safety
Agents/planning, RAG/tool use, bias/fairness, security, privacy/memorization, efficiency/cost.

### Stage 5 — Evaluation
Contamination, benchmark validity, shortcut success, LLM judges, evaluation reliability.

### Stage 6 — Integrated synthesis
What was fixed, persists, is disputed, may be fundamental, and remains unknown.

## Weekday study schedule

Monday–Friday, 14:00–15:00 Europe/Berlin.

Default 60-minute session:

1. **10 min — Recall:** reconstruct previous knowledge without notes.
2. **10 min — Map + concept:** show `YOU ARE HERE` in the knowledge graph and teach one focused concept.
3. **30 min — Evidence:** analyze one important paper/experiment or a tightly related evidence set.
4. **10 min — Teach-back + synthesis:** learner explains the new connection; prepare the course summary.

The structure can flex when a paper requires more time, but the learning goal and evidence discipline remain fixed.

## Lesson opening rule

Every lesson starts with:

```text
YOU ARE HERE
Stage -> Topic -> Subtopic -> Today's node
```

Then answer four questions before details:

1. What are we learning today?
2. Why does this node matter?
3. How does it connect to the existing graph?
4. What should the learner be able to explain by the end?

## Paper-selection rule

Do not choose papers randomly or only because they are famous.
For each important topic, aim to cover these evidence roles when available:

- foundational paper;
- strong empirical demonstration;
- replication/extension;
- counter-evidence or qualification;
- modern-model reassessment;
- 2025–2026 frontier work;
- survey/synthesis when useful.

The literature census is broader than the deep-read set. The course deeply reads the papers needed to build the mental model; the census tracks the wider candidate literature.

## Scientific reading rule

For each paper, capture:

- research question;
- models/tasks/data;
- experimental design;
- main result;
- what the result **does prove**;
- what it **does not prove**;
- alternative explanations;
- threats to validity;
- relation to earlier evidence;
- later support/counter-evidence;
- one-sentence memory.

## Completion rule for a lesson

A lesson is complete only when:

- the learner participated;
- the key concept is understood;
- the learner can explain it back in their own words;
- the new node is connected to the existing knowledge graph;
- the scientific summary is recorded.

A missed session does not advance the course.

## Completion rule for a topic

A topic is complete when the learner can explain:

1. what the limitation is;
2. how it manifests;
3. the strongest supporting evidence;
4. important counter-evidence;
5. how the evidence evolved over time;
6. what newer models/methods changed;
7. what remains unresolved;
8. connections to neighboring limitations.

## Completion rule for a stage

Before moving to the next stage:

- all required topics for the stage are covered;
- core paper/evidence maps are populated;
- a stage synthesis exists;
- the learner passes a recall/reconstruction test;
- `COURSE-STATE.md` and `progress.md` are updated.

## GitHub update rule

After each completed lesson, write a concise scientific summary containing only durable course knowledge:

- topic/concept;
- paper/evidence;
- what was learned;
- what the evidence proves;
- what it does not prove;
- one-sentence memory;
- knowledge-graph connections;
- exact next step.

Do not record private conversation details or personal information.

## Long-chat / new-chat continuity protocol

When the current chat becomes too long:

1. ensure `COURSE-STATE.md` is current;
2. ensure the latest lesson summary is committed;
3. ensure the next exact lesson/section is written;
4. start a new chat;
5. the new chat reads, at minimum:
   - `00-course/COURSE-STATE.md`
   - `00-course/COURSE-MANAGEMENT.md`
   - `00-course/MASTER-KNOWLEDGE-GRAPH.md`
   - `00-course/progress.md`
6. continue from the exact next step; do not restart or guess.

## Quality target

The course is finished only when the learner can reconstruct the full limitation map, explain evidence and disagreements, and analyze a new limitation paper independently.
