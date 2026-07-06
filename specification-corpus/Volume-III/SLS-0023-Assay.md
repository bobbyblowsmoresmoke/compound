# SLS-0023 — Assay Specification

Status: Accepted  
Version: 1.0  
Authority: Spider Labs Domain  
Depends On: SLS-0002, SLS-0003, SLS-0020

## Purpose

This specification defines Assays.

## Definition

An Assay is a deterministic evaluation of a Specimen or refined output.

Its job is diagnosis, not praise.

## Assay categories

The initial listing domain should evaluate:

- identity
- completeness
- search optimization
- trust signals
- marketplace fit
- readability
- visual readiness
- commercial quality

## Example findings

Assays should detect:

- missing shipping information
- missing dimensions
- missing weight
- missing material
- missing brand
- missing condition details
- weak title
- weak opening sentence
- poor keyword coverage
- unclear return policy
- missing image references
- price ambiguity

## Scoring

Scores must explain themselves.

No score may exist without findings.

Suggested first scores:

- Quality
- Completeness
- Trust
- SEO
- Marketplace Fit
- Purity

## Purity

Purity is a branded metric that must map to real validation.

It should represent the percentage of required and recommended fields that pass deterministic checks.

## Output contract

An Assay result must include:

- overall status
- score breakdown
- findings
- severity
- recommendations
- inspected Specimen revision
- Formula context where relevant

## Failure mode

If an Assay cannot evaluate a field, it must report that limitation.

It must not guess.
