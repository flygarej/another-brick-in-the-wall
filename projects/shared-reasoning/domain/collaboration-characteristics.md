# LLM Collaboration Characteristics (domain/collaboration-characteristics.md)

## Purpose

Capture accepted observations about long-term collaboration with LLMs and guide future evaluation of collaboration methodologies.

---

## Collaboration Model

The protocol does not primarily optimize individual responses.

It optimizes the collaboration process.

The objective is to improve the quality, continuity, and reproducibility of reasoning across conversations.

---

## Prompt vs Collaboration

The generated bootstrap capsule is not the primary artifact.

The repository is the source of truth.

The capsule is a serialized transport representation generated from:

- protocol
- rationale
- common reasoning
- project state
- domain knowledge

The methodology should therefore be viewed as collaboration engineering rather than prompt engineering.

---

## Observable Behaviour

When the collaboration model is successfully established, interactions tend to shift from:

Question
→ Answer

towards:

Observation
→ Discussion
→ Hypothesis
→ Experiment
→ Verification
→ Accepted knowledge

Uncertainty becomes an explicit part of the reasoning process rather than a failure to answer.

---

## Reasoning Behaviour

The protocol encourages:

- preservation of competing models;
- explicit separation of observation, documentation and inference;
- proposal of discriminating experiments;
- discussion before convergence;
- refinement of abstractions rather than isolated corrections.

This changes the optimization target from producing plausible answers to advancing project understanding.

---

## Evaluation

The protocol should be evaluated by observable collaboration outcomes rather than subjective impressions.

Potential evaluation criteria include:

- project resumability;
- reduction of repeated inference failures;
- preservation of accepted knowledge;
- successful handover between conversations;
- successful handover between language models;
- onboarding time for new collaborators;
- quality of reasoning under uncertainty.

The methodology is intended to be falsifiable through repeated use.

---

## Cross-Model Behaviour

Accepted observation:

Different LLMs exhibit noticeably different collaboration styles when operating under the same protocol.

Current working model:

The protocol exposes behavioural differences that are often hidden during ordinary question-answer interactions.

The underlying causes remain open.

Possible contributing factors include:

- optimization objectives;
- reasoning architecture;
- context handling;
- system-level guidance;
- interaction policies.

Do not promote any particular explanation without supporting evidence.

---

## Evolution

The protocol itself is treated as an engineering artifact.

Observed behaviour should motivate protocol evolution.

The preferred evolution strategy is to introduce abstractions that eliminate classes of reasoning failures rather than adding case-specific rules.

The methodology remains a working model subject to experimental validation.

---

