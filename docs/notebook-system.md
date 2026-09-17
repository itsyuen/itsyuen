# Personal Intention-to-Action Notebook System

[Home](../README.md) · [Ontology](ontology.md) · [Semester cycle](semester-ontology-cycle.md) · [Todoist](todoist.md) · [Artifact placement](artifact-placement.md)

# Purpose

The three-notebook system separates private intention discovery, private design reasoning, and technical execution. The notebooks are not three levels of the same kind of note; each changes the mode of thinking.

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

# Hierarchy sorting and evolution

The notebook system also acts as a **hierarchy sorting and evolution mechanism**. A new thought often arrives with intention, obligation, desired Outcome, possible Milestone, artifact idea, evidence idea, emotional reaction, and next step mixed together. The notebooks separate those ingredients before a formal hierarchy is forced.

```text
I/O notebook
= reveal what the work is trying to become

Milestone / Artifact / Evidence notebook
= explore what structure, artifact, and evidence could make progress visible

Action notebook
= let the actual technical work and executable hierarchy take form
```

This supports **hierarchy sorting** because it becomes easier to distinguish an Outcome from a Milestone, an artifact possibility from evidence, and a possible Action from the technical work itself.

It also supports **hierarchy evolution**. Early wording is provisional rather than something that must be defended. Real work and evidence may show that:

- an apparent Outcome is actually a Milestone inside a larger intention;
- one Milestone should split into several;
- several Milestones are really one route;
- an artifact idea exposes the real technical question;
- an Action reveals that the original Outcome or route was wrong;
- new evidence supports, weakens, redirects, or closes part of the hierarchy.

The evolving loop is therefore:

```text
intention observed
      ↓
possible Outcome
      ↓
Milestones / artifacts / evidence explored
      ↓
technical Action emerges
      ↓
real evidence returns
      ↓
hierarchy may be revised, compressed, split, promoted, or demoted
```

The notebooks therefore provide a place for hierarchy to **incubate before formalization and mature through evidence**. Todoist receives only the subset that has become useful for re-entry, assignment, priority, or future execution.

# 1. I/O notebook — intention and Outcome

The I/O notebook is private and descriptive. It records the **true intention** as honestly as possible and the most desired Outcome associated with it.

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

The Action notebook contains the **work itself**. Todoist contains only the subset of Actions that benefits from external memory, re-entry, assignment, priority, scheduling, delegation, or future execution.

```text
Action notebook = equations, sketches, reasoning, experiments, implementation
Todoist         = coordination and re-entry for concrete Actions
```

Not every Action note needs a Todoist task. A step that can be completed naturally inside the current notebook may simply remain there and be done.

When an Action must survive interruption, involves another person, has a real temporal constraint, or deserves explicit delegation, it becomes a good Todoist candidate. Actual task assignment belongs in Todoist rather than being inferred from the notebook or calendar.

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

The notebooks are not a one-way pipeline. Evidence and execution can change the earlier interpretation.

```text
I/O
intention → desired Outcome
        ↓
Milestone / Artifact / Evidence
possible realization and evidence
        ↓
Action notebook
technical execution
        ↓
artifact / result / evidence
        ↓
feedback
        ├→ revise Action
        ├→ revise Milestone / artifact route
        └→ reconsider Outcome or intention
```

The system should remain permissive enough for thought to change. Its purpose is not to make every intention actionable; it is to make the transition from private intention to technical action deliberate and intelligible.