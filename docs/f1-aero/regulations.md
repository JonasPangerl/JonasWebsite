# Regulations, what frames F1 aero work

This page summarises where the rules live and how they constrain day-to-day aero work. The **Formula One Sporting Regulations** and the **Technical Regulations** define the car’s aerodynamic rules, how parts may deflect and what loads they must withstand under specified conditions, how testing is performed and limited, and how **wind tunnel** and **CFD** activities are controlled and measured.

---

## Testing periods, how allocations are handed out

Aerodynamic testing, both **WT** and **CFD**, is restricted by an **Aerodynamic Testing Regulations** period (**ATR**).
An ATR period is typically about **eight weeks**.
Each team receives an allowance per period that scales with championship position, teams further back receive more allocation,
teams at the front receive less. The counters above, runs, wind on time, occupancy, must all fit within that allowance.

---

## Wind tunnel testing

Wind tunnel activity is bounded by three counters, the goal is to extract maximum information per plan while staying within the allocation.
The WT model is limited to a 60% scale model and the maximum windspeed to 50m/s.

### 1) Runs
A **run** is counted when the speed in the test section rises above a defined threshold and, at the next time it falls back below the threshold, that completes one run. Teams are allowed only a certain number of runs per **ATR** period.

### 2) Wind on time
**Wind on time** is the accumulated time while the test section speed is above the threshold. Every second above that threshold adds to the counter, the total wind on time per period is limited.

### 3) Occupancy
**Occupancy** is the time spent working on the tunnel model and rig, even when the wind is off. This time is also limited, so planning and short change times are essential.

---

## CFD testing

CFD activity is controlled by the declared compute resource and by counters that measure numerical effort and geometry change.

### Declared resource
Each team declares a **HPC resource** to the FIA, activity runs on that resource and is monitored.

### MAUH, numerical effort
**MAUH** (Mega Allocation Unit Hours) represents the numerical effort available within one ATR period. You budget this across your simulations. More efficient setups and numerics let you run more conditions within the same MAUH, heavier models reduce the count but may give deeper insight.

### RATG, restricted aerodynamic testing geometry
**RATG** counts surface geometry changes. One RATG is counted when the surface mesh changes by more than **0.5 mm**. Geometry changes are limited per period, for example on the order of **~2000 RATGs** in 2025. The more efficiently you run, the more **driving conditions** you can simulate per RATG, or you spend MAUH on higher-fidelity studies such as **LES** or **DES** instead of more **RANS** conditions.

---

## Why all of this matters, process efficiency

These constraints make **efficient, automated processes** mandatory, from CAD to meshing to run control to post-processing and correlation. Teams aim to

* minimise change and setup times,
* standardise and template common steps,
* maximise useful data recorded per run and per simulation,
* align CFD and WT conditions so correlation is quick and trustworthy.
