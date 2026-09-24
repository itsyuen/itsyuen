# Artifact Placement

[Home](../README.md) · [Ontology](ontology.md) · [Semester cycle](semester-ontology-cycle.md) · [Todoist](todoist.md) · [Artifact placement](artifact-placement.md) · [NAS consolidation](nas-consolidation.md)

Working agreement — 2026-09-12. Updated 2026-09-17 with the living-artifact lifecycle, intention-based splitting rule, semester-turnover connection, clarified AhaSlides audience-facing authority, and the personal procedure for encountering artifacts. Apply to new and active work; this is not a claim that all historical files have been migrated.

## Governing rule

**Intention determines ownership; editing and collaboration determine the working location; preservation determines the backup.**

Give each artifact one authoritative editable home. Record where supporting data, delivery copies, and backups live. A synchronized counterpart is part of the same working arrangement, not an independent master.

Placement does not imply permanent preservation. An artifact may complete its purpose, transfer its useful evidence or decision into a more durable artifact or into the ontology, and then become disposable.

## My relationship with artifacts

Treat an artifact as evidence of an intention, not a demand on attention. Recover the intention and Outcome it served; then decide whether a thought it triggers belongs in current work, later work, or neither.

## Five questions every artifact answers

An artifact can be understood through five independent dimensions. These are not
five maturity levels and do not need to become mandatory metadata on every
small file. They are questions to use when an artifact's ownership, audience,
role, retention, or next use is unclear.

| Dimension | Question | What it clarifies |
|---|---|---|
| **Subject and intention** | Why does this artifact exist, and what work does it currently serve? | Its intellectual owner and authoritative repository or professional world |
| **Audience** | Who should encounter it now? | Privacy, access, language, explanation depth, and whether an audience-facing derivative is needed |
| **Artifact role** | What is it doing now? | Brainstorm, working model, executable implementation, evidence, deliverable, reference, or archive |
| **Supported outcome** | What claim, capability, decision, obligation, or final product does it support? | Why the artifact matters and how it connects to the larger work |
| **Use horizon** | When, or under what condition, will it be used again? | Immediate delivery, semester development, submission, publication, evaluation, uncertain future reuse, or retirement |

The five answers describe the artifact; they do not replace `intention → Outcome → Milestone → Action`. Derive its authoritative home chiefly from primary intention, then account for editing, audience, delivery, and preservation.

## Working locations

| Location | Intended role |
|---|---|
| Local Git repositories | Main technical working area, edited and tested in VS Code, MATLAB/Simulink, and Linux/ROS 2 |
| GitHub | Committed version history and coordination across machines and collaborators; synchronize through deliberate commits, pushes, and pulls |
| Work OneDrive / NTUST OneDrive | Fall 2026 institutional service-layer experiment: Forms, active Office collaboration, institutional sharing/delivery, and records where Microsoft services are genuinely useful; not the default master for Git-suitable technical or teaching source material, and not automatically the home of every Word/Excel/PowerPoint file |
| NAS personal home | Personal files and private working material |
| NAS SSCLdataRe | Internal curated lab resources, large datasets, and retained research material that have an identified continuing value |
| NAS TemporaryDataSSCL | Internal short-lived student/lab collaboration, exchange, and staging. Review when the activity ends: promote material with continuing value and discard material whose purpose is complete |
| NAS NetBackup | Preserved backups and archives; actual coverage and recovery remain to be verified |
| Legacy institutional Google workspaces | Migration/retirement sources rather than new working homes. Existing mail, Drive files, ownership, sharing, and account dependencies should be reviewed and migrated deliberately before the accounts are allowed to become dormant |
| Other cloud drives | Specific sharing or distribution roles where needed, subject to their actual sync configuration; cloud symmetry is not itself a goal |

## Repository ownership

- **learning:** personal technical exploration and capability gaps.
- **working:** intended research/engineering Outcomes, reasoning, implementation, and evidence.
- **teaching:** knowledge curated for a defined subject, audience, and level.

These roles follow the [ontology](ontology.md); storage format alone does not decide ownership. An institutional report can draw from a research result without becoming the owner of that science.

### Learning ↔ teaching boundary

Place an artifact by its current intention. If it is being developed to teach, its unfinished state or the author's learning does not move it out of `teaching`. Move it to `learning` only when the teaching intention is explicitly paused. Avoid parallel editable copies. Some movement is expected while the Fall 2026 course scope settles.

### One authoritative working artifact per active intention

Keep one editable master while the intention remains unified, even if the file is messy. Split it when another intention needs independent work, audience, or cadence. At semester turnover, [Run 1 and Run 2](semester-ontology-cycle.md) can recover, continue, merge, split, or retire the active artifacts. Do not require a wholesale historical migration.

## Examples

- A teaching module's Markdown and code belong in teaching; large videos can remain on NAS with links from the module.
- An actively co-edited Word document can have its master in Work OneDrive. Any Git copy is an intentional snapshot unless Git is explicitly chosen as its editable home.
- A Word/Excel/PowerPoint file does not belong in OneDrive merely because it is an Office file. Its editable home is determined by the actual collaboration, delivery, institutional, or preservation need.
- Research code belongs with its working project; large experiment data can live on NAS, identified from the project README with enough information to locate and interpret it.
- Student contributions can accumulate in TemporaryDataSSCL while work is active. At the end of the activity, reviewed material with continuing value can be promoted to controlled storage or a relevant repository; the remainder can be deleted after its purpose and retention obligations are complete.
- Frozen deliveries and backups preserve identifiable versions only when preservation serves a continuing scientific, teaching, institutional, contractual, legal, or recovery purpose; they should not become competing editable masters.

## Todoist points to artifacts; it does not own them

A task can link to its working artifact for re-entry. The artifact or data holds the evidence; a Todoist comment briefly records the result, present interpretation, and changed next Action. A task's own artifact link does not automatically warrant `reference_link`; use that label when returning to a source is itself the work. See [Todoist](todoist.md#task-links-working-artifacts-and-evidence-comments).

## Audience-facing and delivery surfaces

For Git-suitable intellectual source material, begin and retain the evolving source in the appropriate local Git repository and commit it to GitHub when it is ready to become durable history. Audience-facing services come later; they do not become competing working masters merely because they retain a cloud copy.

- **HackMD** is a late-stage audience-facing reading/presentation interface for stabilized Markdown. It is not the primary working notebook or default collaboration surface.
- **AhaSlides** may be the authoritative **audience-facing slide deck** for a live class. It does not require a mirrored local slide file merely for preservation or symmetry. Private lecture-preparation notes and reusable explanations, figures, code, or teaching modules should remain in the appropriate Git-managed teaching material when they benefit from versioned source control. In that arrangement, AhaSlides owns the live presentation surface while the repo owns the reusable preparation/source artifacts; neither needs to duplicate the other.
- **NTUST / Work OneDrive** remains appropriate for institutional Office documents, records, required submissions, active Office collaboration, Forms-backed workflows, and delivery copies. It does not need to retain a second authoritative copy of Git-suitable source material simply for safekeeping.
- **NAS** increasingly serves internal reference material, datasets, retained artifacts, binaries, collaboration staging, and archival/backup roles that are unsuitable for Git. It should not be required to carry the evolving ontology of active work, nor should temporary NAS work be archived automatically.

These are role boundaries rather than a demand to migrate all historical material immediately.

### Outside-world interfaces

Choose Forms, Office sharing, HackMD, an LMS, website, email, or another service for the actual audience or transaction. Expose only what is needed, then return resulting evidence to its authoritative internal home. An interface does not inherit ownership. `TemporaryDataSSCL` and `SSCLdataRe` remain internal lab spaces, not outside-facing portals.

## Fall 2026 cloud-service consolidation experiment

The cloud decision for this semester is intentionally asymmetric. The goal is not to preserve every historical cloud environment or rebuild matching directory trees across NAS and cloud. The goal is to reduce the number of plausible working homes while observing which external services still earn a real role.

### Institutional Google workspaces — retire from daily use

The NTUST GApps workspace (`@gapps.ntust.edu.tw`) and the ME Google Apps workspace (`@me.ntust.edu.tw`) are no longer intended as active mail, calendar, Drive, or new-artifact homes.

Retirement means:

```text
stop creating new work there
        ↓
inspect mail / Drive / ownership / sharing / Sign-in-with-Google dependencies
        ↓
migrate only material and relationships that still matter
        ↓
leave the old accounts available long enough to discover forgotten dependencies
        ↓
remove them from the daily working environment when migration is sufficiently understood
```

This is not permission to delete the accounts or bulk-delete their contents. Historical Google-backed NAS sync relationships should therefore be treated as migration evidence, not automatically repaired or reproduced for symmetry.

### Microsoft 365 / Work OneDrive — keep open and test

Microsoft 365 and Work OneDrive remain available during Fall 2026 as an **institutional service layer whose boundary will be learned from actual use**. Likely legitimate uses include Forms for workshops or other recipients who should not enter the Git working environment, Office documents that require active institutional collaboration, and university-supported sharing or delivery.

Do not decide in advance that every Office document belongs in OneDrive. A `.docx`, `.xlsx`, or `.pptx` may originate from Git-managed intellectual work, an administrative obligation, teaching delivery, or collaborative editing. The actual role determines its authoritative home.

The working default is therefore:

```text
my evolving intellectual / technical work
        → local Git + GitHub when suitable

external workflow genuinely needs Microsoft service
        → Forms / Word / Excel / PowerPoint / OneDrive as needed

official or sensitive institutional record
        → location required or approved by the university
```

At the Fall 2026 → Spring 2027 boundary, review real cases: which Microsoft services were actually necessary, which artifacts naturally lived there, which could remain in Git, and which required institutional permissions or delivery. Use that evidence to decide whether OneDrive becomes a narrow service layer, a larger institutional workspace, or something in between.

### Sync follows role

A NAS/cloud sync pair needs a real editing, collaboration, delivery, or verified recovery role. An account or directory does not need a matching mirror. Check direction, deletion propagation, filters, versions, and recovery before relying on a sync.

## Temporary artifacts: preserve the advancement, not automatically the carrier

An artifact is not automatically valuable because work happened through it. A spreadsheet, screenshot, temporary Markdown note, registration export, intermediate report, AI-generated comparison, shared student workbook, or exploratory directory may be only the carrier through which a decision, insight, result, or obligation was completed.

The default lifecycle is:

```text
intention / real activity
        ↓
temporary working artifact
        ↓
evidence / insight / decision / completed obligation
        ↓
consolidate what matters into
ontology / research result / teaching material / durable record / next Outcome
        ↓
review the original artifact
        ├→ continuing independent value → promote / retain
        └→ purpose complete, no continuing value → delete
```

**Preserve the advancement, not necessarily the artifact that produced it.** Historical reminiscence — for example, “this reminds me that I once had a good idea” — is not by itself a reason to retain a file when the idea and its consequences have already been consolidated into the current ontology or a stronger artifact.

Retention should have an identifiable reason. Examples include irreplaceable raw or experimental data, reproducibility evidence, publishable or publication-supporting research material, reusable teaching material, an authoritative final deliverable, a contractual/institutional/legal record, or other evidence whose loss would destroy something that cannot be adequately reconstructed from the current system.

### TemporaryDataSSCL as a working and disposal boundary

`TemporaryDataSSCL` is a concrete NAS application of the general lifecycle above:
a short-lived internal working/staging space should end in a deliberate
**promote-or-discard** decision rather than automatic archiving.

Its specific collaboration examples, privacy/retention cautions, current NAS
state, and future consolidation procedure belong in
[NAS consolidation](nas-consolidation.md). This document supplies the general
artifact rule; the NAS record supplies the storage-specific application.

## Artifact placement is time-dependent

Artifact placement should be treated as a **current best interpretation**, not a permanent classification made once and never revisited.

An artifact's content can evolve. Its primary intention can become clearer. The evidence it contains can become more important than originally expected. The tools, collaborators, audience, file format, and delivery obligations around it can also change. Because of this, the most useful working location or intellectual owner may legitimately change through time.

The five artifact questions above should therefore be revisited only as much as
the active work requires. Their answers may change without implying that the
earlier interpretation was careless or wrong.

### A living and forgiving lifecycle

An artifact may be an Outcome in one relationship and evidence in another. Its
role is relational rather than permanently fixed. A published paper is an
Outcome of a research process; later, the same paper becomes evidence in a
tenure-defense presentation. A student assignment is a teaching deliverable;
student responses then become evidence about capability and about whether the
teaching method worked.

The common movement is:

```text
intention
      ↓
working artifact
      ↓
evidence / insight / decision
      ↓
supported Outcome
      ↓
future presentation / reuse / next investigation
```

This is a loop rather than a one-way production line. New evidence can revise
the intended Outcome, change the artifact's role, or create a justified
derivative for a new audience.

For example, the current Computer Integrated Control Systems course can move through:

```text
course intention
      ↓
course_design_brainstorm.md — active weekly thinking and records
      ↓
syllabus.md — slower stabilized course definition
      ↓
lecture preparation notes + reusable teaching modules
      ↓
AhaSlides — authoritative live audience-facing presentation
      ↓
student submissions + in-class observation
      ↓
evidence of actual student capability and teaching-method effectiveness
      ↓
revised course design / assessment
      ↓
semester turnover → historical course record + next active teaching intention
```

A research paper can move through:

```text
research intention
      ↓
derivation notes + code + simulation / experimental records
      ↓
scrutinized evidence
      ↓
paper draft
      ↓
published paper
      ↓
evidence selected for a tenure-defense slide
```

Everything between these examples remains a legitimate artifact: a private
brainstorm, equation, conceptual model, executable prototype, simulation,
experimental record, lecture plan, worked example, student-facing assignment,
student result, internal report, draft, publication, or professional
presentation. Importance does not begin only when the final public product
appears.

This is deliberately forgiving:

- Place an artifact according to today's honest primary intention; it does not
  need to predict its entire future.
- Let audience changes produce deliberate derivatives rather than competing
  editable masters.
- Allow evidence to change the hierarchy, role, or placement.
- Treat movement among `learning`, `teaching`, and `working` as intellectual
  development when the underlying intention genuinely changes, not as proof of
  an earlier mistake.
- Preserve one authoritative editable copy while the work is active.
- Preserve the advancement when a temporary carrier no longer has independent
  value.

During the semester, resolve placement only as much as the active work requires. Do not repeatedly reorganize directories merely because a new interpretation appears. Preserve one authoritative editable copy and enough context to understand the artifact's role while it is active; allow the placement and retention rules to be tested by real cases.

At the semester boundary, Run 1 and Run 2 can review the accumulated cases together with the [semester ontology cycle](semester-ontology-cycle.md). The semester-end result is a **time-stamped placement snapshot and retention decision**, not a declaration that every encountered artifact deserves a permanent home:

> As of this semester, this is the authoritative artifact, this is its primary intention, this is the evidence it presently supports, and this is its best working location — or its useful content has been consolidated and the artifact itself can now be retired.

A later semester may reach a different conclusion without making the earlier placement wrong. When the artifact itself is retained, the earlier state remains useful intellectual and workflow history; when it is deleted, the consolidated advancement should remain legible in the surviving system.

## Artifacts generate evidence, and evidence can change the work

Artifacts do not merely store the output of a pre-existing Outcome. As their contents evolve, they can generate evidence that **supports, weakens, redirects, or expands the hierarchy that produced them**.

The relationship is therefore bidirectional:

```text
desired Outcome
      ↓
work / investigation
      ↓
evolving artifact
      ↓
evidence
      ↓
interpretation
      ├→ supports the current Outcome
      ├→ weakens or changes the current Outcome
      ├→ exposes a research_idea
      ├→ exposes a teaching_idea
      ├→ exposes a #4 capability gap
      ├→ triggers Industry work
      └→ triggers Administration work
      ↓
ontology / Todoist / artifact placement may change
```

The newly generated work does not have to inherit the artifact's original owner. A research artifact can expose a teaching need. A teaching example can reveal a research question. A collaborator's result can expose a #4 capability gap. A technical result can become necessary evidence for a proposal, reimbursement, institutional submission, industrial report, or other Administration / Industry obligation. The source artifact may remain where its primary intention belongs while the newly triggered work is created in the professional world that now owns that obligation.

### Example — one notebook through several meanings

A MATLAB notebook might begin as a personal numerical investigation:

```text
learning / investigation
      ↓
model and simulation become stable enough to support #3 research
      ↓
results become evidence under a #3 Outcome
      ↓
a clearer explanation emerges → teaching_idea
      ↓
the explanation stabilizes → reusable teaching material
      ↓
a comparison / figure survives scrutiny → publishable_material
```

This does not require one physical file to be copied into every world. The authoritative evolving notebook can remain in the location that best fits its current primary intention, while derived figures, explanations, snapshots, teaching modules, or report copies are created deliberately for other purposes.

If the notebook's evidence contradicts the original desired Outcome, that is not a placement failure. The evidence should be allowed to revise the Outcome, produce a new research idea, or expose a different explanation. Artifact organization should preserve that intellectual movement rather than hide it by forcing the file to remain attached to an outdated interpretation.

## Industry / Administration / Finance artifacts as boundary evidence

During Fall 2026, artifacts arising from **Industry Projects, Administration, and Finance should also be treated as evidence for learning the boundaries among those three professional worlds**.

Do not assume that file type determines the answer. A spreadsheet is not automatically Finance; a reimbursement form is not automatically Administration in every surrounding task; an industrial report can contain scientific evidence that still belongs to Research #1–#3; an invoice, approval, contract, purchase record, reimbursement packet, budget sheet, or client deliverable may participate in more than one real-world process.

For the active semester, first preserve the artifact where the work can actually proceed and ask what obligation it is serving now. When useful, keep enough context to reconstruct:

```text
artifact
   ↓
what event / obligation created it?
   ↓
who is the receiver / decision-maker?
   ↓
what result or evidence does it record?
   ↓
what Todoist hierarchy was acting on it?
   ↓
which primary intention appears to own it?
```

Ambiguous cases are useful rather than inconvenient. They show where the current ontology is still weak. Preserve those cases while they are needed to learn the boundary instead of forcing an early rule. Once the boundary or decision has been consolidated, the temporary carrier does not need to be retained unless it has an independent preservation reason.

At the Fall 2026 → Spring 2027 transition, Run 1 should collect representative Industry / Administration / Finance artifact cases and recover what they actually did. Run 2 should compare the recurring patterns and use them to refine the corresponding ontology boundaries for the next semester. Representative evidence may be preserved through conclusions, examples, or durable records rather than by archiving every temporary source file.

The goal is that Spring 2027 begins with **clearer primary-intention rules learned from real artifacts and obligations**, while still allowing future exceptions and evolution.

## Paper-stage integrations — decision frozen until a real case

Do not design the Overleaf or ResearchRabbit workflow in advance. Keep both decisions frozen until an actual `paper_draft` is active enough that the manuscript and literature workflow can be observed in real use.

At that point, decide from the concrete paper what should connect to GitHub, what should remain authoritative, how collaboration should work, and what should return to the Git-managed research record. Until then, Overleaf and ResearchRabbit are neither prerequisites nor active parts of the standard working loop.

## Apply gradually

Start with the next active artifact. Identify its intention, editable home, supporting files, delivery/backup locations, and — when its purpose finishes — whether anything still deserves promotion or preservation. Leave historical material in place until it is deliberately reviewed. A complete migration is not a prerequisite for productive work.

The [NAS consolidation record](nas-consolidation.md) separates current observations from historical configuration and proposals. NAS repair and migration are frozen for now. The policy recognizes deletion as a valid end state for reviewed temporary artifacts, but this document does not by itself authorize deletion of existing NAS material.