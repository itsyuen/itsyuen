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

## Future role of TemporaryDataSSCL — working, review, promote, discard

The intended future role of `TemporaryDataSSCL` is now clearer. It should be the lab's **short-lived collaboration and staging space**, especially for files that need to be edited or exchanged with students or assembled around a bounded activity.

Examples include:

- an Excel workbook being edited with students during active work;
- a workshop registration or attendance sheet;
- a folder used to exchange files for a short project, meeting, or event;
- intermediate administrative or teaching artifacts whose durable value is not yet known.

The intended lifecycle is:

```text
activity begins
      ↓
TemporaryDataSSCL working artifacts
      ↓
collaboration / tallying / exchange / review
      ↓
activity completes
      ↓
what still has continuing value?
      ├→ evidence / reusable knowledge / required record → promote deliberately
      └→ one-time residue with no future value → delete after review
```

`TemporaryDataSSCL` is therefore **not an inbox whose contents are presumed to become archive material**. Temporary artifacts are presumed disposable once their purpose is complete unless there is an identifiable reason to retain them.

Promotion should be selective. A research result may move to the relevant project or retained data area; a genuinely reusable lab resource may move to `SSCLdataRe`; an authoritative institutional record should move to the location required or approved for that record; a useful workshop contact list may be retained only if future reuse is legitimate under the purpose for which the information was collected, applicable consent, and university/privacy requirements.

The general retention principle — preserve the advancement rather than automatically
preserving every temporary carrier — is defined in
[Artifact placement](artifact-placement.md). Here it is applied specifically to
`TemporaryDataSSCL`.

This is a policy direction, not authorization for unattended cleanup. Existing `TemporaryDataSSCL` material should be reviewed before deletion, especially where student information, research evidence, institutional records, or uncertain ownership may be involved.

## Internal NAS boundary — outside-world interface is separate

From this point forward, treat `TemporaryDataSSCL` and `SSCLdataRe` as **internal lab NAS roots**, not as outside-facing publication, workshop, administration, or collaborator portals.

Their roles are intentionally narrow:

```text
TemporaryDataSSCL
→ internal student/Peter collaboration and staging
→ review → promote or discard

SSCLdataRe
→ internal retained lab/research data and reference material
→ keep only when continuing value is identified
```

An outside-world interface should be a **separate layer selected by the actual audience or transaction**, and its exact service remains to be determined. The general rule lives in [artifact placement](artifact-placement.md): an external interface may expose, collect, deliver, or receive material, but it should not automatically become the working home, long-term holder, or archive for the underlying artifacts.

Do not restructure either NAS root around external sharing merely because Synology can technically expose folders. When an external interaction is needed, expose only what the interaction requires through the appropriate interface, then return any resulting durable artifact or evidence to its proper internal owner.

This is a policy boundary, not a claim that every current NAS ACL has been technically re-audited. Access-control details should still be verified when NAS consolidation resumes.

## Historical mappings and proposals

The handover records X: mapped to TemporaryDataSSCL, Y: to homes/peter, and Z: to google-ME, with screenshots redirected to Y:/Screenshots. These were demonstrated at that earlier time; they are not confirmed current home-computer mappings.

Repo-archive, repos, and repo-snapshot were alternative proposals. Automated GitHub-to-NAS snapshots, scheduled pulls, and NAS-root README creation were not demonstrated. The old proposal to replace desktop-tutorial with working predates the newer repository roles documented in the current ontology; it must not be read as proof of today's repository deployment state.

## Planning update — 2026-09-14 cloud-service direction

The Fall 2026 artifact-placement decision changes the **design target**, but it does not authorize any NAS or cloud mutation yet.

The NTUST GApps (`@gapps.ntust.edu.tw`) and ME Google Apps (`@me.ntust.edu.tw`) environments are being retired from daily use. Their mail, Drive content, ownership, sharing, and account dependencies should be treated as migration material. Existing `google-NTUST`, `google-ME`, or related NAS sync relationships are therefore not to be repaired merely to restore historical symmetry. Their contents and sync behavior should first be inspected so that useful or authoritative material can be migrated deliberately.

Microsoft 365 / Work OneDrive remains open as a Fall 2026 experiment. It may retain a useful institutional-service role for Forms, Office collaboration, required sharing, and delivery, but it is not yet declared the universal home for Office documents or for the knowledge system. The broken `ms-NTUST` Documents pairing should therefore remain deferred until its future role and the authoritative copy of the affected files are clear.

The future target is **role-driven synchronization rather than symmetric cloud mirroring**:

```text
cloud account exists
    ≠ repair/create a matching NAS mirror automatically

NAS folder exists
    ≠ create a matching cloud mirror automatically

verified working, collaboration, delivery, or recovery role
    → define an intentional sync relationship
```

This update is planning evidence only. No Google account, NAS folder, Cloud Sync task, or OneDrive folder has been deleted, moved, disabled, or repaired by this decision.

## Future design baseline

Retain the roles of NetBackup, personal home, SSCLdataRe, and TemporaryDataSSCL, but keep their roles distinct. `SSCLdataRe` is an internal retained lab/research data/reference area; `TemporaryDataSSCL` is an internal active collaboration/staging area that should end in a deliberate promote-or-discard decision rather than automatic archiving. Neither root is the outside-world interface. Keep Work OneDrive available during the semester while its actual institutional-service role is tested, and choose any future outside-facing service according to the concrete audience/workflow rather than by forcing the NAS to serve that role. Technical work primarily happens in local Git repositories coordinated through GitHub. Legacy institutional Google workspaces are migration sources rather than future default working homes. Other cloud accounts receive specific roles only when useful.

The user's clean-slate discussion was brainstorming, not permission to wipe NAS. No deletion, folder move, sync change, or backup automation has been performed as part of this documentation work.

## When consolidation resumes

Inspect current task paths, directions, filters, deletion behavior, backups, and the actual ACLs on the internal NAS roots. For Google-backed sync pairs, first identify authoritative material and migration dependencies before deciding whether to preserve, dismantle, or replace the relationship. Resolve the Work OneDrive pairing only when the intended Microsoft role and authoritative copies are clear. Clarify the nested temporary folder, then review `TemporaryDataSSCL` by completed/active purpose: identify what should be promoted, what must be retained for evidence or records, and what can be safely discarded. Do not add an external-sharing layer to `TemporaryDataSSCL` or `SSCLdataRe`; select that interface separately when a real outside-world use case requires it. Apply placement rules to active artifacts first, documenting only the links and procedures that support real work.
