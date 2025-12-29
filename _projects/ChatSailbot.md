---
layout: project
title: "Fiberglass Sailboat Hull"
description: "Advanced composites and naval architecture design for Cornell University's autonomous sailboat."
technologies:
  - Composite sandwich structures
  - CNC machining
  - SolidWorks
image: /assets/images/hullCompleteBoat.JPG
---

# Fiberglass Sailboat Hull Design & Manufacturing
*Advanced Composites and Naval Architecture Project*

## Project Overview

Cornell University’s Autonomous Sailboat Team (CUSail) required a new sailboat hull for the 2024–2025 competition season. The resulting design became the **most successful hull produced by the team to date**, achieving improved stability, reduced ballast requirements, and enhanced manufacturability. The full design and fabrication process is detailed below.

---

## Naval Architecture

The hull design, named **“Flat Stanley,”** was selected through a miniature model competition in which several hull geometries were tested in a pool environment. Flat Stanley outperformed competing designs, primarily due to its **flat hull geometry**, which significantly improved form stability and eliminated excessive heeling.

Excessive heeling had been a recurring issue in previous seasons, particularly with thinner hull designs. Those designs required substantial ballast to maintain stability, which negatively impacted performance. The Flat Stanley geometry mitigated this issue, reducing ballast requirements while maintaining stability.

<figure class="project-figure align-right">
  <img src="{{ 'assets/images/Figure1-HullGeometry.JPG' | relative_url }}" alt="Hull geometry comparison">
  <figcaption><strong>Figure 1.</strong> Hull geometry showing flat-bottom design improving form stability.</figcaption>
</figure>

---

## Composite Design

To optimize strength while minimizing weight, the hull was designed as a **fiberglass composite sandwich structure with a foam core**. Structural analysis focused on the **least supported midship panel** between bulkheads, which experiences the highest loading under slam pressure during rough conditions.

The midship panel was modeled as a **simply supported beam** with tributary width equal to the arclength at the widest section. A uniformly distributed load was calculated from estimated slam pressure. Bending stiffness was evaluated as a function of face and core thickness, enabling determination of deflection, bending moment, shear forces, and stresses.

Safety factors were applied to both slam pressure magnitude and material strength. Additional failure modes, including fatigue, were evaluated. All calculations and supporting figures are included in **Appendix E**.

The final composite design consists of:
- **Core thickness:** 6.36 mm  
- **Fiberglass face thickness:** 0.267 mm  

---

## Plug Creation

To manufacture the hull, a **positive plug** was CNC machined from high-density machinable foam. The plug was produced in two halves and aligned using locating dowels before being bonded together using JB Weld.

After assembly, the seam between the two halves was filled using **Plaster of Paris** to create a continuous surface.

<figure class="project-figure align-right">
  <img src="{{ 'assets/images/HullFig2.JPG' | relative_url }}" alt="CNC machined hull plug">
  <figcaption><strong>Figure 2.</strong> CNC-machined foam plug prior to surface finishing.</figcaption>
</figure>

<figure class="project-figure align-right">
  <img src="{{ 'assets/images/hullFig3.JPG' | relative_url }}" alt="Plug seam filling">
  <figcaption><strong>Figure 3.</strong> Seam between plug halves filled prior to priming.</figcaption>
</figure>

Approximately six layers of **Duratec surface primer** were applied, with light sanding between coats to remove surface imperfections. Initial machining lines in the foam plug remained visible after early primer coats, requiring extensive sanding. In future iterations, sanding the foam plug prior to primer application is recommended.

The final plug surface finish was achieved following the sanding procedure outlined in **Appendix B**.

<figure class="project-figure">
  <img src="{{ 'assets/images/hullFig4.JPG' | relative_url }}" alt="Duratec primer sanding">
  <figcaption><strong>Figure 4.</strong> Visible machining lines after initial primer application.</figcaption>
</figure>

<figure class="project-figure">
  <img src="{{ 'assets/images/hullfig5.JPG' | relative_url }}" alt="Final finished plug">
  <figcaption><strong>Figure 5.</strong> Final finished plug ready for mold creation.</figcaption>
</figure>

---

## Mold Creation

A **negative fiberglass mold** was created over the finished plug. Eight layers of wax were applied to improve surface finish and act as a release agent. Modeling clay was used to seal the gap between the plug and mounting board, preventing resin leakage.

After waxing, a layer of **PVA release film** was sprayed onto the plug, followed by a tooling gel coat. A thickness gauge was used to achieve a total gel coat thickness of approximately **15 mils**.

Once the gel coat became tacky, two layers of **7 oz fiberglass** were laid using paper templates to avoid wrinkling in complex curvature regions, particularly near the stern. Additional fiberglass strips and resin were used to ensure conformity in high-curvature areas.

The mold layup was vacuum bagged to ensure proper consolidation. Full vacuum bagging procedures are detailed in **Appendix D**.

<figure class="project-figure">
  <img src="{{ 'assets/images/hullfig6.JPG' | relative_url }}" alt="Clay sealing and mold prep">
  <figcaption><strong>Figure 6.</strong> Plug sealed to board prior to gel coat application.</figcaption>
</figure>

<figure class="project-figure large">
  <img src="{{ 'assets/images/hullfig7.JPG' | relative_url }}" alt="Gel coat and fiberglass layers">
  <figcaption><strong>Figure 7.</strong> Plug after application of PVA release film and gel coat.</figcaption>
</figure>

---

## Hull Creation

For final hull fabrication, release agents were applied to the mold before spraying gel coat. The structural layup consisted of:
- Three layers of **2 oz fiberglass**
- One layer of **7 oz fiberglass**
- Carbon fiber reinforcement in high-stress regions including the bow, keel interface, and underbelly

The completed hull was released successfully from the mold and met all structural and geometric requirements.

<figure class="project-figure large">
  <img src="{{ 'assets/images/hullfig9.JPG' | relative_url }}" alt="Finished fiberglass hull">
  <figcaption><strong>Figure 8.</strong> Completed fiberglass hull after mold release.</figcaption>
</figure>

<figure class="project-figure large">
  <img src="{{ 'assets/images/HullBOM.JPG' | relative_url }}" alt="Hull bill of materials">
  <figcaption><strong>Figure 9.</strong> Bill of materials for hull fabrication.</figcaption>
</figure>

---

## Appendices

The following appendices document **manufacturing procedures, composite analysis, and fatigue validation** used to support the hull design:

- **Appendix A:** Spraying Duratec Surface Primer  
- **Appendix B:** Sanding Duratec Surface Primer  
- **Appendix C:** Spraying Gel Coat  
- **Appendix D:** Vacuum Bagging Procedure  
- **Appendix E:** Composite Design Calculations and Figures  

(Procedures and calculations retained verbatim below.)