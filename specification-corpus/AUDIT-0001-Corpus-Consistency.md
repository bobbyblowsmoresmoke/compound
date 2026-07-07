# AUDIT-0001 — Corpus Consistency Audit

Status: Open  
Version: 0.1  
Authority: Spider Labs Corpus  
Depends On: SLS-0006

## Purpose

This audit verifies that the Corpus behaves like one specification instead of a pile of Markdown files.

## Scope

Review all SLS, AX, and experiment documents in the current specification PR.

## Audit rules

### 1. Single concept authority

Every core concept has one authoritative definition.

Other documents reference the authority instead of redefining it.

### 2. Single law authority

Every normative requirement has exactly one authoritative definition.

Other specifications reference the authoritative definition.

### 3. Single contract authority

Every interface, object, lifecycle state, and pipeline contract has one authoritative source.

### 4. No semantic duplicate requirements

The audit looks for duplicate obligations, not merely duplicate words.

Different wording can still define the same requirement.

### 5. Examples are non-normative

Examples, notes, rationale, and illustrations may clarify requirements but must not create new ones.

### 6. Implementation context stays outside the Corpus

Builder names, current model choices, current harness choices, and temporary execution workflows belong in BUILD-PLAN.md or experiments, not Corpus law.

### 7. Experiments do not create requirements

Experiments may ask questions and propose hypotheses.

They do not define architecture until promoted into a specification.

## Review questions

- Is this concept defined somewhere else?
- Is this law defined somewhere else?
- Is this contract defined somewhere else?
- Is this requirement only a paraphrase of an existing requirement?
- Does this example accidentally create an obligation?
- Does this document mention today's builder, model, language, framework, or harness?
- Could two engineers implement different behavior while both claiming to follow the Corpus?

## Pass condition

The Corpus passes when each concept, law, and contract has one authority and every other occurrence is a reference, example, or rationale.

## Current status

Open.

Architecture freeze is not reached until this audit is complete.
