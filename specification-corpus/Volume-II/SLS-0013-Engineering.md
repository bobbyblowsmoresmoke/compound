# SLS-0013 — Engineering

Status: Accepted  
Version: 1.0  
Authority: Spider Labs Engineering  
Depends On: SLS-0002, SLS-0011

## Purpose

This specification defines how Compound should be engineered.

## Engineering principles

- Prefer boring correctness over cleverness.
- Prefer explicit contracts over implicit behavior.
- Prefer composition over inheritance.
- Prefer deterministic behavior where possible.
- Prefer local-first operation.
- Prefer testable modules.
- Prefer explainable failures.

## Code standards

Every implementation must support:

- automated tests
- static analysis where available
- clear module boundaries
- documented public interfaces
- deterministic core behavior

## Hidden state

Hidden state is forbidden in core logic.

Acceptable state must be explicit, serializable, and inspectable.

## Dependency policy

Core dependencies must be minimal.

Provider SDKs, marketplace integrations, and UI-specific dependencies belong outside the core.

## Review gate

Every change must answer:

- Does this improve refinement?
- Does this preserve ownership?
- Is it deterministic where possible?
- Does this belong in core or a Reagent?
- Can it be explained?
- Can it be reproduced?

## Technical debt policy

Technical debt may be accepted only when it is:

- explicit
- documented
- scoped
- reversible

Undocumented debt is not debt.

It is decay.
