# SLS-0022 — Catalyst Specification

Status: Accepted  
Version: 1.0  
Authority: Spider Labs Domain  
Depends On: SLS-0002, SLS-0003

## Purpose

This specification defines Catalysts.

## Definition

A Catalyst is an interchangeable execution adapter that assists refinement.

A Catalyst may be an LLM, local model, cloud model, rule-based transformer, or future provider.

## Core rule

A Catalyst never mutates the original Specimen.

## Responsibilities

A Catalyst may:

- generate suggestions
- transform proposed content
- annotate uncertainty
- return structured outputs

A Catalyst must:

- report provider/model metadata
- report execution options
- report timing metadata
- preserve provenance
- expose uncertainty where possible

## Forbidden behavior

A Catalyst must not:

- own business logic
- make final user decisions
- silently discard source data
- hide uncertainty
- bypass Assays
- produce unrecorded outputs

## Catalyst independence

The Compound Pipeline must not care which Catalyst is active.

Adding Qwen, Gemma, DeepSeek, GPT, Claude, or future models must not require changing core pipeline architecture.
