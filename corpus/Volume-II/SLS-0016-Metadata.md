# SLS-0016 Metadata

Status: Accepted
Version: 1.0
Depends On: SLS-0015

## Purpose

This specification defines metadata expectations for Compound objects.

## Required metadata classes

Identity metadata identifies the object.

Provenance metadata records source and ancestry.

Execution metadata records runtime behavior.

Compatibility metadata declares what an object supports.

Audit metadata records timestamps, versions, and actors where available.

## Unknown metadata

Unknown metadata must be preserved when safe.

Unknown metadata must not silently alter behavior.
