# SLS-0012 — Compound Pipeline

Status: Accepted  
Version: 1.0  
Authority: Spider Labs Architecture  
Depends On: SLS-0011

## Purpose

This specification defines the Compound Pipeline.

The pipeline is the canonical flow through which artifacts are refined.

## Pipeline

```text
Collect -> Normalize -> Refine -> Assay -> Inspect -> Distill -> Notebook
```

## Stage responsibilities

### Collect

Accept raw user-provided artifact data.

Collection may receive JSON, Markdown, text, images, folders, or future formats.

Collection does not refine.

### Normalize

Convert raw collected data into a valid Specimen.

Normalization is deterministic.

Normalization does not call a Catalyst.

### Refine

Apply a Formula through a Catalyst to create a proposed refined Specimen revision.

Refinement is advisory and must preserve the original.

### Assay

Evaluate the Specimen through deterministic findings.

Assay results must explain every score.

### Inspect

Present changes, findings, provenance, and output previews for review.

Inspection must make manual review easy.

### Distill

Generate local outputs.

Distillation may produce Markdown, JSON, plain text, or future marketplace-specific packages.

### Notebook

Record the experiment permanently.

A run without a Notebook entry is incomplete.

## Stage contracts

Each stage must declare:

- input type
- output type
- failure modes
- metadata produced
- whether it mutates state

## Mutation rule

Pipeline stages must not mutate the original Specimen.

New revisions must be explicit.

## Repeatability rule

The pipeline must record enough metadata to reproduce a run where possible.

Required metadata includes:

- Formula ID
- Formula version
- Catalyst ID
- Catalyst version or model identifier
- execution options
- timestamp
- input Specimen revision
- output Specimen revision
- Assay results
