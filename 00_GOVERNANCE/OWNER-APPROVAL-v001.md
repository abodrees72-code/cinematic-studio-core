# OWNER APPROVAL — v001

Status: ACTIVE

## Core rule
No canonical Studio file on the production machines may be modified, overwritten, moved, deleted, re-rigged, re-weighted, re-saved, or replaced without explicit owner approval for that specific write scope.

## GitHub boundary
This repository is a control, versioning, documentation, automation, QA, and manifest layer. It is not authorization to alter canonical local Studio assets.

## Safe-by-default operations
- Read-only inspection.
- New files on isolated branches in this repository.
- Manifests, hashes, QA records, research ledgers, and automation code that do not overwrite canonical production assets.
- Pull requests for review before merge.

## Explicit approval required
- Writes to canonical Studio files.
- Replacing or regenerating approved assets.
- Rig, weights, constraints, topology, or deformation changes.
- Destructive file operations.
- Pushing licensed third-party asset payloads.
- Direct merge to the default branch when a review branch can be used instead.

## Safety rules
- No force push.
- No secrets or credentials in Git.
- No execution from quarantine/intake locations.
- Closed technical gates remain closed unless a concrete defect or new material scope requires reopening.

## Versioning
Use explicit versions such as v001, v002, v003. Do not use final, latest, final-final, or silent rewrites of historical decisions.
