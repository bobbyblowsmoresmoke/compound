# SLS-0030 — CLI Specification

Status: Draft  
Version: 0.1  
Authority: Spider Labs Product Engineering  
Depends On: SLS-0012

## Purpose

This specification defines the initial Compound command-line interface.

## Principle

The CLI is a thin interface over the core refinement engine.

Business logic must not live in CLI handlers.

## Initial commands

```text
compound init
compound refine
compound inspect
compound assay
compound distill
compound notebook
compound formula list
compound catalyst list
compound doctor
```

## Command philosophy

Commands should be understandable without knowing the internal lore.

The laboratory theme may appear in output, but commands must remain practical.

## Example flow

```text
compound init
compound refine samples/jacket.json --formula formula/listing/ebay-standard
compound inspect output/latest
compound distill output/latest --format markdown
compound notebook show latest
```

## Output tone

Output should be minimal, confident, and inspectable.

Example:

```text
Spider Labs :: Compound

Specimen collected.
Formula loaded: ebay-standard@0.1.0
Catalyst: qwen
Assay: PASS
Purity: 92%

Output written to output/CMP-0001/
Notebook entry recorded.
```

## Failure output

Failures should be useful.

Example:

```text
Assay failed.

Finding:
Missing shipping information.

Recommendation:
Add handling time, shipping method, and return policy before distillation.
```
