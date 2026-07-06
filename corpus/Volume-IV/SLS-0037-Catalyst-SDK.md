# SLS-0037 Catalyst SDK

Status: Draft
Version: 0.1

## Purpose

This specification defines requirements for Catalyst implementations.

## Initial implementer context

Nemotron Super 3 is expected to implement Compound through Qwen-Code as the coding harness.

This does not change the Catalyst contract.

## Required behavior

Accept a Specimen revision and Formula context.
Return structured suggestions or proposed revision data.
Report execution metadata.
Report errors clearly.
Never mutate the original Specimen.

## Test requirement

A fake deterministic Catalyst must exist before any real provider Catalyst is considered complete.
