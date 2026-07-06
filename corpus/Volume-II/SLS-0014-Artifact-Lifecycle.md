# SLS-0014 Artifact Lifecycle

Status: Accepted
Version: 1.0
Depends On: SLS-0012, SLS-0020

## Purpose

This specification defines the lifecycle states for artifacts moving through Compound.

## Lifecycle

Collected -> Normalized -> Validated -> Refined -> Assayed -> Inspected -> Accepted -> Distilled -> Archived

## State meanings

Collected means raw artifact data has entered Compound.

Normalized means raw data has been converted into a Specimen.

Validated means required invariants have passed.

Refined means a proposed revision has been created.

Assayed means deterministic evaluation has completed.

Inspected means the user or caller has reviewed findings and output.

Accepted means the user or calling workflow accepted the revision.

Distilled means local output artifacts were generated.

Archived means the run was recorded in the Lab Notebook.

## Rule

No stage may skip preservation, provenance, or Notebook recording requirements.
