# SLS-0011 — Architecture

Status: Accepted  
Version: 1.0  
Authority: Spider Labs Architecture  
Depends On: SLS-0001, SLS-0002, SLS-0003, SLS-0010

## Purpose

This specification defines the architecture of Compound without binding it to a specific programming language.

## Architectural posture

Compound is a refinement engine.

Listings are the first artifact domain.

The core must remain independent of marketplaces, model providers, and user interface surfaces.

## Primary architectural rule

Core modules communicate through domain objects and contracts, not raw dictionaries or provider-specific payloads.

## Core object

The core object is the Specimen.

Every subsystem receives a Specimen or a formal result object derived from one.

Every refinement produces a new revision. The original is preserved.

## Layers

### Domain layer

Defines durable concepts:

- Specimen
- Formula
- Catalyst
- Assay
- Reagent
- Notebook Entry

### Pipeline layer

Coordinates stages without containing business logic.

### Formula layer

Loads and validates versioned refinement protocols.

### Catalyst layer

Executes advisory model transformations through replaceable adapters.

### Assay layer

Runs deterministic quality diagnosis.

### Reagent layer

Handles exports and external-format behavior.

### Interface layer

Provides CLI and future user surfaces.

## Dependency direction

Outer layers may depend on inner layers.

Inner layers must not depend on outer layers.

The core must not know about:

- eBay
- Shopify
- Etsy
- Playwright
- browser sessions
- provider SDKs
- network-only services

## Error philosophy

Compound should fail clearly.

Silent failure is forbidden.

Every failure should include:

- what failed
- why it failed
- what can be inspected
- what the user can do next

## Architectural smell list

Avoid:

- mutable Specimens
- hidden global state
- marketplace logic in core
- Catalyst-specific branching in the pipeline
- unversioned Formulas
- unverifiable scores
- outputs without Notebook entries
