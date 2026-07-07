# SLS-0003 — Domain

Status: Accepted  
Version: 1.0  
Authority: Spider Labs Architecture  
Depends On: SLS-0001, SLS-0002

## Purpose

This specification defines the language of Spider Labs.

Terms are precise. They are not decorative.

## Domain

The domain is **artifact refinement**.

Listings are the first artifact type. Compound must not be designed as if listings are the only possible artifact.

## Specimen

An immutable artifact submitted for refinement.

Examples:

- marketplace listing
- product description
- document
- resume
- article

A Specimen is not a raw JSON blob. Raw input is collected and normalized into a Specimen.

## Formula

A versioned refinement protocol.

A Formula defines how refinement should occur. It does not execute refinement by itself.

## Catalyst

An interchangeable model or provider adapter.

Examples:

- Qwen
- Gemma
- DeepSeek
- GPT
- Claude

A Catalyst is not the source of truth. Business logic does not belong inside a Catalyst.

## Assay

A deterministic evaluation.

Its purpose is diagnosis, not generation.

## Reagent

An adapter connecting Compound to external systems or output formats.

Examples:

- Markdown exporter
- JSON exporter
- eBay export adapter
- Shopify export adapter

Reagents isolate external behavior.

## Lab Notebook

Permanent experiment history.

Every refinement run becomes an auditable Notebook entry.

## Distillation

A refined output produced from a Specimen through one or more Formulas.

## Compound Pipeline

```text
Collect -> Normalize -> Refine -> Assay -> Inspect -> Distill -> Notebook
```
