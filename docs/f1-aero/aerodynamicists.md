# Aero Development

When people say F1 aero development, they usually refer to the work of **Aerodynamicists**. These engineers create and evolve concepts, build parts in a **CAD** environment, often with support from **Surfacers**, run **CFD** through automated pipelines, and evaluate results to decide the next steps. The goal is to shape the flow field around the car so that downforce goes up, drag goes down, and sensitivities move in a helpful direction.

## Typical workflow, concept to decision
1. **Idea and intent**, define a flow objective, for example a stronger floor sealing vortex, a cleaner front wheel wake, a more stable diffuser structure  
2. **CAD surfaces**, create water tight surfaces that express the idea, keep packaging and legality in mind, request surfacing support where useful  
3. **CFD release**, place the option into a fully automated CFD process
4. **Post processing**, review forces and moments, surface pressure and total pressure, flow structures and vortex criteria, compare with a clean reference  
5. **Multi condition view**, inspect the option across relevant ride heights, yaws, steering, rake, front and rear heights
6. **Decision**, refine and loop, or prepare a **WT release**, or drop the concept if evidence is weak

## Conditions and sensitivities
F1 parts can behave very differently across conditions. A floor edge that helps at low ride height can be neutral or negative at
high ride height, a front wing tweak that looks good at zero yaw can hurt at high yaw. Aero development therefore balances
overall load levels and drag,
gradients across ride height, yaw, steer, speed,
robustness to setup variation.

## Reading the data
Aerodynamicists look at

* **Forces and moments**, trends and deltas against a stable reference
* **Surface fields**, pressure coefficient and total pressure, separation lines, attachment quality  
* **Volume fields**, vortex cores, shear layers, losses, ...
* **Diagnostics**, numerical and aerodynamic health, reference alignment for correlation

## Wind tunnel handover and testing
After several CFD iterations the option can go to the **wind tunnel**. Aerodynamicists hand water tight surfaces to **Model Design**, 
which splits and prepares parts for the WT model. Depending on the team, aerodynamicists may also cover WT shifts, 
or a dedicated WT group runs the plan. 
Results return to the aero development owner for analysis and a decision, release to track, iterate, or stop.

## Correlation mindset
Aero development checks how **CFD** predictions compare with **WT**. Differences can point to modelling gaps, measurement limits, or concept sensitivity. Good notes and clean comparisons make later decisions faster.

## Collaboration touchpoints
* **Surfacers**, help turn quick design intent into clean surfaces  
* **CFD group**, keeps pipelines reliable, advises on meshing and numerics, maintains standards  
* **Model Design**, translates surfaces into WT hardware, plans splits, interfaces, stiffness  
* **WT testing**, executes plans, controls change times, secures repeatability  
* **Aero Performance**, provides track context and priorities

## Skills and interests checklist
* Strong **CAD** fundamentals, comfortable building clean, water tight surfaces  
* Practical **CFD** literacy, release options into automated workflows, read field data with purpose  
* Curiosity for **flow physics**, ability to form testable hypotheses  
* Statistical sense for **multi condition** behaviour, read gradients, not only single points  
* Clear **communication**, concise plots and notes, evidence you and others can act on  
* Planning ability for **WT releases**, understanding of constraints and measurement options
