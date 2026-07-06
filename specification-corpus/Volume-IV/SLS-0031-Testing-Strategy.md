# SLS-0031 — Testing Strategy

Status: Draft  
Version: 0.1  
Authority: Spider Labs Engineering  
Depends On: SLS-0013

## Purpose

This specification defines the testing strategy for Compound.

## Testing goals

Tests must protect:

- Specimen immutability
- Formula versioning
- Catalyst independence
- Assay determinism
- Notebook recording
- local-first behavior

## Golden Specimens

Compound must maintain a golden specimen suite.

Suggested categories:

- fashion
- electronics
- books
- collectibles
- automotive
- household

Golden Specimens are stable fixtures used to detect refinement regressions.

## Required test classes

### Domain tests

Validate domain invariants.

### Pipeline tests

Validate stage ordering, failure behavior, and metadata recording.

### Formula tests

Validate Formula loading, versioning, and compatibility checks.

### Catalyst tests

Validate contract compliance with fake and real Catalysts.

### Assay tests

Validate deterministic findings and scores.

### Notebook tests

Validate that every run records required metadata.

## Regression rule

If a golden specimen produces worse deterministic Assay results after a change, the build must flag the regression.

## No-network baseline

The core test suite must pass without network access.
