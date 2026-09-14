# Artifact Placement

[Home](../README.md) · [Ontology](ontology.md) · [Semester cycle](semester-ontology-cycle.md) · [Todoist](todoist.md) · [Artifact placement](artifact-placement.md) · [NAS consolidation](nas-consolidation.md)

Working agreement — 2026-09-12. Apply to new and active work; this is not a claim that all historical files have been migrated.

## Governing rule

**Intention determines ownership; editing and collaboration determine the working location; preservation determines the backup.**

Give each artifact one authoritative editable home. Record where supporting data, delivery copies, and backups live. A synchronized counterpart is part of the same working arrangement, not an independent master.

## Working locations

| Location | Intended role |
|---|---|
| Local Git repositories | Main technical working area, edited and tested in VS Code, MATLAB/Simulink, and Linux/ROS 2 |
| GitHub | Committed version history and coordination across machines and collaborators; synchronize through deliberate commits, pushes, and pulls |
| Work OneDrive / NTUST OneDrive | Institutional records and active Office collaboration or delivery; not the default master for Git-suitable technical or teaching source material |
| NAS personal home | Personal files and private working material |
| NAS SSCLdataRe | Curated lab resources, large datasets, and retained research material |
| NAS TemporaryDataSSCL | Student collaboration, exchange, and work awaiting review |
| NAS NetBackup | Preserved backups and archives; actual coverage and recovery remain to be verified |
| Other cloud drives | Specific sharing or distribution roles where needed, subject to their actual sync configuration |

## Repository ownership

- **learning:** personal technical exploration and capability gaps.
- **working:** intended research/engineering Outcomes, reasoning, implementation, and evidence.
- **teaching:** knowledge curated for a defined subject, audience, and level.

These roles follow the [ontology](ontology.md); storage format alone does not decide ownership. An institutional report can draw from a research result without becoming the owner of that science.

## Examples

- A teaching module's Markdown and code belong in teaching; large videos can remain on NAS with links from the module.
- An actively co-edited Word document can have its master in Work OneDrive. Any Git copy is an intentional snapshot unless Git is explicitly chosen as its editable home.
- Research code belongs with its working project; large experiment data can live on NAS, identified from the project README with enough information to locate and interpret it.
- Student contributions accumulate in TemporaryDataSSCL. Reviewed material can be promoted to controlled storage or a relevant repository through an explicit curation decision.
- Frozen deliveries and backups preserve identifiable versions rather than becoming competing editable masters.

## Todoist points to artifacts; it does not own them

A Todoist task may contain an attachment or link to the artifact through which the work is being carried out. This is often useful because it lets the task act as a re-entry point into the actual working object without moving that object's intellectual ownership into Todoist.

The relationship is:

```text
Todoist hierarchy / task
= intended work

linked or attached artifact
= where the work is actually being developed / observed

artifact result
= evidence

Todoist comment
= concise evidence / decision statement
```

The actual evidence remains in the artifact or associated data: a figure, dataset, notebook, derivation, comparison table, experiment, video, student result, report section, or other working output. A Todoist comment may summarize what that evidence currently means, especially when the result changes the next Action or the interpretation of the Outcome.

This is deliberately lighter than adding `artifact` or `evidence` as Todoist labels. Artifact identity, evidentiary meaning, and placement depend on real results, file format, tool availability, collaboration, and the evolving ontology. They should remain part of the artifact / directory / Markdown reasoning rather than becoming another task taxonomy.

The Todoist `reference_link` label may point to either an **external source** or a **personally created artifact** when consulting, reusing, or returning to that object is itself part of the task. A task's link to its own working artifact does not automatically make the task a `reference_link` task.

For example:

```text
Task: Re-check low-speed friction mismatch
Working artifact: link to MATLAB notebook
Evidence: plots and identified mismatch stored in notebook / data
Todoist comment: mismatch remains concentrated near zero velocity;
                 another static-friction identification experiment is needed
```

When the task is later completed, the link helps locate the artifact and the comment helps reconstruct what the work established. During Run 1, this can make old intention and evidence much easier to recover without turning Todoist itself into the long-form research record.

## Audience-facing and delivery surfaces

For Git-suitable intellectual source material, begin and retain the evolving source in the appropriate local Git repository and commit it to GitHub when it is ready to become durable history. Audience-facing services come later; they do not become competing working masters merely because they retain a cloud copy.

- **HackMD** is a late-stage audience-facing reading/presentation interface for stabilized Markdown. It is not the primary working notebook or default collaboration surface.
- **AhaSlides** is a classroom presentation/delivery surface. The durable source of question text, explanations, figures, code, and other reusable teaching content should remain upstream in the appropriate Git-managed teaching material when practical; the AhaSlides cloud copy is not the intellectual master.
- **NTUST / Work OneDrive** remains appropriate for institutional Office documents, records, required submissions, active Office collaboration, and delivery copies. It does not need to retain a second authoritative copy of Git-suitable source material simply for safekeeping.
- **NAS** increasingly serves large reference material, datasets, frozen artifacts, binaries, and archival/backup roles that are unsuitable for Git. It should not be required to carry the evolving ontology of active work.

These are role boundaries rather than a demand to migrate all historical material immediately.

## Artifact placement is time-dependent

Artifact placement should be treated as a **current best interpretation**, not a permanent classification made once and never revisited.

An artifact's content can evolve. Its primary intention can become clearer. The evidence it contains can become more important than originally expected. The tools, collaborators, audience, file format, and delivery obligations around it can also change. Because of this, the most useful working location or intellectual owner may legitimately change through time.

A file therefore has at least three distinct questions:

```text
What is the artifact now?
What evidence does it currently support?
What is its best present working / ownership location?
```

During the semester, resolve placement only as much as the active work requires. Do not repeatedly reorganize directories merely because a new interpretation appears. Preserve one authoritative editable copy and enough context to understand the artifact's role; allow the placement rules to be tested by real cases.

At the semester boundary, Run 1 and Run 2 can review the accumulated cases together with the [semester ontology cycle](semester-ontology-cycle.md). The semester-end result is a **time-stamped placement snapshot**, not a declaration of a permanent final home:

> As of this semester, this is the authoritative artifact, this is its primary intention, this is the evidence it presently supports, and this is its best working location.

A later semester may reach a different conclusion without making the earlier placement wrong. The earlier state remains useful intellectual and workflow history.

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

## Paper-stage integrations — decision frozen until a real case

Do not design the Overleaf or ResearchRabbit workflow in advance. Keep both decisions frozen until an actual `paper_draft` is active enough that the manuscript and literature workflow can be observed in real use.

At that point, decide from the concrete paper what should connect to GitHub, what should remain authoritative, how collaboration should work, and what should return to the Git-managed research record. Until then, Overleaf and ResearchRabbit are neither prerequisites nor active parts of the standard working loop.

## Apply gradually

Start with the next active artifact. Identify its intention, editable home, supporting files, and delivery/backup locations. Leave historical material in place until needed. A complete migration is not a prerequisite for productive work.

The [NAS consolidation record](nas-consolidation.md) separates current observations from historical configuration and proposals. NAS repair and migration are frozen for now. No NAS deletion is authorized by this document.
