# CFD

The CFD group looks after the full chain from **CAD** to **post processing**. They work very closely with Software inside Aero,
in some teams both are one department, here we focus on CFD. The goal is fast, robust, and accurate simulation that Aero development 
can rely on for decisions and correlation.

## The pipeline, CAD to mesh to solve to post
1. **CAD preparation**, enforce naming and structure, export with stable references and units, simple and repeatable export macros help a lot,
2. **Meshing**, generate a robust mesh with predictable boundary layer settings and wake resolution, guardrail checks for skewness, non orthogonality, cell count, y plus targets,
3. **Solving**, choose numerics and turbulence models with fast turnaround and acceptable accuracy, monitor residuals and forces,
4. **Post processing**, create standard figures and tables, forces and moments, surface pressure and total pressure, vortex criteria and sections, all compared to a clean reference and ready to compare with WT,

## Correlation focus
Part of the team studies the differences between **CFD**, **WT**, and **track**. 
They align conditions and references, they maintain correlation cases, and they suggest setup improvements. 

## Methods and fidelity
The workhorse is **RANS**, Reynolds Averaged Navier Stokes, chosen for speed and coverage across many conditions. 
When budget allows, the team can also runs **higher fidelity** cases, for example **LES** or **DES**,
to study specific flow physics. Efficient numerics and smart meshing let you simulate more conditions per geometry, or to spend effort on fewer but deeper cases.

## Efficiency under regulations
Within an ATR period the team budgets **MAUH** for numerical effort and counts **RATG** for
geometry changes. Efficient pipelines allow

* more conditions per RATG when running RANS,
* or the use of LES and DES on selected flows where the extra insight is worth the cost,
* 
Either way, reliable automation and templated setups are essential.


## Tooling
Teams commonly use **OpenFOAM**, some also run **STARCCM+** or **Ansys Fluent**. 


## Skills and interests

* Strong **CFD fundamentals**, numerics, turbulence modelling,
* Scripting, data handling, automation, plotting,
* **Basic understanding** of the **flow physics**,
* Familiarity with **OpenFOAM** is a strong plus at most teams, data analytics skills are very useful.

