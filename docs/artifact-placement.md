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
| Work OneDrive | Institutional records and active Office collaboration |
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

## Connections when needed

Connect Overleaf with GitHub for LaTeX manuscript collaboration when an active paper needs it. Bring ResearchRabbit discoveries into the workflow through shared collections or bibliography exports. These integrations are deferred, not prerequisites for starting work.

## Apply gradually

Start with the next active artifact. Identify its intention, editable home, supporting files, and delivery/backup locations. Leave historical material in place until needed. A complete migration is not a prerequisite for productive work.

The [NAS consolidation record](nas-consolidation.md) separates current observations from historical configuration and proposals. NAS repair and migration are frozen for now. No NAS deletion is authorized by this document.
