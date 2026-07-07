# SLS-0006 — Reference Law

Status: Accepted  
Version: 1.1  
Authority: Spider Labs Corpus  
Depends On: SLS-0002, SLS-0018

## Purpose

This specification defines how the Corpus prevents duplicate laws, duplicate contracts, and duplicate concept definitions.

## Core law

Every authoritative architectural element has exactly one home.

Every normative requirement has exactly one authoritative definition.

Other specifications reference the authoritative definition.

## Authority classes

### Concept authority

Concepts define meaning.

Every core concept has exactly one authoritative definition.

### Law authority

Laws define obligations.

Every normative requirement has exactly one authoritative definition.

### Contract authority

Contracts define interaction.

Every interface, object contract, pipeline contract, and lifecycle contract has exactly one authoritative definition.

## Normative language

Normative language creates obligations.

Normative terms include:

- must
- must not
- shall
- shall not
- required
- prohibited

## Informative language

Informative language explains, illustrates, or motivates.

Informative terms include:

- example
- note
- rationale
- discussion
- motivation
- illustration

Informative language does not create architectural requirements.

## Reference-first rule

Before introducing a new normative statement, an author must determine whether an authoritative requirement already exists.

If an applicable requirement exists, the specification must reference that requirement instead of restating it.

A new normative statement may be introduced only when it establishes a new architectural requirement.

## Duplicate requirement rule

Duplicate words are not the issue.

Duplicate requirements are the issue.

The Corpus audits semantic duplication, not only repeated wording.

## Review test

If two different specifications could be read as independently defining the same obligation, the Corpus is inconsistent until one definition becomes authoritative and the other becomes a reference.
