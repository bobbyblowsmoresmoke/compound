# SLS-0020 — Specimen Specification

Status: Accepted  
Version: 1.0  
Authority: Spider Labs Domain  
Depends On: SLS-0003, SLS-0011

## Purpose

This specification defines the Specimen domain object.

## Definition

A Specimen is an immutable artifact under refinement.

## Required properties

A Specimen must have:

- stable identity
- revision identifier
- artifact domain
- source provenance
- created timestamp
- content payload
- metadata

## Immutability

A Specimen revision must never be mutated.

Any refinement creates a new revision linked to the prior revision.

## Provenance

A Specimen must preserve where it came from.

Examples:

- user-supplied JSON
- imported Markdown
- image folder
- manually entered text

## Listing Specimen fields

The initial listing domain should support:

- title
- description
- price
- category
- condition
- brand
- material
- color
- size
- dimensions
- weight
- shipping information
- return policy
- image references
- tags
- notes

## Original vs suggested data

Compound must distinguish:

- original user data
- observed facts
- generated suggestions
- accepted changes
- final output

Generated suggestions must not be presented as original facts.
