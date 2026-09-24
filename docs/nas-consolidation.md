# NAS Consolidation

[Home](../README.md) · [Ontology](ontology.md) · [Todoist](todoist.md) · [Artifact placement](artifact-placement.md) · [NAS consolidation](nas-consolidation.md)

Record assembled 2026-09-12 from the user's historical handover and current File Station / Cloud Sync screenshots. Updated 2026-09-14 with the temporary-artifact lifecycle and internal/external boundary. This is not a live audit of NAS settings.

**Status: sync repair and physical migration deferred.** The [artifact-placement agreement](artifact-placement.md) guides future active work. An earlier NAS-first design was explored in 2025, but it is now superseded; its details remain recoverable through Git history rather than being kept as active guidance in the current tree.

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

## Future role of TemporaryDataSSCL

Use `TemporaryDataSSCL` for short-lived internal student/lab collaboration and staging: shared workbooks, event lists, exchanges, and intermediate artifacts. At the end of an activity, review each item: promote research evidence, reusable resources, or required records to their proper homes; discard residue whose purpose is complete. Retain personal data only for legitimate reuse under applicable consent and institutional requirements. This is a policy direction, not authorization for unattended deletion. See [Artifact placement](artifact-placement.md#temporary-artifacts-preserve-the-advancement-not-automatically-the-carrier).

## Internal NAS boundary

`TemporaryDataSSCL` and `SSCLdataRe` are internal lab roots, not public or outside-collaborator portals. Choose an external interface for the actual audience, expose only what is needed, and return durable results to their internal owner. Current ACLs remain unaudited. See [Artifact placement](artifact-placement.md#outside-world-interfaces).

## Historical mappings and proposals

The handover records X: mapped to TemporaryDataSSCL, Y: to homes/peter, and Z: to google-ME, with screenshots redirected to Y:/Screenshots. These were demonstrated at that earlier time; they are not confirmed current home-computer mappings.

Repo-archive, repos, and repo-snapshot were alternative proposals. Automated GitHub-to-NAS snapshots, scheduled pulls, and NAS-root README creation were not demonstrated. The old proposal to replace desktop-tutorial with working predates the newer repository roles documented in the current ontology; it must not be read as proof of today's repository deployment state.

## Planning update — 2026-09-14

The institutional Google workspaces are retirement/migration sources, not future default working homes. Do not repair their NAS sync pairs for visual symmetry. Work OneDrive remains a Fall 2026 institutional-service experiment; the broken Documents pairing stays deferred until its role and authoritative copies are clear. Future sync must serve a verified working, collaboration, delivery, or recovery need. No account, folder, or sync task was changed by this policy decision. Technical work primarily lives in local Git repositories coordinated through GitHub.

## When consolidation resumes

Inspect current task paths, directions, filters, deletion behavior, backups, and the actual ACLs on the internal NAS roots. For Google-backed sync pairs, first identify authoritative material and migration dependencies before deciding whether to preserve, dismantle, or replace the relationship. Resolve the Work OneDrive pairing only when the intended Microsoft role and authoritative copies are clear. Clarify the nested temporary folder, then review `TemporaryDataSSCL` by completed/active purpose: identify what should be promoted, what must be retained for evidence or records, and what can be safely discarded. Do not add an external-sharing layer to `TemporaryDataSSCL` or `SSCLdataRe`; select that interface separately when a real outside-world use case requires it. Apply placement rules to active artifacts first, documenting only the links and procedures that support real work.
