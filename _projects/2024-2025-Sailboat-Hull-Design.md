---
layout: project
title: Sailboat Hull Design and Manufacturing
description: Advanced Composites and Naval Architecture Project
technologies: [Composite sandwhich, CNC, Solidworks]
image: /assets/images/hullCompleteBoat.JPG
---

- Cornell University's Autonomous Sailboat team (CUSAIL) required a sailboat hull to be designed and manufactured for their boat in the 2024-2025 season. This would become the msot successfull hull seen from the team and design process is detailed below. 

## Naval Architecture

- The hull design, named ”Flat Stanley”, was chosen from a miniature model competition. Several hull shapes were tested in a pool, and Flat Stanley outperformed its competitors. In particular, the flat shape of the hull seen in Figure 1 drastically improved form stability and eliminated heeling. Excessive heeling has been a recurring problem in past years which opted for thinner designs. Due to the heeling, prior boats required substantial ballast weight that encumbered performance.

![Figure 1]({{ "assets/images/Figure1-HullGeometry.JPG" | relative_url }}){: class="half-width"}

## Composite Design

- To optimize the strength and minimize weight, the hull is designed as a composite and foam core shell. To determine the composite structure we will focus on the least supported panel, the midship section between bulkheads. Here, it is critical that hull integrity is maintained under the slam pressure encountered in poor weather conditions. The midship panel is treated as a simply supported beam, with a tributary width equal to the arclength at the widest section. A uniform distributed load is calculated using the slam pressure and the set tributary width. The bending stiffness of a prospective composite structure is evaluated based on core and face thickness. Then, bending deflection, maximum bending moment, transversal shear and bending stress can be determined. Safety factors are implemented into the magnitude of slam pressure and the strength of the material. Finally, other failure modes such as fatigue failure are evaluated and all figures and calculations are shown in Appendix E. The final composite design includes a core thickness of 6.36 mm and a fiberglass thickness of  0.267 mm. 

## Plug Creation

![Figure 2]({{ "assets/images/HullFig2.JPG" | relative_url }}){: class="half-width algin-left"}

To manufacture the hull, a positive model of the hull, called a plug, is CNC machined. Then a negative mold can be created by performing a layup over the plug. High-density machinable foam was CNC cut to the shape of the hull. The plug, seen in figure 2, was cut to specifications and with satisfactory quality. The plug was cut in two halves that could be placed together with locating dowels. To create one solid plug, JB Weld is used to glue the two halves and locating dowels into place. Afterwards, the seam between the two pieces was filled in with Plaster of Paris as seen in figure 3. 

![Figure 3]({{ "assets/images/HullFig3.JPG" | relative_url }}){: class="half-width"}

After combining the two halves of the plug, roughly six layers of Duratec primer were sprayed onto the plug as described in Appendix A. In between layers of Duratec, a brief sanding was done to remove any surface imperfections that would translate into the next coat. This practice provided satisfactory results, however the foam plug initially had machining lines that were visible in the plug as seen in figure 4. Extensive sanding was required through the Duratec to remove these lines, which could have been easily removed with sanding prior to applying the Duratec. For future practice, the plug should be sanding smooth with a low-grit sandpaper prior to any application of Duratec. After the final coat of primer, sanding was conducted using the procedure listed in Appendix B. The final result of the plug, seen in figure 5, was considered satisfactory.

![](/assets/images/HullFig4.JPG)

![](/assets/images/HullFig5.JPG)

## Mold Creation

To create a negative mold for the hull, a gel coat and layers of fiberglass would be applied on top of the plug. First, 8 layers of wax were applied to the surface of the plug. The wax increases the surface finish of the plug and also acts as a release agent for the subsequent layers. After the wax, modeling clay was used to seal the gap between the plug and the board it was placed on as seen in figure 6. The gap between the plug and board is sealed to stop resin from leaking under the plug and increasing the difficulty of mold release. The plug was then moved into the spray booth, where a layer of PVA release film was sprayed onto the plug. After the PVA had dried, a tooling gel coat was applied to the plug using the gel coat spray gun. Figure 7 shows the plug after applications of PVA and gel coat. For details on spraying gel coat, see Appendix C. A thickness gauge was used to target a total thickness of 15 mils (thousandth of an inch). Then, the gel coat was allowed to set for roughly 30-45 minutes before fiberglass was laid in. Allowing the gel coat to become tacky improves the bond between the gel coat and fiberglass. Not giving enough time for the gel coat to set will cause it to mix with the laminating resin, creating unsatisfactory results. Two layers of 7 oz fiberglass were placed behind the gel coat. Paper templates had been cut out and placed over the plug to ensure wrinkles did not form in the complex curves. These templates were used to cut the fiberglass which prevented wrinkles and easier to lay into the mold. At the stern, significant work was required to ensure the fiberglass conformed to that area. The fiberglass often peeled up from the 90 degree bend and required creative use of resin and extra strips of fiberglass to keep everything in place. With all of the composite materials laid and saturated with resin, a vacuum bag was used to ensure close fitment to the plug. Details of how to perform a vacuum bag are included in Appendix D. 

![](/assets/images/HullFig6.JPG)
![](/assets/images/HullFig7.JPG)

## Hull Creation

First, release agents such as wax and PVA were applied, the gel coat was sprayed in, then fiberglass was laid and saturated. Three layers of 2 oz fiberglass were initially used for the layup. Afterwards, a layer of 7 oz fiberglass and strips of carbon fiber were used to stiffen the hull in high stress areas such as the bow, keel connection, and underbelly. The hull after its release from the mold, is seen in figure 9.

![](/assets/images/HullFig9.JPG)

![](/assets/images/HullBOM.JPG)

## Appendix A - How to spray Duratec Surface Primer

1. Put 300 grams of Duratec gray surface primer into a mixing cup. 
2. Add 10 percent acetone and 1 percent methyl ethyl ketone peroxide (MEKP) by mass. 
3. Mix thoroughly with a popsicle stick. 
4. Pour the Duratec mixture into a spray gun, and using the spray gun, paint the part with the Duratec. Alternate horizontal and vertical spraying motions. Don’t start a new stream of spray directly on the part. Start a new spray away from the part and then bring the gun toward the part
5. Paint in a paint booth with ventilation on until Duratec runs out.
6. Let the Duratec dry for at least 24 hours before handling and or sanding the part

## Appendix B - How to sand Duratec Surface Primer

 1. Put 80 grit sanding paper on a sanding block. 
 2. Sand until the entirety of the part has scratch lines going in a single direction. 
 3. Sand again until the entirety of the part has scratch lines going perpendicular to the original direction. 
 4. Repeat steps 1-3, increasing the sandpaper grit each time to 120, 200, 400, 600, 800, and eventually to 1000 grit sandpaper. 
 5. Dunk 1500 grit sandpaper in water and continue to sand the part adding water when needed. At this point there will not be scratch lines but still sand the part in the same way as if there were scratch lines (sand in one direction thoroughly and then again perpendicular to the original direction). 
 6. Repeat step 5 with 2000 grit sandpaper. 
 7. Using wet paper towels, remove all excess Duratec ‘dust’ from part. The part should have a shiny, reflective, mirror finish.

## Appendix C - How to spray gel coat

 1. Put 300 grams of gel coat into the gel coat cup gun disposable cup 
 2. If high gloss desired, add Duratec high gloss additive. 
 3. Add 2 percent MEKP as hardener to the mix 
 4. Mix thoroughly with a Popsicle stick. 
 5. Place cap over disposable cup and place inside Cup Gun with 2.5- 4 mm nozzle 
 6. Paint in paint booth with ventilation 
 7. Let gel coat dry for roughly 30 minutes before placing fiberglass

## Appendix D - How to Vacuum Bag
1. Set up an area on a solid, flat table or sheet of acrylic or metal about twice as large as the part. 
2. Place a sheet of Breather/Bleeder fabric that is just slightly larger than the part on the part.
3. Place a sheet of release fabric that is just slightly larger than the part over the Breather/Bleeder fabric. 
4. Cover the whole thing with bagging fabric with lots of extra room around the part. 
5. Place the bottom vacuum attachment on the release fabric. 
6. Use double sided yellow tape to create a vacuum by sticking the tape to the table and the bagging fabric. 
7. Cut a small hole in the bagging fabric where the bottom of the vacuum attachment is. 
8. Attach the rest of the vacuum attachment and the vacuum, and turn on the vacuum. 
9. Make sure there is release and bagging fabric between both parts of the vacuum attachment.

## Appendix E - Composite Design Calculations and Figures

The following figures are generated using a model that focuses on loading due to hull slam pressure. The geometry focuses on the largest unsupported panel (of length L) in the composite strucutre, and trats it as a flat sheet. This model was chosen becuase it introduces conservatisim into the design. Both bending (Euler Bernoulli) and shear (Timoshenko) deflection were accounted for to calculate bending moments and shear forces. A deflection target of L/200 was chosen based off of maritime standards. 

![](/assets/images/hullAppendix A.jpg.JPG)

### Meaningful deductions

Based on Figure E1, which assumes a nominal face thickness of 0.24 mm, the required core thickness to reach out target deflection is 6.24 mm. The foam we will use is Divinycell DIVINYMAT due to its effectiveness with vacuum bagging. Each layer is 3.18 mm thick so to reach our target deflection two layers will be used for a 6.36 mm thick core. The shear deflection share (what percentage of deflection is caused by shear) is plotted in Figure E2. To maintain model assumptions, we need to ensure the panel will have bending-dominated behavior. At a core thickness of 6.36 mm the shear deflection share is still low (< 25%) and our panel will have bending-dominated behavior. As seen in Figure E3, at a core thickness of 6.36 mm the maximum shear in the core is significantly below the maximum allowable shear stress. The heat map shown in figure E4 provides a convenient way to choose face thickness based on the target deflection and your set core thickness. Here, a face thickness of 0.26 mm allows us to reach our deflection limit while operating at the allowable face stress during slamming. Using three layers of 2 oz fiberglass, a face thickness of 0.267 mm will be achieved. As seen in Figure E5, our current face and core thicknesses produce a maximum face stress well below the allowable amount.

To assess fatigue failure due to bending stress the SN curve in Figure E6 [Reference 4] is used. For a face thickness of 0.267 mm and core thickness of 6.36 mm we encounter a face stress magnitude of 26.62 MPa. At that stress magnitude, over 10^6 cycles are required to fail. Considering the hull will only be used for 2 months fatigue failure from bending stress is unlikely to occur. Since the core shear stress is below 25% of our allowable stress, it is again unlikely for fatigue failure for shear stress to occur. 

![](/assets/images/hullSNcurve A.jpg.JPG)

## References

[1] Germanisher Lloyd, Rules and Guidelines 2008 - I Ship Technology, Part 3 Special Craft Section Chapter 3 (updated 2003), 2008.

[2] Birman V, Bert CW. On the Choice of Shear Correction Factor in Sandwich Structures. Journal of Sandwich Structures & Materials. 2002;4(1):83-95. doi:10.1177/1099636202004001180

[3] International Organization for Standardization. (2019). ISO 12215-5:2019 Small craft—Hull construction and scantlings—Part 5: Design pressures for monohulls, design stresses, scantlings determination. ISO.

[4] Izadi Gonabadi, H., Oila, A., & Bull, S. J. (2016). Fatigue of sandwich composites in air and seawater. Journal of Bio- and Tribo-Corrosion, 2(2), 10. https://doi.org/10.1007/s40735-016-0043-2
