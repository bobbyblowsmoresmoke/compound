# SLS-0002 — Constitution

Status: Accepted  
Version: 1.2  
Authority: Spider Labs Architecture  
Depends On: SLS-0001, SLS-0006

## Purpose

This specification defines the constitutional principles of Spider Labs software.

Every product, specification, build plan, and implementation must comply.

## Constitutional Principle 1 — Single Authority

Authoritative concepts, laws, and contracts each have exactly one home.

Other specifications reference authority instead of redefining it.

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

## Constitutional Principle 2 — Corpus Authority

The Corpus is the authoritative source of architectural truth.

The Corpus defines concepts, laws, contracts, and architectural invariants.

Implementation realizes the Corpus.

Implementation does not redefine the Corpus.

When implementation and the Corpus disagree, one of two conditions exists:

1. The implementation is incorrect and shall be corrected.
2. The Corpus no longer reflects the intended architecture and shall be amended through the Corpus itself.

Architectural change occurs by changing the Corpus.

Code follows the Corpus.

The Corpus does not follow the code.

## Engineering axioms

### AX-001 — Ownership

Users own their work.

### AX-002 — Preservation

Original artifacts are preserved.

### AX-003 — Repeatability

Every refinement is reproducible.

### AX-004 — Human authority

AI is advisory rather than authoritative.

### AX-005 — Interface durability

Interfaces outlive implementations.

### AX-006 — Explainability

Every recommendation must be explainable.

### AX-007 — No hidden state

Hidden state is technical debt.

### AX-008 — Trust over convenience

Trust is more valuable than convenience.

## Domain law references

Catalyst behavior is specified by SLS-0022 and SLS-0037.

Formula behavior is specified by SLS-0021 and SLS-0036.

Specimen behavior is specified by SLS-0020.

Assay behavior is specified by SLS-0023 and SLS-0026.

Notebook behavior is specified by SLS-0025.

Pipeline behavior is specified by SLS-0012 and SLS-0027.
