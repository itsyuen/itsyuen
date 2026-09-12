# Todoist and Actionable Work

[Home](../README.md) · [Ontology](ontology.md) · [Todoist](todoist.md) · [Artifact placement](artifact-placement.md) · [NAS consolidation](nas-consolidation.md)

This operating method applies the [professional ontology](ontology.md). Intellectual ownership follows intention; Todoist exposes work that benefits from re-entry, assignment, or future execution.

# Todoist: Actionable Operating System

Todoist is used as a **living realization system**, not merely a task list.

Hierarchy answers:

> **Where is this work going, and what are we committed to accomplishing?**

Labels answer:

> **What kind of intellectual work/object is this right now?**

Assignment answers:

> **Who actually has to do or demonstrate it?**

The research coordinate adds another question:

> **Which research world, scientific stage, or justified V4 branch is this work advancing?**

Together they allow immature ideas to remain forgiving while still creating accountable execution when the work becomes mature enough.

## Labels

- `research_idea` — a possible scientific question, hypothesis, comparison, experiment, or research direction; not yet a committed Outcome.
- `teaching_idea` — an explanation, exercise, demonstration, or teaching possibility worth preserving but not yet curated.
- `theory_investigation` — work intended to derive, check, or understand mathematics, physics, assumptions, model structure, or theoretical meaning.
- `platform_investigation` — work intended to understand or test a tool, API, hardware interface, software architecture, timing behavior, communication route, or deployment boundary.
- `reference_link` — supporting external knowledge retained because it serves a specific investigation or mastery need; not a generic bookmark collection.
- `teaching_material` — stabilized reusable student-facing knowledge, example, exercise, demonstration, or module.
- `publishable_material` — a **scientific quality / maturity marker** for validated evidence, comparison, result, figure, limitation, or finding worth preserving as a reusable building block. It describes the scientific value and readiness of the material, **not its legal or IP publication status**. Confidentiality, contracts, and IP restrictions remain separate release questions.
- `report_draft` — an active formal document being assembled for an external or institutional recipient, including grant proposals, industrial proposals, progress/final reports, government reports, and similar deliverables. It describes the document-output state, not scientific ownership.

`paper_draft` and `book_draft` are better treated as later-stage mental/organizational states once enough material has clustered to justify an actual manuscript structure. `report_draft` is broader and may appear before or after validated evidence: a proposal can combine `research_idea`, prior `publishable_material`, and planned future work, while a final report usually consolidates completed evidence and obligations.

Labels may cross project boundaries. **A label never overrides primary intention or hierarchy.**

## From idea to material

Research can mature as:

```text
research_idea
   ↙︎                    ↘︎
theory_investigation   platform_investigation
   ↘︎                    ↙︎
       actions / experiments
               ↓
        validated evidence
               ↓
      publishable_material
               ↓
            paper
```

External formal documents can draw from several states:

```text
research_idea ───────┐
                     ├→ report_draft → submitted proposal / report / deliverable
publishable_material ┤
                     │
planned future work ─┘
```

Teaching can mature as:

```text
teaching_idea
   ↙︎                    ↘︎
theory_investigation   platform_investigation
   ↘︎                    ↙︎
 demonstrations / explanations
               ↓
 curate by technical subject / target audience / knowledge level
               ↓
        teaching_material
               ↓
       module / course
```

The same investigation can feed several paths, but **learning or teaching is not automatically research**, a useful research result is not automatically ready to teach, and a formal proposal/report does not become the owner of the scientific work it describes.

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

The three-run method applies both to historical Todoist recovery and to new thoughts. Old work usually requires a heavier Run 1 because the original intention must be reconstructed; new work can often begin as a flat note in the file where the thinking is already happening.

## Run 1 — Reveal / recover intention

Start with the thought or old task and deliberately expand it enough to understand why it exists.

```text
thought / old task
      ↓
recover the true intention without moral judgment
      ↓
identify a possible Outcome and the evidence that would make it meaningful
      ↓
guess general Milestones, including likely deliverable shape / format
      ↓
identify possible Actions
      ↓
identify what result / evidence would support or weaken the proposed Outcome
(or show that a criterion is met / not met)
      ↓
place it in the correct professional / research world
```

For old tasks, Run 1 is partly archaeology. The purpose is to reconstruct what the earlier work was trying to accomplish, **not to accuse the earlier wording, decision, student, collaborator, or self**. Preserve useful intellectual history before deciding what should survive.

For new work, the same rule applies: a proposed hierarchy is permission to think, not a promise that the first interpretation is correct. General Milestones may initially be guesses, but they should already suggest the **shape or format of a deliverable**—for example a verified model, comparison table, figure, capability matrix, demonstrated behavior, or working implementation.

Possible Actions should also point toward evidence. The resulting evidence may support the proposed Outcome, weaken it, show that a criterion is not met, or expose a different explanation. That is useful information, not failure or accusation. It is explicit permission to **redo the hierarchy** when the evidence says the original structure was wrong.

For a new thought, Run 1 may simply be a handwritten note or a verbose block inside the current `.md` file. Todoist is not required at this stage.

## Run 2 — Compress, cluster, and reorganize

Once the intention is visible, return to the original thought and ask what actually needs to survive.

```text
long explanation
      ↓
cluster related ideas / evidence
      ↓
merge / rename / reorder
      ↓
remove scaffolding
      ↓
preserve the useful relationships
```

At this stage, items may be **sorted, merged, promoted, split, retained, archived, or discarded**. The hierarchy is a living hypothesis and should change when theory, platform investigation, evidence, or a better abstraction changes the understanding.

The goal of Run 2 is not to fill Todoist correctly. It is to make the ontology clear enough that the useful work can be represented simply.

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

