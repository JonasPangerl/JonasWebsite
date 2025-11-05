# Surfacing

Surfacing engineers turn aerodynamic intent into **clean, water-tight CAD**. They understand the regulations well, they can visualise complex 3D shapes, and they know how to build robust models that can be **edited safely** by Aerodynamicists later. Input often arrives as sketches, screenshots, short briefs, or design notes, output is a surface model that fits packaging and legality and is ready for CFD and model design.

## Typical workflow
1. **Intake and brief**, clarify the idea, targets, affected zones, constraints, references  
2. **Scaffolding**, set up construction geometry, key sections, rails, wireframes, guides  
3. **Primary surfacing**, create continuous, high-quality patches, enforce curvature goals  
4. **Legality support**, run checks, add helper features for automated legality checking where useful  
5. **Robustness pass**, organise history, name features, stabilise dependencies for future edits  
6. **Handover**, deliver water-tight surfaces to Aerodynamicists, note change knobs and limits  
7. **Feedback loop**, review CFD and WT outcomes to refine patterns and standards

## What “clean CAD” means
* Water-tightness, no gaps, no inverted normals, closed volumes where required  
* Continuity, control of G0, G1, G2 as appropriate, smooth blends, no ripples  
* Topology discipline, logical patch layout, minimal and stable trim lines  
* Sensible parameterisation, editable rails and sections, protected references  
* Legality awareness, surfaces carry or respect reference planes and envelopes

## Collaboration touchpoints
* **Aerodevelopment**, translate intent into shapes, expose safe edit handles, agree naming and file structure  
* **CFD group**, ensure surfaces import cleanly, meshing tolerances make sense, fix pain points quickly  
* **Model Design**, confirm splits, flanges, inserts, minimum radii, thickness, and stiffness needs  
* **Legality and standards**, align on automated checks, shared references, and macros

## Legality and standards
Surfacing often helps by baking in or checking geometry rules.
* Maintain shared **reference geometry**, legality planes, boxes, keep-outs  
* Provide simple **check features** or layer tags so automated scripts can validate quickly  
* Keep unit systems, tolerances, naming, and layer conventions consistent

## Building for change
The best surfaces are robust against edits, because concepts evolve quickly.
* Favour **stable wireframes** and sectional control, avoid fragile chains of trims  
* Keep a **shallow history** where possible, reduce cross-part dependencies  
* Name features clearly, expose **edit parameters** for the common change requests  
* Store **before and after** variants for quick reversions and A–B comparisons

## Skills and interests checklist
* Strong CAD fundamentals, curvature control, patch layout, trimming, joining  
* Good 3D imagination and spatial reasoning, comfort working in sections and guides  
* Appreciation of **aero needs** and **meshing needs**, understand what helps CFD and WT
* Curiosity for feedback, CFD results, WT outcomes
