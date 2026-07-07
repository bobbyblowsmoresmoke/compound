# SLS-0024 — Reagent Specification

Status: Accepted  
Version: 1.0  
Authority: Spider Labs Domain  
Depends On: SLS-0003, SLS-0011

## Purpose

This specification defines Reagents.

## Definition

A Reagent is an adapter that connects Compound to a specific external format, platform, export target, or integration boundary.

## Core rule

Marketplace behavior belongs in Reagents, not core.

## Initial Reagents

Compound v0.1 should include local export Reagents:

- Markdown
- JSON
- plain text

Marketplace Reagents are future work.

## Responsibilities

A Reagent may:

- export a Distillation
- validate target-specific required fields
- package output for a platform
- generate local handoff files

A Reagent must:

- declare compatibility
- preserve provenance
- avoid mutating Specimens
- record output metadata

## Forbidden behavior

A Reagent must not:

- bypass Assays
- auto-submit listings
- hide platform-specific failures
- introduce marketplace logic into core

## Future compatibility

A future eBay, Etsy, Shopify, TikTok, or Facebook Marketplace Reagent must be additive.

Adding one must not require changing core architecture.
