# Peter I-Tsyuen Chang 張以全

Assistant Professor  
Department of Mechanical Engineering  
National Taiwan University of Science and Technology (Taiwan Tech)

## Focus Areas
- Robotics & Autonomous Systems
- Control Engineering
- Embedded Systems (STM32 / Real-Time)
- MATLAB / Simulink
- ROS 2 Development
- Engineering Education

## Current Mission
Building modern learning pathways that connect mechanical engineering, software, electronics, and intelligent systems.

## Repositories
- teaching → course materials and curriculum
- learning → experiments, notes, prototypes
- working → integrated development projects

## Contact
itchang@mail.ntust.edu.tw

## Philosophy
Learning → building → teaching → research evidence → publication

Historical working idea:

research/publish = learning + teaching

Current interpretation:

learning → research/building → validated evidence → publication

research/building → curated knowledge → teaching

The older `research/publish = learning + teaching` idea is kept here because it reflects how the current system evolved. The newer structure separates the intentions more clearly: research develops and validates knowledge, publication records research outcomes, and teaching consumes selected, stabilized knowledge in a form appropriate for students.

## Transition
Vision → Outcome → Milestone → Next Action

For example: Learn ROS Control

That's neither a clear outcome nor a good next action.

Compare:

```
Vision
Build a reusable ROS 2 control architecture for research and teaching.

↓

Outcome
Omni vehicle executes closed-loop velocity control through ROS 2.

↓

Milestone
ROS 2 node publishes wheel velocity commands and reads encoder feedback.

↓

Next action
Run existing ros2_control example and identify controller, command topic, and feedback topic.
```

Now Todoist knows what you can actually do.

## PROFESSIONAL PURPOSE

```text
│
├── RESEARCH
│   ├── Omni-Vehicle Integrated Control Systems
│   ├── Robot Manipulator Force Control
│   ├── Motor Torque Estimation & Compensation
│   └── Real-Time Embedded System Integration
│
├── TEACH
│   ├── Computer Integrated Control Systems
│   └── Lab Courses
│
└── PUBLISH
    └── publication is normally an outcome of the research theme that produced it
```

Research projects are organized by technical/research intention rather than by tool. MATLAB, Simulink, Python, C/C++, ROS 2, Gazebo, RViz, STM32, RTOS, and related technologies live inside whichever research theme their use primarily advances.

Teaching is downstream of the research worlds: mature knowledge is curated and simplified into course outcomes, milestones, examples, laboratories, and student-facing material.

## Technical infrastructure

```text
model → simulation → software → embedded implementation → sensing → feedback/control → ROS 2/distributed system → physical experiment
```

```text
MATLAB / Simulink
       ↓
Python / numerical computing
       ↓
C / C++
       ↓
STM32 / RTOS
       ↓
ROS 2
       ↓
simulation + hardware
       ↓
control / estimation experiments
```

## Review template

```text
| Dimension                      | Question                                                                                   |
| ------------------------------ | ------------------------------------------------------------------------------------------ |
| **Subject**                    | Who/what is this fundamentally for? Me / student / collaborator / course / research system |
| **Actor** *(only when needed)* | Who actually has to perform the work?                                                      |
| **Time-wise**                  | Active / Next / Archive                                                                    |
| **Level**                      | Vision / Outcome / Milestone / Next Action                                                 |
| **Interpretation**             | What was I actually trying to accomplish when I wrote this?                                |
```

## Todoist philosophy

Research  
Todoist Project = research theme/world  
→ Section = Outcome  
→ Task = Milestone  
→ Subtask = ~1-hour Action

Teaching  
Todoist Project = Teaching  
→ Section = Course / semester / target student body  
→ Task = Outcome  
→ Subtask = Milestone  
→ Sub-subtask = ~1-hour Action

## Todoist hierarchy

```text
RESEARCH PROJECTS
│
├── 1. Omni-Vehicle Integrated Control Systems
│      Research Theme Platform Project
│      omni-vehicle dynamics / kinematics / estimation / force compensation
│      platform integration through ROS 2 and embedded systems
│      MATLAB / Simulink, Python, C/C++ as needed by the research intention
│      Gazebo / RViz / TurtleBot and related simulation/deployment work
│      high-level distributed control → low-level embedded deployment
│
├── 2. Robot Manipulator Force Control
│      Research Theme Project
│      robotics theory / manipulator modeling / numerical analysis
│      DH / MDH / SDH / URDF / rigid-body representation / kinematics
│      dynamics with force / impedance / adaptive control
│      Jacobian-based deployment analysis and Jacobian-free development
│      MATLAB Robotics Toolbox / ROS Toolbox / ROS 2
│      Gazebo / RViz manipulator simulation and deployment
│      high-level theory → physical implementation
│      *JACOBIAN-FREE ADAPTIVE CONTROL*
│
├── 3. Motor Torque Estimation & Compensation
│      Research Theme Platform Project
│      single-axis actuator foundation: DC → PMSM / BLDC
│      electrical + mechanical modeling
│      nonlinear friction modeling
│      EKF / stochastic estimation / external torque estimation
│      torque and friction compensation
│      MATLAB / Simulink modeling and validation
│      Speedgoat / embedded-code-generation experiments where they advance actuator research
│      provides low-level force/torque estimation foundations for Projects 1 and 2
│
│      Projects 1–3 all require shared embedded-system understanding ↓
│
├── 4. Real-Time Embedded System Integration
│      Research Theme Platform/Foundation Project
│      currently in a learning / exploratory phase
│      contains learning objectives, research ideas, experiments, and teaching ideas
│      when the primary intention is understanding the deployment boundary itself
│      │
│      ├── Simulink Embedded Code Generation
│      │      model
│      │        ↓
│      │      Embedded Coder
│      │        ↓
│      │      generated C/C++
│      │        ↓
│      │      STM32 peripherals / HAL
│      │        ↓
│      │      real hardware
│      │
│      └── RTOS Embedded Control Architecture
│             C/C++ implementation
│             STM32 HAL
│             timers / interrupts
│             FreeRTOS tasks
│             scheduling
│             timing / jitter
│             buffering / communication
│             micro-ROS
│
│      research question:
│      how do implementation boundaries, timing, scheduling, computation,
│      communication, and hardware constraints alter assumptions made in
│      mathematical/control models?
│
└──────────────────────────┐
                           ↓ curated and stabilized knowledge
TEACHING
└── Computer Integrated Control Systems
       └── Embedded / real-time control outcome
             ├── MCU and system boundary
             ├── model → code → hardware
             ├── sampling / timers
             ├── HAL / peripherals
             ├── RTOS scheduling
             └── ROS 2 / embedded integration
```

### 4a — Model-Based Embedded Deployment

```text
MATLAB/Simulink model
        ↓
Embedded Coder
        ↓
generated C/C++
        ↓
HAL / board support
        ↓
STM32
```

### 4b — Explicit Real-Time Embedded Architecture

```text
Control/system model
        ↓
C/C++ implementation
        ↓
HAL / drivers
        ↓
interrupts + timers
        ↓
RTOS tasks
        ↓
scheduler
        ↓
STM32 hardware
```

## Controller development

Your control algorithm can begin as mathematics and simulation—MATLAB/Simulink, your adaptive law, force-control formulation, estimator, and so on. But to become robotics research rather than only a control-theory result, it needs a software layer that connects it to sensors, actuators, robot models, logging, visualization, and eventually hardware. ROS 2 is that integration layer.
So the chain is roughly:
```
control algorithm → ROS 2 controller/node → robot interfaces → embedded/RTOS layer → sensors & actuators
```
And information comes back upward:
```
ADC/encoder/force sensor → MCU/driver → ROS 2 messages/interfaces → controller → commanded torque/velocity/position
```
That also clarifies why your platform-investigation work matters. Learning rclcpp, messages, services/actions, parameters, lifecycle, ros2_control, hardware interfaces, timing behavior, and vendor APIs isn't a separate research hobby.

### Example of `platform_insvestication`

A `platform-investigation` such as *learning an rclcpp API* might initially just be exploration. As you work on it, it can branch naturally: (`research_idea` or `teaching_idea`)

```
→ Vision: integrated control/robotics lab capability
→ Outcome: ROS 2 control platform
→ Milestone: controller successfully runs through rclcpp
→ Action: understand callback/API/template syntax
```

But that same investigation may produce two different ideas:

`Research_idea`: “Can my Jacobian-free adaptive controller operate effectively within the standard ROS 2 robot stack?”\

`Teaching_idea`: “Students don't understand why rclcpp callbacks use templates and smart pointers; turn this into a C++ → ROS 2 teaching note.”

And importantly, an idea doesn't have to become an outcome immediately. Your tags let it sit as research-idea, teaching-idea, or platform-investigation until there's enough evidence that it's worth promoting.

Then the lifecycle becomes something like:
```
investigate → idea → promote → outcome → milestone → actions → result
```
And for research, a successful result can eventually become a publication outcome.

### usage of todoist

Tags answer: “What kind of thing is this?”

Hierarchy answers: “What are we actually committed to accomplishing?”

Tags allow thoughts to be immature. Hierarchy represents increasing commitment.

```
vison->outcome->milestone->action/task
```

### Usage of todoist labels

- research_idea — this might become research.

- teaching_idea — this might become teaching.

- platform_investigation — I need to understand/test this platform, API, hardware, etc.

- reference_link — retain this as a useful external reference.

- teaching_material — this has become reusable material for teaching.

- publishable_material — this has become reusable evidence/content for a publication.

For example, while working on your Jacobian-free force controller, you might produce a particularly good simulation comparison. At first the task could be research_idea or part of a research milestone. Once the result exists and you realize, this figure/result belongs in a future paper, tagging it publishable_material makes sense—even before you've committed to a particular manuscript.

The same thing already happens on the teaching side:
```
investigation → useful explanation/example → teaching_material → eventually incorporated into a course outcome
```
and now research gets the symmetrical path:
```
investigation → useful scientific result/evidence → publishable_material → eventually incorporated into a publication outcome
```
### side note

Learning + deliberate investigation can generate both teaching and research—but learning/teaching is not automatically research.

earn → investigate → understand → deduce/create
↙︎　　　　　　　　　　　　　　↘︎
teaching_material　　　　publishable_material
↓　　　　　　　　　　　　　　↓
course/module　　　　　 paper
↘︎　　　　　　　　　　　　　　↙︎
　　　　feeds the next investigation

- Learning gives you vocabulary.
- Investigation gives you understanding.
- Teaching forces you to make that understanding explicit and coherent.
- Research asks where the existing understanding is insufficient.
- Experimentation produces evidence.
- Publishing forces the evidence into a defensible argument.

Then published research becomes new teaching material, while teaching exposes gaps and questions that become new investigations.

### How to reach research materials

Vision
→ What scientific/engineering capability am I ultimately trying to establish?

Outcome
→ What concrete state would demonstrate progress?
Often a validated method, experimental result, working system, or ultimately a publication.

Milestone
→ What meaningful checkpoint can Peter or a student own and report?

Action
→ What can somebody actually do?
Derive this equation, modify this node, run this experiment, compare these datasets, make this figure.

Then the intellectual-state labels remain free to move through that hierarchy:
```
research_idea
↙︎ theory_investigation — Stribeck/stick-slip/model structure
↘︎ platform_investigation — Gazebo/hardware/contact/sampling behavior
↓
experiments + deductions - action/tasks and sub-tasks without labeling
↓
publishable_material
```
