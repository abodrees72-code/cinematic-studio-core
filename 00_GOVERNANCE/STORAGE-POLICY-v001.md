# STUDIO STORAGE POLICY — v001

Status: ACTIVE

## Purpose
Keep GitHub fast, reviewable, legally safe, and useful as the Studio control layer.

## GitHub stores
- Source code and automation.
- Unreal configuration and small text-based project controls.
- QA gates and reports.
- Research/evidence ledgers.
- Shot and asset manifests.
- Hashes, source URLs, license notes, local-path references, and approval states.
- Small project-neutral documentation.

## GitHub does not store by default
- Large Blender project files.
- Unreal binary asset payloads and maps.
- 4K/8K texture libraries.
- Raw scans, Alembic caches, VDB caches, render sequences, or video masters.
- Marketplace/Fab asset source payloads.
- Any third-party file whose redistribution rights are not explicitly proven.
- Secrets, API keys, tokens, passwords, or private credentials.

## Asset manifest minimum fields
Every external production asset should eventually record:
- asset_id
- canonical_name
- source
- source_url
- license_status
- redistribution_status
- commercial_use_status
- local_storage_reference
- SHA-256 when available
- version
- approved_scope
- historical_or_visual_status when relevant
- notes

## License states
Use only:
- PROVEN
- NEEDS_VERIFICATION
- HOLD
- REJECTED

If redistribution rights are unclear, the asset payload stays out of GitHub.

## Large-file rule
Git LFS is not automatic approval to upload large or licensed files. LFS may be introduced only for assets that are both technically suitable and legally permitted to be stored there.
