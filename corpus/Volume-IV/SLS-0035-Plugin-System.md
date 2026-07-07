# SLS-0035 Plugin System

Status: Draft
Version: 0.1

## Purpose

This specification defines the plugin posture for Compound.

## v0.1 posture

Plugins are closed internal modules.

Interfaces should be designed as if they may become public, but they are not public commitments yet.

## Plugin classes

Formula providers.
Catalyst adapters.
Assay packs.
Reagents.
Exporters.

## Rule

No plugin may bypass Corpus laws.

Plugins extend Compound. They do not redefine it.
