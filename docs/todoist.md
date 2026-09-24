# Todoist and Actionable Work

[Home](../README.md) · [Ontology](ontology.md) · [Notebook system](notebook-system.md) · [Semester cycle](semester-ontology-cycle.md) · [Todoist](todoist.md) · [Artifact placement](artifact-placement.md) · [NAS consolidation](nas-consolidation.md)

This operating method applies the [professional ontology](ontology.md). Intellectual ownership follows intention; Todoist exposes work that benefits from re-entry, assignment, or future execution. Private upstream reasoning can begin in the [notebook system](notebook-system.md), where intention and Outcome are observed before Milestone/artifact/evidence possibilities are developed into technical Action.

# Todoist: Actionable Operating System

Todoist is used as a **living realization system**, not merely a task list.

Hierarchy answers:

> **Where is this work going, and what are we committed to accomplishing?**

Labels answer:

> **What kind of intellectual work/object is this right now?**

Assignment answers:

> **Who actually has to do or demonstrate it?**

For research work, the task hierarchy should still be traceable to the relevant research world or scientific responsibility, but Todoist does not need to reproduce the full research coordinate.

Together these cues allow immature ideas to remain forgiving while still creating accountable execution when the work becomes mature enough.

## Current personal use — keep Todoist lean

Todoist is Peter's personal action and re-entry surface. Read each live task as “I need to …”; recover the intention behind old student or collaborator wording, then keep only Peter's current action, decision, delegation, or revisit need. Empty coordinates are allowed: the durable ontology lives in Markdown. If Todoist becomes a team surface, add structure only where shared ownership requires it.

## Calendar relationship

The detailed calendar/intention model belongs in the [notebook system](notebook-system.md). Todoist owns the **concrete Action, explicit delegation, re-entry, priority, and follow-up** that need to survive outside the calendar.

A calendar invitee is not automatically a Todoist assignee. Do not reproduce event context as task structure unless a concrete Action actually needs to persist.

## Labels

- `research_idea` — a possible scientific question, hypothesis, comparison, experiment, or research direction; not yet a committed Outcome.
- `teaching_idea` — an explanation, exercise, demonstration, or teaching possibility worth preserving but not yet curated.
- `theory_investigation` — work intended to derive, check, or understand mathematics, physics, assumptions, model structure, or theoretical meaning.
- `platform_investigation` — work intended to understand or test a tool, API, hardware interface, software architecture, timing behavior, communication route, or deployment boundary.
- `reference_link` — an internal or external source/artifact retained because consulting, reusing, or returning to it serves a specific task, investigation, or mastery need. It may point to a paper, manual, webpage, vendor documentation, dataset, prior report, notebook, Markdown note, figure set, GitHub file, frozen export, or another personally created artifact. It is not a generic bookmark collection and does not merely mean that a task happens to contain a link.
- `teaching_material` — stabilized reusable student-facing knowledge, example, exercise, demonstration, or module.
- `publishable_material` — a **scientific quality / maturity marker** for validated evidence, comparison, result, figure, limitation, or finding worth preserving as a reusable building block. It describes the scientific value and readiness of the material, **not its legal or IP publication status**. Confidentiality, contracts, and IP restrictions remain separate release questions.
- `report_draft` — an active formal document being assembled for an external or institutional recipient, including grant proposals, industrial proposals, progress/final reports, government reports, and similar deliverables. It describes the document-output state, not scientific ownership.

`paper_draft` and `book_draft` are better treated as later-stage mental/organizational states once enough material has clustered to justify an actual manuscript structure. `report_draft` is broader and may appear before or after validated evidence: a proposal can combine `research_idea`, prior `publishable_material`, and planned future work, while a final report usually consolidates completed evidence and obligations.

Labels may cross project boundaries. **A label never overrides primary intention or hierarchy.**

## Task links, working artifacts, and evidence comments

Detailed artifact identity, placement, and evidentiary meaning belong in [artifact placement](artifact-placement.md), not in Todoist.

Keep the Todoist rule small:

```text
Task / hierarchy = intended work
Label            = useful type or state of work
Attachment/link  = working artifact or source the task needs
Comment          = short evidence / decision statement
```

Do **not** add `artifact` or `evidence` as general labels. A link to the task's own working artifact does not by itself require `reference_link`; use `reference_link` when consulting, reusing, or returning to the linked object is itself part of the task. A comment may record what happened and what it presently means, but the underlying artifact or data remains the evidence.

## From idea to material

`research_idea` can lead through theory or platform investigation to scrutinized evidence and `publishable_material`; a coherent claim can then justify a paper. `teaching_idea` can become curated `teaching_material`. An external `report_draft` can draw on ideas and evidence without taking ownership of the science. See [Ontology](ontology.md#evidence-accumulation-and-publication) for the research lifecycle.

# Working Hierarchy: Think Freely, Normalize Deliberately

Research thinking does not need to begin in a perfect hierarchy. During exploration, a new thought or an old task may naturally appear at arbitrary depth:

```text
possible Outcome
→ general Milestone
→ forming sub-Milestone
→ deeper sub-Milestone
→ possible Action
→ sub-Action
```

These are **temporary interpretations**, not permanent ontology categories. Their purpose is to reveal intention and relationships while the work is still being understood.

The long form is therefore an **explanation to myself**. It should make it possible to answer:

> **Why did I want to do this Action? Where is it embedded? What larger result does it support? How did this line of work get here?**

A long-form hierarchy may be deliberately verbose:

```text
intention
    ↓
desired Outcome
    ↓
Milestones that would make the Outcome true
    ↓
possible Actions
    ↓
expected result / evidence idea
and likely evidence form: figure / table / comparison / demonstration / verified behavior
```

This explanation may live in a Markdown note, research notebook, README, paper notebook, or another working document. It does not need to be copied into Todoist.

## Three-level wording rule

The stable three-level hierarchy has different wording because each level answers a different question.

- **Outcome — expected result / subject / evidence-oriented noun phrase or desired state.** It names what should ultimately exist or become true, without pretending the method is already known.
- **Milestone — deliverable or verifiable state wording.** It describes an intermediate condition that can be inspected, demonstrated, compared, or declared ready.
- **Action — verb-first executable wording.** It says what someone can actually do next to move the Milestone toward that state.

A simple example is:

```text
Outcome
Programming capability matrix for ROS 2 development

Milestone
C/C++ capability criteria defined and mapped to representative ROS 2 work

Action
Map arrays, classes, references/pointers, callbacks, and interfaces to ROS 2 examples
```

Another Milestone under the same Outcome could be:

```text
Milestone
Diagnostic questionnaire piloted against the capability matrix

Actions
Draft reasoning-based questions
Pilot the questionnaire
Compare responses with the intended capability levels
```

The wording rule is a preference, not a grammar law. Its purpose is to make the relationship visible: the Outcome names the result, the Milestone names a demonstrable intermediate state, and the Action begins the work.

## Short hierarchy preserves the long-form relationship
Once the reasoning is understood, much of the wording can disappear without losing the relationship.

```text
Programming capability for ROS 2 development
└── Capability matrix
    └── Define C/C++ criteria
```

The short hierarchy still says:

```text
this Action
    → supports this Milestone
    → supports this Outcome
    → exists because of this intention
```

The long form preserves **reasoning and history**. The short hierarchy preserves the **structure of that reasoning**.

`Outcome`, `Milestone`, and `Action` are therefore **relative roles, not permanent task classes**. An Outcome may later become a Milestone inside a larger understanding. A Milestone may become today's Action. An apparently small Action may reveal enough complexity to temporarily need its own hierarchy.

```text
large Outcome today
       ↓
part of a larger understanding tomorrow
       ↓
Milestone
       ↓
current executable Action
```

The ontology should clarify thought, not create bureaucracy.

# Run 1 → Run 2 → Run 3

The three names describe one movement from understanding to action. They are also the left, right, and forward steps:

| Run | Step | Working space | Result |
| --- | --- | --- | --- |
| Run 1 | Left | Notebook 1 | Long form, including the semester snapshot |
| Run 2 | Right | Notebook 2 | Short-form map |
| Run 3 | Forward | Todoist | Minimum useful Actions and re-entry |

These are modes, not compulsory documents. Notebook 1 and Notebook 2 support the first two runs; Notebook 3 holds technical work. Todoist coordinates Run 3. A thought need not pass through every form.

The older use of “forward step” meant looking across the placed clusters for patterns of past focus and possible routes. Keep that observation in the right step when it is useful; the forward step now means taking justified action. Do not create tasks merely because a coordinate looks sparse.

## Run 1 — Reveal / recover intention

For a thought or old task, recover its true intention, possible Outcome, Milestones, associated artifacts, and desired evidence before reorganizing it. Old wording and file type are clues, not authority. A deliverable's likely shape—model, comparison, figure, capability matrix, or demonstration—helps clarify the Milestone.

For historical files, mark `freeze_file` when preservation suffices or `future_outcome` when valid work is not active. These are provisional annotations, not ontology categories. Continue only the active subset. Evidence may revise the hierarchy; doing so is learning, not an indictment of earlier work. A new thought may stay in Notebook 1 or a working note without entering Todoist.

## Run 2 — Compress, cluster, and reorganize

Condense the recovered relationships into a short form. Merge duplicate historical hierarchies, while preserving genuinely distinct Outcomes. Judge whether each surviving intention calls for action now, delegation, waiting, or later re-entry; do not invent urgency. Priority and dates are evidence to interpret, not commands inherited from old tasks.

Cluster, split, rename, relocate, retain, or retire work as evidence warrants. Preserve the intention and time horizon, then update the long-form snapshot if the short form reveals a better interpretation. The result should be clear enough for a lean Todoist projection.

## Run 3 — Expose the minimum actionable subset

Todoist receives only the work that benefits from external memory, re-entry, assignment, priority, or future execution.

```text
understood hierarchy
      ↓
minimum useful subset
      ↓
short actionable wording
      ↓
do
      ↓
tick
```

Not every thought becomes a task. Not every task deserves a hierarchy. Immediate working steps may stay in the current file and simply be completed there.

Hierarchy is most useful when the work must survive interruption, spans several sessions or people, or needs to preserve why a future Action exists. A team project may intentionally preserve more explicit hierarchy and short annotation because the structure must communicate intention to people who do not share the same mental context.

The practical separation is:

```text
working notes            = current thinking and execution detail
README / long-form notes = durable reasoning and ontology
Todoist                  = minimum actionable / re-entry subset
finished artifacts       = what should actually grow
```

The goal is **not to grow the ontology map**. The goal is to grow finished lectures, modules, code, experiments, figures, drafts, and papers.

## Run outputs and the semester snapshot

The useful result is a coherent passage from understanding to action, not a required number of files:

```text
left / Run 1  → Notebook 1 → long-form understanding and semester snapshot
right / Run 2 → Notebook 2 → short-form map of the current direction
forward / Run 3 → lean Todoist actions and re-entry
technical execution → Action notebook and working artifacts
```

For the current cleanup, Todoist may be lean first. Reconstruct the dated [semester map](semester-ontology-cycle.md) in long form and condense it in short form; revise the long form if compression reveals something new. Keep V0 in Todoist until the provisional snapshot is satisfactory, then lean further. The map can remain relatively stable as work evolves.

Before an item enters or stays in Todoist, ask:

- Does it need external memory, assignment, a genuine time constraint, or future re-entry?
- Is there a concrete Action or useful Milestone that can be named briefly?
- Does the task still point to the recovered intention and the authoritative working artifact?
- Should it be done now, delegated, revisited later, or removed after checking evidence?

A Markdown candidate list is optional. Long form holds reasoning and the snapshot; short form maps it; Todoist keeps timely Actions. Avoid duplicating them.
