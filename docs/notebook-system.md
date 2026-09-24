# Personal Intention-to-Action Notebook System

[Home](../README.md) · [Ontology](ontology.md) · [Semester cycle](semester-ontology-cycle.md) · [Todoist](todoist.md) · [Artifact placement](artifact-placement.md)

# Purpose

The three notebooks change the mode of thinking: Notebook 1 supports [Run 1 / left / long form](todoist.md#run-1--run-2--run-3); Notebook 2 supports Run 2 / right / short form; Notebook 3 holds technical execution. Run 3 / forward uses Todoist for actionable re-entry.

```text
I/O notebook
private observation
true intention → desired Outcome
        ↓
Milestone / Artifact / Evidence notebook
private design reasoning
possible Milestones
→ artifact shape / form / format
→ evidence possibilities
→ possible next Action
        ↓
Action notebook
technical / potentially student-facing execution
        ↓
Todoist
only the Actions that benefit from re-entry,
delegation, priority, or future execution
```

The purpose is to avoid forcing a raw feeling or intention directly into an Action. Intention can first be observed, then interpreted through possible Milestones, artifacts, and evidence, before technical work is exposed.

# Trigger and triage

An outside request or obligation may trigger several internal intentions. Separate them, then judge **urgency** (when to respond) and **clarity** (how much thought is needed). If the next Action is clear and urgent, act; capture unresolved follow-up afterward. Otherwise, use the notebooks to move from intention through possible Milestones, artifacts, and evidence toward technical Action. Todoist preserves only work needing future re-entry, assignment, priority, or scheduling.

The hierarchy is provisional. An Outcome may become a Milestone; evidence may split, merge, redirect, or close a route. Use the notebooks to sort these roles before imposing a formal hierarchy. A feeling may prompt inquiry into intention, but it does not prove a technical claim or obligate action.

# 1. I/O notebook — intention and Outcome

The I/O notebook is private and descriptive. It records the **true intention** as honestly as possible and the most desired Outcome associated with it.

Here, recover the reasoning and write the dated, provisional semester snapshot when satisfactory.

The first question is:

> **What do I actually want, and what Outcome would satisfy that intention?**

Record the intention before judging whether it is wise, moral, feasible, obligatory, or something that should be acted upon. Observation is not endorsement. The aim is to avoid distorting the intention before understanding it.

A compact relationship is:

```text
felt intention
      ↓
desired Outcome
```

No Action is required merely because an intention has been written down.

# 2. Milestone / Artifact / Evidence notebook — possibility design

This notebook is the private bridge between intention and work. It asks what intermediate states could make an Outcome more real and what kind of artifact or evidence could make those states inspectable.

Here, condense the snapshot into a short-form map; return new insights to the long form.

Useful questions include:

- What Milestone would make meaningful progress visible?
- What would that Milestone look like when it exists?
- What artifact shape, form, or format could embody it?
- What evidence could support, weaken, redirect, or reject the present interpretation?
- Does the work suggest a theory investigation, platform investigation, capability-gap closure, teaching activity, learning activity, or research activity?
- What concrete Action becomes visible from this reasoning?

Artifact shape is deliberately considered early. A vague Milestone often becomes actionable once its possible form can be imagined, for example:

```text
derivation
block diagram
comparison table
MATLAB / Simulink model
STM32 demonstration
experiment
figure
lecture example
capability matrix
```

These are possibilities, not commitments. The notebook remains a free-thinking space where Milestones and routes may be rewritten as understanding changes.

## Two kinds of evidence

Keep two meanings of evidence distinct.

### Internal evidence — evidence about intention

Feelings such as attraction, resistance, relief, resentment, appeasement, excitement, or unease can be useful observations about the relationship between the person and the proposed Outcome.

```text
feeling / reaction
      ↓
evidence about intention,
alignment, or relationship to the Outcome
```

This evidence can justify re-examining the intention, Outcome, or route. It is not technical proof that a model, controller, experiment, or scientific claim is correct.

Strong anxiety can be treated as a **signal worth investigating**, especially when an external obligation appears to have triggered competing internal intentions. It is not proof that such a conflict exists: anxiety may also come from uncertainty, perceived threat, time pressure, overload, lack of control, or other causes. The useful response is therefore clarification rather than diagnosis:

```text
strong reaction / anxiety
        ↓
ask what intentions are active
        ↓
separate possible intention conflict
from uncertainty / overload / genuine urgency
        ↓
clarify the desired Outcome and next response
```

The notebook system therefore uses emotional reaction as **internal evidence for inquiry**, not as a verdict. Its role is to help unresolved intentions become clear before they are converted into Milestones, Actions, or new obligations.

### Technical evidence — evidence about the work

Derivations, measurements, experiments, comparisons, figures, observed behavior, student demonstrations, and verified implementations can support or weaken technical claims, Milestones, or research Outcomes.

```text
derivation / measurement / experiment / demonstrated behavior
      ↓
evidence about a technical claim,
Milestone, or Outcome
```

A useful artifact may be **evidence-bearing** without yet being sufficient evidence for the final Outcome.

# 3. Action notebook — technical execution

The Action notebook changes mode. It is no longer primarily personal ontology reasoning; it is where the actual technical work lives and is deliberately capable of becoming student-facing or collaborator-facing.

Notebook 3 holds the work; Todoist preserves only Actions needing re-entry, scheduling, or delegation.

Typical contents include:

```text
equations and derivations
block diagrams
signal-flow sketches
platform / wiring / interface sketches
experimental procedures
MATLAB / Simulink work
embedded / ROS / software notes
measurements and observations
technical questions and demonstrations
```

Private intention archaeology does not need to be copied here. The technical work should be understandable on its own terms to the people who may need to learn from, execute, review, or extend it.

The transition is therefore:

```text
personal intention
      ↓
designed Milestone / artifact / evidence possibility
      ↓
executable technical work
```

## Investigative Action, artifact, and evidence

Theory investigation, platform investigation, capability-gap work, and other technical Actions will often **create, revise, test, or inspect an artifact**. The resulting behavior or observation may then become evidence.

```text
investigative Action
      ↓
create / revise / test / inspect artifact
      ↓
result / observed behavior
      ↓
evidence
      ↓
update the present interpretation
```

Keep the roles distinct:

```text
Action   = what is done
Artifact = what is created, revised, tested, inspected, or preserved
Evidence = what the resulting artifact or behavior presently supports,
           weakens, contradicts, or reveals
```

Investigative work does **not** require a new file for every Action. When the same intention and artifact continue, revising the existing authoritative artifact is normally preferable to proliferating copies. Create another artifact when the work genuinely needs a different object, format, audience, or evidentiary role.

Likewise, an artifact is not automatically evidence merely because it exists. A MATLAB script, block diagram, model, figure, dataset, or derivation becomes evidence-bearing through what its execution, comparison, inspection, or interpretation actually shows.

When an investigative Action is represented in Todoist, the practical boundary is:

```text
Task / Action
= what needs to be done or revisited

Attachment / link
= where the current authoritative working artifact lives

Comment
= concise evidence / decision interpretation:
  What happened?
  What does it presently mean?
  Did it change what comes next?
```

`evidence` therefore normally remains a **result / interpretation relationship**, not a general Todoist label. The durable technical evidence remains in the artifact; the Todoist comment only preserves enough interpretation to support re-entry and later recovery.

# Todoist boundary

The Action notebook holds technical work. Todoist coordinates only Actions needing re-entry, assignment, priority, scheduling, or delegation; immediate steps can be done directly. A linked artifact remains in its authoritative working home. See [Todoist](todoist.md).

# Calendar relationship

Calendar provides another projection of the same intention system: **intention situated in time and company**.

```text
Calendar title       = real-world context / commitment
Calendar description = intention / ontology direction
Calendar invitees    = people accompanying that intention / first delegation candidates
Todoist assignment   = actual delegation of a concrete Action
```

An invitee is not automatically assigned a task. The calendar marks who is presently in the human path of an intention; Todoist makes delegation explicit when a concrete Action exists.

# Operating loop

Execution and evidence can revise the Action, Milestone, artifact route, Outcome, or even the interpretation of intention. The notebooks support that feedback without requiring every thought to become a task.
