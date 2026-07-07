# SLS-0025 — Lab Notebook Specification

Status: Accepted  
Version: 1.0  
Authority: Spider Labs Domain  
Depends On: SLS-0002, SLS-0012

## Purpose

This specification defines the Lab Notebook.

## Definition

The Lab Notebook is the permanent experiment history for Compound.

Every pipeline run must create a Notebook entry.

## Required entry data

A Notebook entry must include:

- experiment ID
- timestamp
- input Specimen revision
- output Specimen revision
- Formula ID and version
- Catalyst ID and version
- execution options
- Assay results
- Distillation outputs
- warnings
- errors
- duration

## Reproducibility

A Notebook entry should contain enough metadata to reproduce or replay a run where possible.

## Permanence

Notebook entries must not be silently overwritten.

Corrections require a new entry or explicit revision.

## User value

The Notebook allows the user to answer:

- what changed?
- why did it change?
- when did it change?
- which Formula was used?
- which Catalyst was used?
- what did the Assay find?
- can I reproduce this?

## Format

The initial implementation should prefer local, portable formats.

Markdown and JSON are acceptable first formats.
