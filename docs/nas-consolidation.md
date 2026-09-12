# NAS Consolidation

[Home](../README.md) · [Ontology](ontology.md) · [Todoist](todoist.md) · [Artifact placement](artifact-placement.md) · [NAS consolidation](nas-consolidation.md)

Record assembled 2026-09-12 from the user's historical handover and current File Station / Cloud Sync screenshots. This is not a live audit of NAS settings.

**Status: sync repair and physical migration deferred.** The [artifact-placement agreement](artifact-placement.md) guides future active work. The earlier NAS-first proposal is preserved verbatim in the [historical blueprint](archive/old-nas-blueprint-2025-09-10.md); its commands and templates are historical material, not a current execution plan.

## Original role

NAS-Peter served as a working filesystem, counterpart for several cloud accounts, personal/institutional storage, controlled SSCL server, and backup/archive location. Cloud-named roots preserve storage origins; they are not ontology categories.

## Access boundaries recorded historically

| Area | Historical purpose and access |
|---|---|
| SSCLdataRe | Curated data/reference area; Peter and NAS Assistant role RW, PhD/MS RO |
| TemporaryDataSSCL | Student collaboration/exchange; Peter, Assistant, PhD/MS RW |
| Cloud-account shares | Peter/Assistant storage, separated from student shares |
| NetBackup | Peter-only backup administrative area |
| homes | User home directories |

The NAS Assistant role does not imply AI access. Current permissions have not been audited. Curation from TemporaryDataSSCL to SSCLdataRe was intended, but no finalized procedure was established.

## Synchronization: history and newer evidence

| Area | Historical record | Newer evidence / remaining uncertainty |
|---|---|---|
| dropbox-Personal | Root bidirectional | Connection shows green; individual current settings not inspected |
| google-Personal | My Drive root bidirectional | Connection shows green; individual current settings not inspected |
| google-NTUST | My Drive root bidirectional | Connection shows green; individual current settings not inspected |
| ms-Personal | Desktop, Documents, Pictures bidirectional | Whole-root coverage not established |
| google-ME | Selected BUdata, LEAT@MIT公開演講授課, Saved from Chrome paths NAS → cloud | Current screenshot confirms /google-ME ↔ remote root, Bidirectional; exclusions not inspected |
| SSCLdataRe → Google-ME/SSCLdata | Separate one-way relationship | Current existence and direction not verified |
| ms-NTUST | Previously blocked by institutional authorization | User confirms Microsoft Taiwan helped establish sync; Desktop task shows Up to date, Documents task needs repair |

Green connection indicators do not prove every task is functioning or bidirectional. Deletion propagation, filters, version retention, and backup coverage remain unverified.

## Work OneDrive rename issue — deferred

The user renamed the Work OneDrive folder from 文件 to 教學文件. Cloud Sync still displays remote /文件 paired with NAS /ms-NTUST/Documents, shows red --, and has Edit disabled. The newest visible log entry was 2026-09-01 09:49:31, recording Delete local file for 2025. NAS Documents differs from the current Dell teaching directory.

The rename is a likely cause, not a confirmed diagnosis. The log does not prove who initiated the deletion or why. Treat NAS Documents as potentially outdated. A fresh download pairing and comparison were discussed but not executed; the user explicitly froze this repair.

## TemporaryDataSSCL nesting

Screenshots show the outer share contains #recycle and another TemporaryDataSSCL folder. The inner folder contains 27 items (20 folders, 7 files), mixing people, research platforms, teaching, reference, reports, and records. Outer modification dates show 2026-09-11; children retain older dates. Who introduced the nesting and whether it resulted from moving or copying are unknown.

## Historical mappings and proposals

The handover records X: mapped to TemporaryDataSSCL, Y: to homes/peter, and Z: to google-ME, with screenshots redirected to Y:/Screenshots. These were demonstrated at that earlier time; they are not confirmed current home-computer mappings.

Repo-archive, repos, and repo-snapshot were alternative proposals. Automated GitHub-to-NAS snapshots, scheduled pulls, and NAS-root README creation were not demonstrated. The old proposal to replace desktop-tutorial with working predates the newer repository roles documented in the current ontology; it must not be read as proof of today's repository deployment state.

## Future design baseline

Retain the roles of NetBackup, Work OneDrive, personal home, SSCLdataRe, and TemporaryDataSSCL. Technical work primarily happens in local Git repositories coordinated through GitHub. Other cloud accounts receive specific roles only when useful.

The user's clean-slate discussion was brainstorming, not permission to wipe NAS. No deletion, folder move, sync change, or backup automation has been performed as part of this documentation work.

## When consolidation resumes

Inspect current task paths, directions, filters, deletion behavior, and backups. Resolve the Work OneDrive pairing while preserving NAS-only work. Clarify the nested temporary folder and curation responsibilities. Apply placement rules to active artifacts first, documenting only the links and procedures that support real work.
