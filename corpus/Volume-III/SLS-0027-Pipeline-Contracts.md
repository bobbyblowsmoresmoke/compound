# SLS-0027 Pipeline Contracts

Status: Accepted
Version: 1.0

## Purpose

This specification defines the input and output contract for each Compound Pipeline stage.

## Contract rule

Every stage declares input, output, metadata, and failure behavior.

## Stages

Collect accepts raw input and returns collected artifact data.

Normalize accepts collected data and returns a Specimen.

Refine accepts Specimen, Formula, and Catalyst context and returns a proposed Specimen revision.

Assay accepts a Specimen revision and returns Assay results.

Inspect accepts revision plus findings and returns a review package.

Distill accepts accepted revision and returns output artifacts.

Notebook accepts run context and records history.

## Mutation rule

No stage mutates the original Specimen.
