---
layout: project
title: "Wind Turbine Blade Design"
year: 2025
description: "Design and testing of a scale-model wind turbine blade optimized for torque at extremely low Reynolds numbers.
technologies: [Blade element theory, ANSYS Fluent CFD, structural validation,  wind tunnel testing]
featured: true
image: /assets/images/blade.png
---

# Torque-Optimized Wind Turbine Blade  
### Low-Re Aerodynamics, CFD, and Experimental Validation

This project documents my work designing, analyzing, and testing a **small-scale wind turbine blade optimized for torque production** in an extremely low Reynolds number regime. The design emphasizes **startup torque, low-speed operation, and experimental feasibility**, rather than peak aerodynamic efficiency, reflecting real-world constraints encountered in small-scale energy systems.

The workflow integrates **blade element momentum theory, CAD modeling, CFD simulation in ANSYS Fluent, structural safety analysis, and physical wind tunnel testing**, with iterative refinement driven by both modeling insight and experimental limitations.

---

## Design Context and Objectives

The blade was designed for operation in the **Big Blue wind tunnel**, characterized by a Weibull wind distribution with a mean wind speed of approximately 4.6 m/s. Given a maximum chord of 2 inches and air kinematic viscosity of 1.5×10⁻⁵ m²/s, the blade operates in a **Reynolds number range of roughly 9,300–21,000**, where conventional NACA airfoils perform poorly due to laminar separation.

**Primary objectives:**
- Maximize **torque output** across the expected wind distribution  
- Achieve reliable **startup and low-speed operation**  
- Remain within **geometric, structural, and testing constraints**  
- Validate aerodynamic behavior using **CFD and experiment**

---

## Airfoil Selection and Aerodynamic Rationale

A comparative evaluation of low-Re airfoils identified the **S1223 airfoil** as the optimal choice. Unlike conventional sections, the S1223 achieves **exceptionally high lift coefficients (CL ≈ 1.8–2.0)** in the relevant Reynolds range and exhibits **gentle stall behavior**, which is critical for stable torque production during startup and off-design operation.

![Figure 1]({{ "assets/images/s1223.JPG" | relative_url }}){: class="project-image align-right"}
*Figure 1: Lift coefficient vs. angle of attack comparison at low Reynolds number.*

---

## Blade Geometry and Torque Optimization

The blade was designed around a **low tip-speed ratio (λ = 3)** to intentionally rotate the lift vector toward the tangential direction, increasing torque at the expense of peak efficiency. Blade element momentum theory guided the geometry:

- **Linear chord taper:** 2.0 in (root) → 0.4 in (tip)  
- **Strong twist distribution:** ~60° at root → ~14° near tip  
- **Target angle of attack:** ≈ 3° across the span  

This geometry prioritizes torque generation while maintaining structural robustness and manufacturability.

![Figure 2]({{ "assets/images/torque.JPG" | relative_url }}){: class="project-image align-right"}
*Figure 2: Predicted rotor torque vs. expected wind speeds*

---

## Structural Validation

Structural safety was assessed using MATLAB-based bending moment calculations derived from distributed aerodynamic loads. Accura 25 SLA material properties were used to verify that stresses remained well below allowable limits.



![Figure 3]({{ "assets/images/bend.JPG" | relative_url }}){: class="project-image align-right"}
*Figure 3: Root bending moment and structural safety margin.*

The predicted **failure wind speed of ~68 m/s** provides more than a **10× safety margin** over expected operating conditions.

---

## CAD Modeling and Manufacturing Challenges

The blade was modeled in **SolidWorks** using multiple airfoil cross-sections lofted along the span. Early CAD iterations revealed practical issues related to **trailing edge closure, STL integrity, and hub geometry**, which affected both printing and CFD usability.


![Figure 4]({{ "assets/images/cad.JPG" | relative_url }}){: class="project-image align-right"}
*Figure 4: Final closed CAD geometry used for CFD analysis.*

These challenges required manual airfoil data cleanup and segmented lofting, introducing minor geometric discontinuities that were deemed negligible for aerodynamic analysis.

---

## CFD Methodology (ANSYS Fluent)

### Geometry and Domain
The CFD model used a **120° periodic wedge domain** to reduce computational cost while capturing rotational flow physics.


### Meshing
A refined surface and polyhedral volume mesh balanced near-wall resolution with manageable runtime.

![Figure 5]({{ "assets/images/mesh.JPG" | relative_url }}){: class="project-image align-right"}
*Figure 5: Volume mesh cross-section*

![Figure 6]({{ "assets/images/p.JPG" | relative_url }}){: class="project-image align-right"}
*Figure 6: Pressure contour along the blade surface*

![Figure 7]({{ "assets/images/p2.JPG" | relative_url }}){: class="project-image align-right"}
*Figure 7: Pressure contour across blade crossection*