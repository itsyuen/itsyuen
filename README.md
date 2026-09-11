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
       ├── foundational theory / reference-system generator → #1 / #2
       ├── canonical implementation examples → #4 Infrastructure
       └── stabilized demonstrations → Teaching

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

The numbering identifies research worlds rather than priority. #3 is intentionally foundational: the motor/actuator is a comparatively simple, theory-rich physical system in which common estimation, control, reference-generation, implementation, and demonstration ideas can be derived before being challenged by the richer physics of #1 and #2.

## Common V1–V3 scientific pipeline

The main Visions now have explicit scientific roles:

```text
V1 — infer the system
     state estimation + parameter/system identification
     x, x_hat, parameters, disturbances

                ↓

V2 — control the system
     design real-time u(t)
     make the relevant state derivative / acceleration /
     generalized force or physical response well defined

                ↓

V3 — define where the system should go
     x_ref(t), x_dot_ref(t), x_ddot_ref(t)
     or appropriate angular / generalized counterparts
     human intention → desired behavior / reference
```

The exact states, parameters, physics, coordinates, sensors, actuators, and equations change between motor, Omni vehicle, and manipulator. The scientific questions and transferable abstractions provide the linkage; equations are re-derived for the actual research platform rather than copied blindly.

## #3 as foundational generator

#3 is the **foundational theory and reference-system generator**.

```text
                         #3 MOTOR / ACTUATOR
                    derive / test / abstract clearly
                              │
             ┌────────────────┼────────────────┐
             ↓                ↓                ↓
       #1 / #2 Research   #4 Infrastructure   Teaching
       richer physics     reference impl.     clear demonstrations
             │                │                │
             └────────────────┴────────────────┘
                              ↑
                    feedback / new questions
```

It should intentionally generate:
- foundational scientific abstractions that can be re-derived under #1 Omni-Vehicle and #2 Manipulator physics;
- canonical minimal examples for #4 capability criteria and implementation routes; and
- stable motor/actuator demonstrations that can become reusable Teaching material.

Transfer is not automatic. #1/#2 own their application-specific scientific questions, #4 owns reusable engineering capability standards, and Teaching owns stabilized pedagogy and assessment.

## V4 and research branching

V4 is not a required fourth step after V3.

For #1 and #2, V4 is a **controlled entry point for a scientifically valuable platform-specific challenge**. It may branch as `V4a`, `V4b`, `V4c`, etc. when experimental evidence, collaborators, industry, or another outside-originated/inspired problem reveals a defensible scientific question. Empty branch names do not need to be filled.

Examples currently include:
- `#1V4a` → wheel failure / fault-tolerant Omni-Vehicle control;
- `#2V4a` → Jacobian-free manipulator control, including the scientific challenge created when a Jacobian-free formulation meets conventional Jacobian/model-mediated robotics and ROS 2 assumptions.

#3V4 is intentionally asymmetric: it is the **cross-world intellectual-upward abstraction/consolidation space**. Structures such as `x_dot = A x + B u`, `y = C x`, or appropriate nonlinear forms can be used to ask what `x_hat`, `u`, `x_ref`, `x_dot_ref`, `x_ddot_ref`, parameters, disturbances, and physical meanings should be across the three research worlds. The paper question should emerge from the science rather than from a pre-filled V4 slot.

## Research coordinate and admission control

A notation such as `#iVj_k` acts as a lightweight research coordinate:
- `i = 1..3` identifies the research world;
- `j = 1..3` identifies the common scientific pipeline stage;
- `j = 4` identifies a justified research branch or, for #3, the abstraction/consolidation role;
- `k = a, b, c...` distinguishes genuine V4 branches when they emerge.

The coordinate helps answer three practical questions: **Where is the research now? Who is a good student/owner for it? Does a new external opportunity deserve admission into the research architecture?**

Student interest can first align with the research world: #1 with vehicle dynamics and vehicle experimentation; #2 with manipulator dynamics, Cartesian interaction, and force control; #3 with control theory, modeling, identification, estimation, derivation, and actuator-level experimentation. The Vision coordinate then gives the student a more precise scientific responsibility.

External or industrial work should not automatically create a new research direction. It should enter #1–#3 when it materially strengthens V1–V3 or earns a genuine V4 branch by exposing a worthwhile scientific problem. Otherwise it may belong in service, Teaching, Administration, another project, or simply be declined.

The hierarchy exists to make these large ideas executable without losing their meaning:

```text
Vision / research coordinate
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

Research #3's motor/actuator system is the preferred canonical minimal reference platform when it can demonstrate these capabilities without unnecessary vehicle/manipulator complexity.

## Infrastructure implementation routes

Capability Outcomes define **what must be achievable and demonstrable**. Implementation routes describe **how the capability may be realized**; they are not separate Projects or Outcome Sections.

```text
4a — Model-Based Embedded Deployment
     model/control → MATLAB/Simulink → code generation → MCU

4b — Explicit Embedded / Real-Time Architecture
     algorithm → C/C++ → HAL/peripherals → timers/RTOS → MCU

4c — Distributed ROS 2 / Cross-Platform Integration
     algorithm → ROS 2 interfaces → distributed compute/embedded nodes
               → simulation and/or robot hardware
```

A capability criterion may use one route or several. Tools may change while the capability standard remains. Regardless of route, signals, units, coordinate frames, timing/rates, numerical behavior, communication content, sensing, actuation, and physical response must preserve the intended engineering meaning.

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

Research #3's motor/actuator system is a preferred canonical minimal demonstration when it can expose the full model → state/parameter estimation → control input → reference/intention → implementation chain more clearly than a vehicle or manipulator. Once stabilized, the same example can become Teaching material and can demonstrate selected #4 capability criteria.

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

Is the work an industry-facing relationship, contract, deliverable, proposal/report, or client obligation?
→ Industry Projects

Is the work a government/university submission, approval, compliance, reimbursement, proposal/report, or other institutional obligation?
→ Administration
```

Industry Projects and Administration are **external-obligation shells**, not additional technical research worlds. Their proposals and reports may draw heavily from #1–#3, but the underlying scientific questions, methods, experiments, and evidence remain in their owning research coordinates.

The same technical subject can legitimately appear in several projects at different stages. What changes is the intention.

For example:

```text
ROS 2 behavior is unclear
→ #4 platform_investigation

ROS 2 is used to test an Omni-Vehicle scientific question
→ Research #1

ROS 2 understanding has stabilized into a student exercise
→ Teaching

An industrial final report needs the validated Omni-Vehicle result
→ report_draft in Industry Projects
   drawing from #1 publishable_material

A government grant proposal develops the next research direction
→ report_draft in Administration
   drawing from research_idea + existing evidence + planned #iVj_k work
```

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
- `publishable_material` — validated scientific evidence, comparison, result, figure, limitation, or finding worth preserving as a reusable building block. In industry-facing work this does **not** automatically mean legally/publicly publishable; confidentiality and IP restrictions still govern release.
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
        teaching_material
               ↓
       module / course
```

The same investigation can feed several paths, but **learning or teaching is not automatically research**, a useful research result is not automatically ready to teach, and a formal proposal/report does not become the owner of the scientific work it describes.

# The Actionable Loop

The system is intentionally cyclic:

```text
Research coordinate / Vision
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

Small tasks remain connected to purpose. Large ideas are forced toward executable evidence. Teaching develops people. Infrastructure preserves engineering competence. Research generates new understanding. External proposals/reports package selected ideas, plans, evidence, and obligations for a particular recipient without taking ownership away from the underlying work. Each can feed the next cycle.
