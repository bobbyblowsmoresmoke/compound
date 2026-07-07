# SLS-0037 Catalyst SDK

Status: Draft
Version: 0.1

## Purpose

This specification defines requirements for Catalyst implementations.

## Corpus boundary

Catalyst behavior is architecture.

Builder identity is not architecture.

The Corpus defines what Catalyst implementations must do, not which tool or agent builds them.

## Required behavior

Accept a Specimen revision and Formula context.

Return structured suggestions or proposed revision data.

Report execution metadata.

Report errors clearly.

Never mutate the original Specimen.

## Test requirement

A fake deterministic Catalyst must exist before any real provider Catalyst is considered complete.
