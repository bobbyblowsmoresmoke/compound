# SLS-0032 — Security and Privacy

Status: Draft  
Version: 0.1  
Authority: Spider Labs Engineering  
Depends On: SLS-0002

## Purpose

This specification defines security and privacy expectations for Compound.

## Local-first rule

Compound must function locally.

Cloud services are optional and must be explicit.

## Data ownership

User data belongs to the user.

Compound must not require uploading listings, images, Notebook entries, or Formula data to Spider Labs infrastructure.

## Telemetry

No telemetry in v0.1.

Future telemetry, if ever introduced, must be opt-in and documented.

## Secrets

Secrets must not be stored in source-controlled files.

Catalyst provider credentials must use explicit local configuration or environment-level secret management.

## Network behavior

Network calls must be explicit.

A user should be able to understand when Compound is calling a model provider or external system.

## Sensitive artifacts

Compound may process product data, images, notes, and seller metadata.

These artifacts must be treated as user-owned private data.

## Failure rule

Security failures must fail closed.

Do not silently fall back to unsafe behavior.
