# QWEN BUILD PLAN

Implementer: Nemotron Super 3
Harness: Qwen-Code
Repository: bobbyblowsmoresmoke/compound

## Prime directive

Implement the Corpus.

Do not invent architecture.

If a design question is not answered by the Corpus, create an experiment or stop for architectural review.

## Required reading order

1. corpus/Volume-0
2. corpus/Volume-I
3. corpus/Volume-II
4. corpus/Volume-III
5. corpus/Volume-IV
6. corpus/Volume-V
7. experiments

## Phase 0 Repository scaffold

Create the project layout authorized by SLS-0050.

Add package metadata, test framework, formatter, linter, and local development commands.

Stop condition: repo installs locally and tests can run.

## Phase 1 Domain model

Implement Specimen, Formula, Catalyst, Assay, Finding, Reagent, Distillation, and Notebook entry contracts.

Stop condition: domain invariant tests pass.

## Phase 2 Pipeline

Implement Collect, Normalize, Refine, Assay, Inspect, Distill, Notebook stages.

Stop condition: fake deterministic Catalyst can complete a full pipeline run.

## Phase 3 Formula system

Implement Formula loading, validation, compatibility, and registry behavior.

Stop condition: Formula lookup is deterministic and ambiguity fails clearly.

## Phase 4 Catalyst system

Implement fake deterministic Catalyst first.

Then implement Qwen-compatible Catalyst only after the fake Catalyst passes contract tests.

Stop condition: real Catalyst never mutates original Specimen and records metadata.

## Phase 5 Assay engine

Implement listing-domain Assays for missing dimensions, missing shipping information, missing trust signals, weak title, weak description, and incomplete metadata.

Stop condition: Golden Specimen Assays are deterministic.

## Phase 6 Distillation and Notebook

Implement Markdown, JSON, and plain text outputs.

Every run must produce a Notebook entry.

Stop condition: no output can be produced without provenance.

## Phase 7 CLI

Implement compound init, refine, inspect, assay, distill, notebook, formula list, catalyst list, doctor.

Stop condition: CLI smoke test completes local pipeline run.

## Phase 8 Golden Specimens

Add initial fixtures for fashion, electronics, books, collectibles, automotive, and household.

Stop condition: regression suite passes.

## Hard prohibitions

Do not build browser automation.

Do not build marketplace login.

Do not add telemetry.

Do not make cloud required.

Do not mutate original Specimens.

Do not hide Catalyst uncertainty.

Do not put marketplace-specific logic in core.

## Output expectation

Open a draft PR with implementation notes, tests run, Corpus references, and any experiments created.
