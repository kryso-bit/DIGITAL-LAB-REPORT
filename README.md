# Digital Electronics Laboratory --- Portfolio

**Institute of Engineering & Management (IEM), Kolkata**\
**Course:** Digital Electronics Laboratory (ESC392)\
**Department:** Information Technology\
**Semester:** 3rd Semester, B.Tech.\
**Student:** Suprobhat Dey\
**Class Roll No.:** 11\
**Section:** A\
**Academic Session:** 2026

------------------------------------------------------------------------

## About This Repository

This repository presents my Digital Electronics Laboratory portfolio for
**ESC392**. It brings together nine laboratory assignments covering
combinational logic, Boolean algebra, finite state machines (FSMs),
sequential circuits, counters, shift registers, datapath design, and
practical automation systems.

The portfolio combines theoretical design with circuit implementation
and simulation using **Logisim / Logisim Evolution**. Selected
assignments also explore the use of Generative AI tools (ChatGPT and
Gemini) to assist with logic synthesis, design explanation, and
debugging. AI-assisted results are treated as design support and are
evaluated against circuit behaviour, truth tables, and simulation.

## Portfolio at a Glance

  ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
                    No. Experiment / Assignment                                         Main Concepts           Circuit / Report
  --------------------- --------------------------------------------------------------- ----------------------- ----------------------------------------------------------------------------------------------------------------
                      1 [AI-Assisted Boolean Expression                                 4-variable K-map, SOP   [`circuits/Experiment-01-Boolean-Simplifier.circ`](circuits/Experiment-01-Boolean-Simplifier.circ)
                        Simplifier](#1-ai-assisted-boolean-expression-simplifier)       minimization, circuit   
                                                                                        equivalence             

                      2 [Natural Language to Logic Circuit                              Boolean modelling,      [`circuits/Experiment-02-Natural-Language-Logic.circ`](circuits/Experiment-02-Natural-Language-Logic.circ)
                        Generator](#2-natural-language-to-logic-circuit-generator)      AND/OR logic,           
                                                                                        access-control example  

                      3 [FSM Design for Traffic Light                                   Moore FSM, state        [`circuits/Experiment-03-Traffic-Light-FSM.circ`](circuits/Experiment-03-Traffic-Light-FSM.circ)
                        Controller](#3-fsm-design-for-traffic-light-controller)         transitions, D          
                                                                                        flip-flops, pedestrian  
                                                                                        request                 

                      4 [AI-Based Fault Detection in Digital                            Truth-table testing,    [`circuits/Experiment-04-Fault-Detection.circ`](circuits/Experiment-04-Fault-Detection.circ)
                        Circuits](#4-ai-based-fault-detection-in-digital-circuits)      fault diagnosis,        
                                                                                        circuit correction      

                      5 [24-Hour Digital Clock Using                                    Synchronous counters,   [`circuits/Experiment-05-Digital-Clock.circ`](circuits/Experiment-05-Digital-Clock.circ)
                        FSM](#5-24-hour-digital-clock-using-fsm)                        flip-flops, rollover    
                                                                                        logic, 7-segment        
                                                                                        display                 

                      6 [Application Mapping of Sequential Building                     D flip-flop, Mod-60     [`circuits/Experiment-06-Sequential-Blocks.circ`](circuits/Experiment-06-Sequential-Blocks.circ)
                        Blocks](#6-application-mapping-of-sequential-building-blocks)   counter, shift register 

                      7 [Automatic Parking Barrier                                      FSM, vehicle detection, [`circuits/Experiment-07-Parking-Barrier.circ`](circuits/Experiment-07-Parking-Barrier.circ)
                        Control](#7-automatic-parking-barrier-control)                  payment confirmation,   
                                                                                        safety interlock        

                      8 [4-Bit Mini-ALU and Program                                     Arithmetic datapath,    [`circuits/Experiment-08-Mini-ALU-Program-Counter.circ`](circuits/Experiment-08-Mini-ALU-Program-Counter.circ)
                        Counter](#8-4-bit-mini-alu-and-program-counter)                 addition/subtraction,   
                                                                                        registers, synchronous  
                                                                                        counter                 

                      9 [AI-Assisted Code-to-Gate                                       Conditional logic,      [`circuits/Experiment-09-Code-to-Gate.circ`](circuits/Experiment-09-Code-to-Gate.circ)
                        Explainer](#9-ai-assisted-code-to-gate-explainer)               magnitude comparator,   
                                                                                        multiplexers,           
                                                                                        code-to-hardware        
                                                                                        mapping                 
  ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

> **Circuit-link note:** The links above use a suggested repository
> naming convention. Place the corresponding `.circ` files in the
> `circuits/` directory and rename the files to match these paths, or
> edit the links to match your actual filenames. If an experiment has
> multiple circuit files, add each file under its experiment row or
> section.

## Table of Contents

-   [About This Repository](#about-this-repository)
-   [Portfolio at a Glance](#portfolio-at-a-glance)
-   [Experiments](#experiments)
    -   [1. Boolean Expression
        Simplifier](#1-ai-assisted-boolean-expression-simplifier)
    -   [2. Natural Language to Logic
        Circuit](#2-natural-language-to-logic-circuit-generator)
    -   [3. Traffic Light
        FSM](#3-fsm-design-for-traffic-light-controller)
    -   [4. AI-Based Fault
        Detection](#4-ai-based-fault-detection-in-digital-circuits)
    -   [5. 24-Hour Digital Clock](#5-24-hour-digital-clock-using-fsm)
    -   [6. Sequential Building
        Blocks](#6-application-mapping-of-sequential-building-blocks)
    -   [7. Automatic Parking
        Barrier](#7-automatic-parking-barrier-control)
    -   [8. Mini-ALU and Program
        Counter](#8-4-bit-mini-alu-and-program-counter)
    -   [9. Code-to-Gate
        Explainer](#9-ai-assisted-code-to-gate-explainer)
-   [Tools and Technologies](#tools-and-technologies)
-   [Repository Structure](#repository-structure)
-   [How to Open the Circuits](#how-to-open-the-circuits)
-   [Learning Outcomes](#learning-outcomes)

------------------------------------------------------------------------

## Experiments

### 1. AI-Assisted Boolean Expression Simplifier

**Objective:** Simplify a four-variable Boolean function using a
Karnaugh map, implement both canonical and minimized SOP forms, and
compare their outputs.

-   Function studied: `F(A, B, C, D) = Σm(0, 2, 8, 10, 12, 14)`
-   Focus: K-map grouping, prime implicants, SOP minimization, and
    truth-table verification.
-   The report compares the unsimplified and minimized implementations
    in Logisim.

**Circuit:**
[`Experiment-01-Boolean-Simplifier.circ`](circuits/Experiment-01-Boolean-Simplifier.circ)

### 2. Natural Language to Logic Circuit Generator

**Objective:** Translate a natural-language access-control requirement
into a Boolean expression and a gate-level circuit.

-   Example system: secure vault release.
-   Boolean expression: `Y = A · (B + C)`
-   Focus: translating requirements into logic variables, factoring
    Boolean expressions, and verifying all input combinations.

**Circuit:**
[`Experiment-02-Natural-Language-Logic.circ`](circuits/Experiment-02-Natural-Language-Logic.circ)

### 3. FSM Design for Traffic Light Controller

**Objective:** Design a synchronous Moore finite state machine for a
traffic light controller with a pedestrian-request input.

-   States represent Green, Yellow, and Red phases.
-   A pedestrian request initiates the transition from Green to Yellow.
-   Focus: state encoding, transition tables, D flip-flop input
    equations, and output logic.

**Circuit:**
[`Experiment-03-Traffic-Light-FSM.circ`](circuits/Experiment-03-Traffic-Light-FSM.circ)

### 4. AI-Based Fault Detection in Digital Circuits

**Objective:** Use truth-table behaviour and logical analysis to
identify and correct a digital-circuit fault.

-   The report demonstrates a faulty Full Adder sum path behaving like a
    Half Adder sum.
-   The missing carry-in contribution is identified and corrected using
    an additional XOR stage.
-   Focus: test vectors, expected-versus-observed outputs, debugging,
    and simulation-based verification.

**Circuit:**
[`Experiment-04-Fault-Detection.circ`](circuits/Experiment-04-Fault-Detection.circ)

### 5. 24-Hour Digital Clock Using FSM

**Objective:** Design a 24-hour digital clock using synchronous counters
and flip-flops.

-   Seconds and minutes count from 00 to 59.
-   Hours count from 00 to 23.
-   Carry signals connect the counter stages, and the clock rolls over
    after 23:59:59.
-   Focus: counter design, rollover conditions, and 7-segment display
    output.

**Circuit:**
[`Experiment-05-Digital-Clock.circ`](circuits/Experiment-05-Digital-Clock.circ)

### 6. Application Mapping of Sequential Building Blocks

**Objective:** Study and simulate common sequential building blocks and
relate them to practical digital systems.

This experiment covers:

1.  **D Flip-Flop:** a one-bit memory element with clocked data storage.
2.  **Mod-60 Counter:** a counter for 0--59 with reset/rollover logic,
    relevant to clock timebases.
3.  **Shift Register:** serial/parallel data movement, including
    shifting and parallel loading.

**Circuit:**
[`Experiment-06-Sequential-Blocks.circ`](circuits/Experiment-06-Sequential-Blocks.circ)

### 7. Automatic Parking Barrier Control

**Objective:** Design an FSM-based automatic parking barrier controller.

-   Inputs include vehicle detection, payment confirmation, reset, and
    clock.
-   The controller waits for payment before opening the barrier.
-   It monitors vehicle movement and includes a safety response if a
    vehicle is detected during closing.
-   Focus: state transitions, next-state logic, output decoding, and
    status indicators.

**Circuit:**
[`Experiment-07-Parking-Barrier.circ`](circuits/Experiment-07-Parking-Barrier.circ)

### 8. 4-Bit Mini-ALU and Program Counter

**Objective:** Implement a 4-bit arithmetic datapath and a 4-bit
synchronous program counter.

-   The Mini-ALU supports addition and subtraction using mode-controlled
    logic.
-   The datapath uses registers and multiplexers for operand selection
    and write-back.
-   The Program Counter increments synchronously under enable control.
-   Focus: arithmetic hardware, register-based datapaths, and mapping
    program operations to hardware blocks.

**Circuit:**
[`Experiment-08-Mini-ALU-Program-Counter.circ`](circuits/Experiment-08-Mini-ALU-Program-Counter.circ)

### 9. AI-Assisted Code-to-Gate Explainer

**Objective:** Explain how a high-level conditional statement can be
represented using digital hardware and verify the resulting logic.

-   Code concept: select the greater of two 2-bit values.
-   Hardware mapping: a 2-bit magnitude comparator controls two 2:1
    multiplexers.
-   Focus: code-to-hardware mapping, gate-level multiplexer design,
    truth-table verification, and critical evaluation of AI-generated
    designs.

**Circuit:**
[`Experiment-09-Code-to-Gate.circ`](circuits/Experiment-09-Code-to-Gate.circ)

------------------------------------------------------------------------

## Tools and Technologies

-   **Logisim / Logisim Evolution** --- digital logic design and circuit
    simulation.
-   **ChatGPT / Gemini** --- AI-assisted design exploration,
    explanation, and debugging in selected experiments.
-   **Digital logic concepts** --- Boolean algebra, K-maps,
    combinational circuits, FSMs, flip-flops, counters, registers,
    multiplexers, and ALU datapaths.

## Repository Structure

Suggested layout:

``` text
Digital-Electronics-Lab/
│
├── README.md
├── report/
│   └── FINAL_DE.pdf
│
├── circuits/
│   ├── Experiment-01-Boolean-Simplifier.circ
│   ├── Experiment-02-Natural-Language-Logic.circ
│   ├── Experiment-03-Traffic-Light-FSM.circ
│   ├── Experiment-04-Fault-Detection.circ
│   ├── Experiment-05-Digital-Clock.circ
│   ├── Experiment-06-Sequential-Blocks.circ
│   ├── Experiment-07-Parking-Barrier.circ
│   ├── Experiment-08-Mini-ALU-Program-Counter.circ
│   └── Experiment-09-Code-to-Gate.circ
│
└── images/
    └── (optional circuit screenshots)
```

The structure is a recommendation. Keep only files that are actually
present in the repository and update the links if your folder or
filenames differ.

## How to Open the Circuits

1.  Install and open **Logisim Evolution** (or the Logisim version used
    to create the circuit).
2.  Open the required `.circ` file from the `circuits/` folder.
3.  Inspect the inputs, outputs, and circuit components.
4.  Change input pins or clock signals to test the circuit.
5.  Compare the observed output with the truth table or expected
    behaviour in the corresponding experiment report.

## Learning Outcomes

Through these assignments, this portfolio documents practice in:

-   Simplifying Boolean functions and reducing gate-level complexity.
-   Translating written system requirements into Boolean expressions.
-   Designing and analysing finite state machines.
-   Understanding sequential logic, flip-flops, counters, and shift
    registers.
-   Building practical control systems using digital logic.
-   Relating software-level operations to hardware datapaths and control
    circuits.
-   Testing, debugging, and validating circuits through simulation.
-   Using AI tools as assistance while checking the resulting designs
    against digital logic principles.

------------------------------------------------------------------------

*This repository is an academic laboratory portfolio prepared for
Digital Electronics Laboratory (ESC392) at the Institute of Engineering
& Management, Kolkata.*
