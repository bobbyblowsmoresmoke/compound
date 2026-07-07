# SLS-0002 — Constitution

Status: Accepted  
Version: 1.1  
Authority: Spider Labs Architecture  
Depends On: SLS-0001, SLS-0006

## Purpose

This specification defines the constitutional principles of Spider Labs software.

Every product, specification, build plan, and implementation must comply.

## Corpus authority

The Corpus is the authoritative source of architectural truth.

When implementation and the Corpus disagree, the implementation is incorrect or the Corpus must be formally amended.

Implementation shall not redefine architecture.

Architecture evolves through the Corpus, not through code.

## Single authority principles

### Single Concept Authority

Every core concept has exactly one authoritative definition.

Concepts define meaning.

### Single Law Authority

Every normative requirement has exactly one authoritative definition.

Normative requirements are defined once.

Normative requirements may be referenced many times.

Normative requirements shall not be independently restated, paraphrased, or redefined.

Dependent specifications shall reference the authoritative definition.

Laws define obligations.

### Single Contract Authority

Every contract has exactly one authoritative definition.

Contracts define interaction.

## Engineering axioms

### AX-001 — Ownership

Users own their work.

Always.

### AX-002 — Preservation

Original artifacts are never mutated.

### AX-003 — Repeatability

Every refinement is reproducible.

### AX-004 — Human authority

AI is advisory.

Never authoritative.

### AX-005 — Interface durability

Interfaces outlive implementations.

### AX-006 — Explainability

Every recommendation must be explainable.

### AX-007 — No hidden state

Hidden state is technical debt.

### AX-008 — Trust over convenience

Trust is more valuable than convenience.

## Catalyst laws

A Catalyst:

- may suggest
- may transform
- may annotate
- must explain
- must report execution metadata
- must preserve provenance
- must expose uncertainty
- must never mutate the original Specimen

## Formula laws

A Formula:

- is versioned
- is deterministic where possible
- is immutable after release
- is inspectable
- declares compatibility

## Specimen laws

A Specimen:

- has identity
- has provenance
- has revisions
- has timestamps
- is immutable

## Assay laws

An Assay:

- diagnoses
- never flatters
- never hides defects
- cites findings
- recommends improvement
- remains deterministic

## Notebook laws

Every experiment:

- is recorded
- can be replayed
- can be audited
- can be reproduced
