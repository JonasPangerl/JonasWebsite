# Boundary Layer Meshing Setup Tool

*An interactive, browser-based tool to design boundary-layer (BL) meshes quickly and scientifically, before you spend time on full meshing runs.*

---

## Use the tool online

**No installation required** — the tool runs entirely in your browser:

**[:material-open-in-new: Launch the BL Meshing Setup Tool](https://jonaspangerl.github.io/BL_Meshing_Setup_Tool/){ .md-button .md-button--primary target="_blank" }**

Want to explore the source code or contribute?  
**[:material-github: View on GitHub](https://github.com/JonasPangerl/BL_Meshing_Setup_Tool){ .md-button target="_blank" }**

---

## What it is
This tool helps you determine **optimal boundary-layer mesh parameters** in minutes.  
It visualizes and computes all relevant near-wall settings **in real time**, so you can pick robust values without waiting for a full meshing job.

- Works great alongside **OpenFOAM** and **STAR-CCM+** (and similar tools).
- Focuses on **external freestream flows** with Reynolds numbers ~**10⁴–10⁷**.
- Based on **turbulent flat-plate** theory for BL thickness and skin friction.

---

## Why this helps
If you’ve ever spent hours “dialing in” BL settings for a CFD case, you know the pain:
- Picking the **first cell height** to hit your target **y⁺**,
- Choosing the right **BL thickness** and **number of layers**,
- Setting a **geometric growth (stretch) factor**,
- Ensuring a smooth **transition to the volume mesh**.

This tool answers those questions **instantly** with live plots and metrics, so you can iterate scientifically—not by guesswork.

---

## What it calculates & shows
- **Target y⁺** → suggests **first cell height** at the wall.
- **Boundary-layer thickness** (theoretical) at a chosen station.
- **Number of BL layers** and **geometric stretch** between layers.
- **Transition** from BL mesh to volume mesh (**first volume cell size**).
- **Log-scale y⁺ plot** and a **mesh sketch** for quick sanity checks.
- **Layer distribution** across viscous sublayer, buffer, and log region.

The output parameters can be plugged into **STAR-CCM+**, **OpenFOAM**, **ANSYS**, **ANSA**, …  

---

## Typical workflow
1. **Set flow conditions** (U∞, ν, characteristic length / Re).
2. **Choose target y⁺** → tool proposes **first cell height**.
3. **Pick BL thickness** & **number of layers**; adjust **stretch factor**.
4. Inspect the **preview plots** (mesh sketch + y⁺ log plot).
5. Export or note the final set of **mesh parameters**.

---

## Parameters at a glance

| Parameter | Meaning / Use |
|---|---|
| **Target y⁺** | Near-wall resolution objective (e.g., 1 for low-Re models, 30–100 for wall functions). |
| **First Cell Height** | Calculated wall-adjacent cell size to hit the target y⁺. |
| **BL Thickness** | Theoretical boundary-layer thickness at your station. |
| **Number of Layers** | Layers in the BL block (sets resolution normal to the wall). |
| **Geometric Stretch** | Growth factor between successive layers (controls smoothness/stability). |
| **First Volume Cell Size** | Cell height immediately after BL block, ensuring smooth transition. |

---

## Assumptions & limits
- Uses **turbulent flat-plate** correlations → a **first estimate** for real geometries.
- Local **skin friction, velocity, pressure gradients** in your final flow field may differ.  
  Expect to **tune** values once you see first results from your CFD mesh/solution.
- Best suited for **external flows** in **Re ≈ 10⁴–10⁷**.

!!! note
    The tool is designed to **narrow the search** for workable BL parameters before you invest time in heavy meshing/solving. Use it to **bracket** sensible settings fast.

---

## Legacy desktop version (deprecated)

!!! warning "Deprecated"
    The standalone Python desktop application is no longer actively maintained. Use the [browser-based version](https://jonaspangerl.github.io/BL_Meshing_Setup_Tool/) instead.

The original Windows executable is still available on the [Downloads Page](downloads.md) if you need offline access.

---

## Compatibility
- **CFD tools:** OpenFOAM, STAR-CCM+, ANSYS/Fluent, ANSA (parameter transfer by hand or scripts).
- **Browser:** Any modern browser (Chrome, Firefox, Edge, Safari) — no plugins or installation needed.

---

## Contact
Questions, feedback, or feature requests? I’m happy to help—also available for **consulting** around **aerodynamic development** and **Python tooling**.

