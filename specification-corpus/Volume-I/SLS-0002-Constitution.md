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
