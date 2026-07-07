# SLS-0036 Formula Registry

Status: Draft
Version: 0.1

## Purpose

The Formula Registry resolves Formula identity, compatibility, and versions.

## Responsibilities

List available Formulas.
Resolve Formula by ID and version.
Validate compatibility.
Prevent ambiguous Formula selection.
Record Formula metadata in Notebook entries.

## Rule

Formula lookup must be deterministic.

If multiple Formulas match, Compound must ask for explicit selection or fail clearly.
