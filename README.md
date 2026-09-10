# Peter I-Tsyuen Chang 張以全

Assistant Professor  
Department of Mechanical Engineering  
National Taiwan University of Science and Technology (Taiwan Tech)

## Focus Areas
- Robotics & Autonomous Systems
- Control Engineering
- Embedded and Real-Time Systems
- MATLAB / Simulink
- ROS 2 Development
- Engineering Education

## Current Mission

Build a control/robotics laboratory in which **research, engineering capability, teaching, and student development reinforce one another**.

The goal is not simply to collect tools or complete isolated projects. Mathematical models and control ideas should survive the path through simulation, software, communication, embedded execution, sensing, actuation, and physical hardware; the knowledge required to do this should become teachable and reusable; and experiments should return evidence that improves both research and education.

## Repositories
- `teaching` → reusable teaching modules, course materials, exercises, and curriculum
- `learning` → experiments, notes, and exploratory work
- `working` → integrated development and research work

## Contact
itchang@mail.ntust.edu.tw

# Philosophy

An earlier working idea was:

```text
Learning → building → teaching → research evidence → publication
research/publish = learning + teaching
```

The current interpretation is more explicit about intention and boundaries:

```text
                    ┌→ research question → theory → experiment → evidence → publication
learning/investigation
                    └→ stabilized understanding → teaching material → student capability
                                                        ↓
                                             stronger research platform
                                                        ↓
                                             next investigation/question
```

Teaching and research can share the same technical knowledge without being the same activity. Teaching forces understanding to become explicit and coherent; research asks where existing understanding is insufficient; engineering infrastructure makes theory physically realizable; publication organizes validated evidence into a defensible scientific argument.

A compact version is still:

```text
research = teaching + learning + questioning + validation
```

but the important improvement is that each activity now has a clear home and a clear path to action.

# Professional Purpose

```text
RESEARCH WORLDS
│
├── #1 Omni-Vehicle Integrated Control Systems
├── #2 Robot Manipulator Force Control
└── #3 Motor Torque Estimation & Compensation
       │
       │ require shared engineering capability
       ↓
#4 CONTROL SYSTEM INTEGRATION INFRASTRUCTURE
       │
       │ capability criteria / competence tests
       ├──────────────→ research platforms faithfully realize theory
       │
       └──────────────→ selected criteria become teaching/assessment requirements
                              ↓
TEACHING
       course → outcomes → milestones → actions
       labs / demonstrations / midterms / final projects
                              ↓
                    demonstrated student capability
                              ↓
                   stronger laboratory capability
                              ↓
                         RESEARCH WORLDS
```

Publication is normally an outcome of the research world that generated the scientific evidence rather than a separate technical world.

# Research Worlds #1–#3

The three research projects own **scientific questions, theory, application-specific implementation, experiments, and validated evidence**.

Their control-system Visions preserve the large research direction. The coherent **Vision v1 → v2 → v3** chain describes the main system-control development, while **v4 may remain an independent research branch** when a scientifically valuable question should mature without being forced into the main chain.

The hierarchy exists to make large ideas executable without losing their meaning:

```text
Vision
  ↓
Outcome
  ↓
Milestone
  ↓
Action assigned to the actual subject/receiver
  ↓
result / evidence
  ↓
revision of the larger understanding
```

A small Action should therefore be traceable upward to a meaningful research goal. A large Vision should be able to generate work small enough for Peter, a student, collaborator, subgroup, or specialist to actually perform.

# #4 Control System Integration Infrastructure

#4 is **not a fourth research-question generator**. It is the laboratory's reusable operational-capability standard.

Its purpose is to ensure that a research hardware platform is sufficiently understood, configured, and verified to faithfully execute the intended control theory.

```text
model / estimator / controller
        ↓
simulation
        ↓
software
        ↓
communication
        ↓
real-time / embedded execution
        ↓
sensing + actuation
        ↓
physical hardware
        ↓
verified experimental behavior
```

Current capability Outcomes include areas such as:
- STM32 / embedded control
- hardware/software integration
- numerical simulation
- theoretical derivation and explanation
- cross-platform communication and content verification
- CAD/CAE and physically meaningful geometry/inertial properties

A capability criterion is not a list of technologies to learn. It is a **demonstrable engineering standard**.

```text
necessary capability
      ↓
criterion
      ↓
appropriate subject tested
      ↓
competence gap exposed
      ↓
action generated
      ↓
learning / teaching / demonstration
      ↓
capability established
```

Not every capability must be mastered by everyone. A criterion may apply to Peter, broadly relevant MS students, a research subgroup, or a designated specialist.

## Intellectual-upward rule

#4 should become clearer as experience accumulates rather than simply becoming longer.

```text
read → reconstruct intent → annotate → restructure only when justified

accumulate → cluster → organize → revise → improve → promote
```

**Do not append downward by default. Integrate upward.**

The active hierarchy should increasingly represent the laboratory's current best understanding of what capability is actually necessary while preserving useful historical intent.

# Teaching

Teaching is the professional world where stabilized knowledge is **curated, sequenced, delivered, practiced, and assessed for a particular student population**.

```text
Teaching Project
  ↓
Section = course / semester / target student body
  ↓
Task = teaching Outcome
  ↓
Subtask = Milestone
  ↓
Sub-subtask = focused Action
```

The key boundary with #4 is:

> **#4 defines what must be demonstrable. Teaching defines how the selected students learn and demonstrate it.**

This means suitable #4 capability criteria can generate the engineering content of:
- laboratory demonstrations,
- practical midterm/final tests,
- final projects,
- project defenses, and
- MS graduation capability checks.

The assessment does not decide what engineering competence matters. The necessary capability is defined upstream; the assessment provides evidence that the selected student has met it.

A useful knowledge lifecycle is:

```text
external reference
      ↓
Peter learns / investigates
      ↓
Peter explains / teaches / demonstrates
      ↓
stabilized Teaching module
      ↓
student learns / presents / demonstrates
      ↓
verified laboratory capability
      ↓
research platform becomes stronger
```

Courses can then assemble reusable Teaching modules rather than becoming permanent containers for every technical idea.

# Project Boundaries

Placement follows **primary intention**.

```text
Is the question scientifically new or application-specific?
→ Research #1–#3

Is the problem a reusable engineering capability needed across research platforms?
→ #4 Infrastructure

Is the knowledge stable and now being prepared/delivered for students?
→ Teaching

Is the work institutional processing, reimbursement, approval, compliance, etc.?
→ Administration
```

The same technical subject can legitimately appear in several projects at different stages. What changes is the intention.

For example:

```text
ROS 2 behavior is unclear
→ #4 platform_investigation

ROS 2 is used to test an Omni-Vehicle scientific question
→ Research #1

ROS 2 understanding has stabilized into a student exercise
→ Teaching
```

# Todoist: Actionable Operating System

Todoist is used as a **living realization system**, not merely a task list.

Hierarchy answers:

> **Where is this work going, and what are we committed to accomplishing?**

Labels answer:

> **What kind of intellectual work/object is this right now?**

Assignment answers:

> **Who actually has to do or demonstrate it?**

Together they allow immature ideas to remain forgiving while still creating accountable execution when the work becomes mature enough.

## Labels

- `research_idea` — a possible scientific question, hypothesis, comparison, experiment, or research direction; not yet a committed Outcome.
- `teaching_idea` — an explanation, exercise, demonstration, or teaching possibility worth preserving but not yet curated.
- `theory_investigation` — work intended to derive, check, or understand mathematics, physics, assumptions, model structure, or theoretical meaning.
- `platform_investigation` — work intended to understand or test a tool, API, hardware interface, software architecture, timing behavior, communication route, or deployment boundary.
- `reference_link` — supporting external knowledge retained because it serves a specific investigation or mastery need; not a generic bookmark collection.
- `teaching_material` — stabilized reusable student-facing knowledge, example, exercise, demonstration, or module.
- `publishable_material` — validated evidence, comparison, result, figure, limitation, or finding worth preserving as a possible building block for publication.

`paper_draft` and `book_draft` are better treated as later-stage mental/organizational states once enough material has clustered to justify an actual manuscript structure.

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

Teaching can mature as:

```text
teaching_idea
   ↙︎                    ↘︎
theory_investigation   platform_investigation
   ↘︎                    ↙︎
 demonstrations / explanations
               ↓
        teaching_material
               ↓
       module / course
```

The same investigation can feed both paths, but **learning or teaching is not automatically research**, and a useful research result is not automatically ready to teach.

# The Actionable Loop

The system is intentionally cyclic:

```text
Research Vision
      ↓
scientific question / desired behavior
      ↓
Outcome → Milestone → bite-sized Action
      ↓
theory / simulation / experiment
      ↓
implementation requires capability
      ↓
#4 capability criterion
      ↓
competence test
      ↓
Peter / student / subgroup gap
      ↓
assigned mastery Action
      ↓
stabilized understanding
      ↓
Teaching module / assessment
      ↓
demonstrated student & lab capability
      ↓
stronger physical research platform
      ↓
validated evidence / new discrepancy / new question
      ↓
Research Vision revised or advanced
```

This loop is meant to generate **bite-sized, assignable work with directional meaning without losing the big picture**.

Small tasks remain connected to purpose. Large ideas are forced toward executable evidence. Teaching develops people. Infrastructure preserves engineering competence. Research generates new understanding. Each can feed the next cycle.
