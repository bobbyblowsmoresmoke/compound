# SLS-0023 — Assay Specification

Status: Accepted  
Version: 1.1  
Authority: Spider Labs Domain  
Depends On: SLS-0002, SLS-0003, SLS-0020, SLS-0026

## Purpose

This specification defines Assays.

## Definition

An Assay is a deterministic evaluation of a Specimen or refined output.

Its job is diagnosis, not praise.

## Invariant

Assays must be deterministic, reproducible, and inspectable.

The same Specimen revision, Formula context, Assay definition, and Assay configuration must produce the same result.

## Assessment status

Every Assay result must produce an assessment status.

Valid statuses are:

- Pass
- Warn
- Fail
- Blocked

Pass means required checks were satisfied.

Warn means the artifact is usable but has recommended improvements.

Fail means one or more required checks failed.

Blocked means evaluation cannot complete because required inputs or execution conditions are missing.

The status must be derived from Findings.

The status must be explainable.

The status must not replace Findings.

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

If an Assay computes a score, the scoring method must be deterministic, reproducible, and recorded.

The Corpus does not freeze category weights.

Weight selection is an experimental or Formula-level decision until evidence promotes a model into specification.

Suggested first scores:

- Quality
- Completeness
- Trust
- SEO
- Marketplace Fit
- Purity

## Purity

Purity is a branded metric that must map to real validation.

It should represent the percentage of required and recommended checks that pass deterministic validation.

## Output contract

An Assay result must include:

- assessment status
- score breakdown when scoring is used
- findings
- severity
- recommendations
- inspected Specimen revision
- Formula context where relevant
- Assay configuration where scoring is used

## Failure mode

If an Assay cannot evaluate a field, it must report that limitation.

It must not guess.
