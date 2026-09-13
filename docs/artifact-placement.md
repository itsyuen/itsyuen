# Artifact Placement

[Home](../README.md) · [Ontology](ontology.md) · [Todoist](todoist.md) · [Artifact placement](artifact-placement.md) · [NAS consolidation](nas-consolidation.md)

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

## Audience-facing and delivery surfaces

For Git-suitable intellectual source material, begin and retain the evolving source in the appropriate local Git repository and commit it to GitHub when it is ready to become durable history. Audience-facing services come later; they do not become competing working masters merely because they retain a cloud copy.

- **HackMD** is a late-stage audience-facing reading/presentation interface for stabilized Markdown. It is not the primary working notebook or default collaboration surface.
- **AhaSlides** is a classroom presentation/delivery surface. The durable source of question text, explanations, figures, code, and other reusable teaching content should remain upstream in the appropriate Git-managed teaching material when practical; the AhaSlides cloud copy is not the intellectual master.
- **NTUST / Work OneDrive** remains appropriate for institutional Office documents, records, required submissions, active Office collaboration, and delivery copies. It does not need to retain a second authoritative copy of Git-suitable source material simply for safekeeping.
- **NAS** increasingly serves large reference material, datasets, frozen artifacts, binaries, and archival/backup roles that are unsuitable for Git. It should not be required to carry the evolving ontology of active work.

These are role boundaries rather than a demand to migrate all historical material immediately.

## Paper-stage integrations — decision frozen until a real case

Do not design the Overleaf or ResearchRabbit workflow in advance. Keep both decisions frozen until an actual `paper_draft` is active enough that the manuscript and literature workflow can be observed in real use.

At that point, decide from the concrete paper what should connect to GitHub, what should remain authoritative, how collaboration should work, and what should return to the Git-managed research record. Until then, Overleaf and ResearchRabbit are neither prerequisites nor active parts of the standard working loop.

## Apply gradually

Start with the next active artifact. Identify its intention, editable home, supporting files, and delivery/backup locations. Leave historical material in place until needed. A complete migration is not a prerequisite for productive work.

The [NAS consolidation record](nas-consolidation.md) separates current observations from historical configuration and proposals. NAS repair and migration are frozen for now. No NAS deletion is authorized by this document.
