# SLS-0040 Observability

Status: Draft
Version: 0.1

## Purpose

This specification defines local observability expectations.

## Rule

Observability exists to help users inspect and reproduce refinement.

It is not telemetry.

## Required local records

Pipeline run metadata.
Catalyst execution metadata.
Assay findings.
Errors and warnings.
Distillation outputs.
Notebook entries.

## Forbidden behavior

Compound must not send observability data to remote services in v0.1.
