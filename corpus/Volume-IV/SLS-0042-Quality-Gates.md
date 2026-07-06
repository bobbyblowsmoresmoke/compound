# SLS-0042 Quality Gates

Status: Draft
Version: 0.1

## Purpose

This specification defines gates that protect Compound quality.

## Required gates

Corpus compliance.
Domain invariant tests.
Pipeline tests.
Golden Specimen regression tests.
Assay determinism tests.
Notebook completeness tests.
Offline baseline tests.

## Merge rule

A change that violates a gate must not merge unless the Corpus is intentionally updated first.
