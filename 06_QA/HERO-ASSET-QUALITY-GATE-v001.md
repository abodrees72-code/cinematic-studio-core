# HERO ASSET QUALITY GATE v001

Status: Generic studio QA policy. Safe for public repository.

## Purpose
Prevent visually impressive but production-weak assets from entering hero-character work.

## Required gates
Every hero-facing asset must be evaluated on:

1. Visual realism
2. Material fidelity
3. Silhouette readability
4. Deformation / animation compatibility
5. Cloth / collision stability where applicable
6. Integration cost
7. Licensing / redistribution safety
8. Historical or domain plausibility when the project requires it
9. Close-up failure risk
10. Root-cause repairability (no patch-first acceptance)

## Decision states
- PASS: ready for controlled proof-shot use.
- HOLD: promising but needs verification or a root fix.
- REJECT: quality, history, license, or integration risk is too high.
- STOP: unsafe license, accidental sensitive-data exposure, or destructive pipeline risk.

## Hero-specific hard failures
Reject or hold if any of the following are visible in intended camera range:
- clipping
- foot sliding
- finger/prop interpenetration
- unstable cloth jitter
- visibly incorrect material scale
- game-like shading in cinematic framing
- physically weightless weapon handling
- inconsistent LOD behavior
- hidden defects masked only by blur, darkness, smoke, or framing

## Asset-first rule
Prefer one coherent high-quality donor/system over a Frankenstein mix of many unrelated assets. Custom work is reserved for visible differentiation or proven gaps.

## Source-of-truth rule
Third-party source payloads are not stored in this repository unless redistribution is explicitly permitted. Store manifests, source URLs, version identifiers, checksums, and license notes instead.

## Approval boundary
This repository does not authorize modification of canonical local Studio assets. Any such write remains owner-approved work only.
