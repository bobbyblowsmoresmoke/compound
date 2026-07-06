# SLS-0021 — Formula Specification

Status: Accepted  
Version: 1.0  
Authority: Spider Labs Domain  
Depends On: SLS-0003, SLS-0012

## Purpose

This specification defines Formulas.

## Definition

A Formula is a versioned refinement protocol.

It tells Compound how a Specimen should be refined for a domain, platform, style, or goal.

## Required metadata

Every Formula must declare:

- ID
- name
- version
- artifact domain
- compatibility
- input expectations
- output expectations
- author or source
- status

## Immutability

Released Formula versions are immutable.

Formula changes require a new version.

## Compatibility

A Formula must declare what it supports.

Examples:

- listings
- eBay-style listing output
- vintage clothing
- electronics
- collectibles

## Prompt storage

Prompts are Formula content, not hardcoded application logic.

A future implementation may store Formulas as TOML plus Markdown, JSON, or another portable format.

## Determinism

Formula selection and validation must be deterministic.

Catalyst output may vary, but the Formula used must always be recorded.
