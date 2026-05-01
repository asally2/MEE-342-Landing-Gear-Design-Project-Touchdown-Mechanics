# Design and Analysis of F-14 Landing Gear System

MEE 342: Principles of Mechanical Design  
## Touchdown Mechanics  

Aditya Sally, Anuj Shastry, Emily Lopez, Joshua Raya, Kevin Ruiz Lopez, Sanad Dababneh  
Yi Ren  
May 1, 2026  

---

# Table of Contents

1. Introduction  
2. Fabrication Process and Parameters  
 2.1 Material Selection and Filament Properties   
 2.2 3D Printer Specifications  
 2.3 Print Settings and Build Parameters  
 2.4 Iterations and Reprints  
 2.5 Slicing Tolerances and Printer Accuracy  
3. Assembly Procedure and Integration  
 3.1 Step-by-Step Assembly Process  
 3.2 Fitment and Alignment Considerations  
 3.3 Challenges Encountered During Assembly  
 3.4 Solutions and Workarounds Implemented  
4. Experimental Testing and Evaluation  
 4.1 Procedure  
 4.2 Results  
 4.3 Interpretation  
5. Comparison with Analytical and Simulation Predictions  
 5.1 Summary of Phase 2 Predictions  
 5.2 Experimental vs. Predicted Performance  
 5.3 Sources of Discrepancy  
6. Failure Analysis and Lessons Learned  
 6.1 Observed Failures and Defects  
 6.2 Root Cause Analysis  
 6.3 Design and Fabrication Mistakes  
 6.4 Unexpected Outcomes and Insights  
7. Design Improvements for Future Iterations  
 7.1 Structural and Geometric Modifications  
 7.2 Material and Manufacturing Improvements  
 7.3 Assembly and Reliability Enhancements
8. Conclusion  

---

# 1. Introduction

Aircraft landing gear systems represent one of the most critical interfaces between an aircraft and its operating environment. During takeoff, landing, and ground operations, the landing gear must support the full weight of the aircraft, absorb significant impact energy, and maintain stability under varying and often unpredictable conditions. These demands make landing gear design a multidisciplinary challenge involving structural mechanics, kinematics, materials, and reliability. This complexity is even more pronounced in military aircraft, where higher loads, aggressive operating conditions, and strict space constraints push the design further.

The Phase 1 portion of this project focused on developing the conceptual design of an F-14–inspired landing gear mechanism. This included defining the overall system layout, identifying key subsystems, and understanding the kinematic behavior required for extension, retraction, and load support. The preliminary design established how the main strut, wheel assembly, and linkage members interact, while also considering fundamental design constraints and potential failure modes.

In Phase 2, the project transitioned from concept to a detailed and realistic representation. A complete 3D CAD assembly was developed to capture the geometry of individual components, their connections, and the motion of the mechanism. Greater emphasis was placed on practical design considerations such as part dimensions, tolerances, and manufacturability using 3D printing. Engineering analyses were also introduced to evaluate stresses, fatigue behavior, and overall structural performance, providing a basis for validating the design.

Phase 3 builds upon this foundation by moving from digital design to physical realization and testing. The finalized components were fabricated using additive manufacturing, assembled into a working prototype, and evaluated under experimental conditions. This phase focuses on understanding how the real system behaves compared to predictions, highlighting discrepancies between simulation and physical performance. Observations from fabrication, assembly challenges, and testing outcomes provide critical insight into design limitations, unexpected behaviors, and areas for improvement.

## 2. Fabrication Process and Parameters

### 2.1 Material Selection and Filament Properties

The ASU print lab supports multiple filament types including PLA, PETG, TPU, and Nylon-based materials. For this project, PLA was selected due to its ease of printing, dimensional stability, and compatibility with standard lab settings.  

PLA provides:  
- Good stiffness for structural representation  
- Low warping, improving dimensional accuracy  
- Ease of support removal for complex geometries  

However, it is noted that PLA has relatively low impact resistance and temperature tolerance compared to engineering-grade materials such as Nylon or PETG. Given the objective of prototyping rather than full structural validation, PLA was considered sufficient.  

---

### 2.2 3D Printer Specifications

The ASU print lab utilizes printers compatible with 1.75 mm filament and supports a variety of materials including PLA, PETG, TPU, and Nylon variants. The maximum build volume is approximately:  

250 mm x 210 mm x 210 mm  

The printers support:  
- Breakaway Support Structures  
- Standard fused deposition modeling (FDM) processes  
- Moderate resolution suitable for functional prototypes  

---

### 2.3 Print Settings and Build Parameters

Print parameters were selected based on ASU lab defaults and adjusted for structural relevance to landing gear geometry.  

Typical settings include but are not limited to:  
- Infill: 10–20%  
- Layer height: ~0.2 mm (standard resolution)  
- Supports: Breakaway supports enabled  
- Filament diameter: 1.75 mm  

Some engineering considerations that would be included with these parameters in mind would be:  

**Infill (10–20%)**  
Chosen to reduce material usage and print time while maintaining basic internal structure. However, this limits load-bearing capability and makes the part more suitable for geometric validation rather than full mechanical testing.  

**Part Orientation**  
Critical to reduce layer-based weakness. The landing gear components were oriented to minimize stress across layer interfaces, improving resistance to bending and shear.  

**Supports**  
Required due to overhangs and complex geometry in the landing gear assembly. Breakaway supports allow easier post-processing but may affect surface finish.  

**Wall Thickness**  
Outer walls contribute more to strength than infill, so geometry was designed to rely more on shell thickness where possible.  

---

### 2.4 Iterations and Reprints

Multiple iterations were required to address dimensional accuracy and fitment issues inherent to FDM 3D printing processes. Initial prints revealed discrepancies between nominal CAD dimensions and the as-printed geometry, particularly in mating features such as hole and shaft interfaces.  

--- 

### 2.5 Slicing Tolerances and Printer Accuracy 

FDM printers such as Bambu Lab and Ender series machines exhibit dimensional deviations due to nozzle size, extrusion behavior, and thermal effects. While the nominal filament diameter is 1.75 mm, variations in extrusion and cooling lead to predictable inaccuracies:  

- Hole undersizing (internal features print smaller than designed)  
- External feature oversizing (shafts print slightly larger)  

Typical dimensional tolerances for these printers are approximately:  

±0.004 in to ±0.012 in  

Slicing software also introduces geometric approximation errors, especially in curved or small features, further affecting dimensional accuracy.

## 3. Assembly Procedure and Integration

### 3.1 Step-by-Step Assembly Process

The assembly process began with securing the base stand, which served as the primary support structure for the entire landing gear system. Establishing a stable reference frame at the start ensured proper alignment during subsequent steps.  

The main strut was first positioned and fixed onto the stand. Once secured, the wheel axle was attached to the strut, forming the central load-bearing connection. The wheel was then mounted onto the axle, completing the primary rolling interface.  

Following this, the attachment fitting for the suspension hinge was installed onto the strut assembly. The suspension hinges were then connected, allowing for vertical compliance and load absorption. Finally, the folding hinges were installed, enabling the mechanism to retract and fold inward, simulating the motion required for stowing the landing gear within an aircraft body.  

All components were connected using quarter-inch screws. While effective for prototyping, future iterations would benefit from the use of bolts and precision pins to improve stability, reduce friction, and allow smoother rotational motion.  

---

### 3.2 Fitment and Alignment Considerations

Initial assembly revealed significant fitment issues, primarily due to tight tolerances and high friction between mating components. Many parts required forceful insertion, indicating that the clearances were insufficient for a functional mechanism.  

To address this, the components were redesigned with adjusted tolerances. Additionally, the overall model was scaled up by approximately 1.5 times the original dimensions to improve manufacturability and ease of assembly. This scaling also enhanced visibility and handling during testing.  

Alignment was another major challenge in the initial build. The components did not align properly, resulting in restricted motion and instability. A redesigned version of the assembly improved alignment, and the addition of a dedicated stand further stabilized the system.  

The motion of the mechanism was initially inconsistent and “janky,” largely due to friction and misalignment. After redesigning tolerances and simplifying the structure, the motion improved, although it was still not perfectly smooth.  

---

### 3.3 Challenges Encountered During Assembly

The initial assembly attempt was largely unsuccessful, as most components did not function as intended. Tight tolerances prevented proper fitting, and the mechanism could not move freely.  

Although no major structural failures occurred, excessive friction between parts led to noticeable wear during repeated assembly attempts. Additionally, variability in print quality introduced inconsistencies in part dimensions, as the components were manufactured using shared 3D printing resources with limited calibration control.  

A significant design challenge involved the intended use of a universal joint to enable rotational motion during retraction. Due to limitations in modeling and implementation within the available timeframe, the universal joint design could not be successfully realized.  

As a result, the mechanism did not initially achieve the desired retraction behavior. This required a fundamental change in the design approach, particularly in how rotational motion was incorporated into the strut system.  

---

### 3.4 Solutions and Workarounds Implemented

To overcome the fitment issues, manual post-processing was performed on several components. Parts were sanded to reduce friction and improve fit, allowing smoother assembly and motion.  

In cases where holes became oversized or inconsistent after modification, epoxy was used to refine dimensions and achieve a better fit between mating components. This approach allowed for quick adjustments without requiring immediate reprinting.  

The most significant workaround involved redesigning the strut mechanism. Instead of using a universal joint, the strut was split into two interfacing components, allowing one part to rotate within the other. This simplified approach successfully enabled the required motion within the constraints of the project.  

Multiple redesigns and reprints were carried out to improve functionality. The assembly process was repeated approximately three times, with the first iteration failing due to excessively tight fits that prevented disassembly.  

Despite not initially incorporating spacers or washers, it was identified that their inclusion in future designs could reduce stress concentrations and improve motion smoothness.  

The most time-consuming aspect of the process was the CAD assembly in SolidWorks, where mating constraints often behaved unpredictably, requiring repeated adjustments to achieve the desired motion.

## 4. Experimental Testing and Evaluation

### 4.1 Procedure

The testing and evaluation process began with numerical simulations conducted in ANSYS. The SolidWorks model was scaled to match the dimensions of the 3D printed prototype, and corresponding loading conditions were applied to approximate those expected in the full-scale system.

A static structural analysis was performed to estimate stress distribution, deformation, and the overall factor of safety. In addition, an eigenvalue buckling analysis was conducted to verify that structural instability would not occur prior to material yielding.  

Following the simulation phase, a physical prototype was constructed by printing out all the individual components and then assembling them together. The assembly was completed using pinned joints to allow rotational motion, with adhesive applied to secure the pins in place.

Experimental testing was conducted by incrementally applying loads to the structure through the axle connected to the wheel. Loading began at low magnitudes to verify structural integrity and was gradually increased until failure occurred. This approach enabled identification of failure locations and critical load thresholds for comparison with simulation results.   

---

### 4.2 Results

The static structural analysis conducted in ANSYS provided insight into the stress distribution and deformation behavior of the system under the applied loading conditions. The results indicated that the most critical stress concentrations occurred at the lower hinge joints located near the wheel. These regions experienced the highest stresses due to their role in transferring load between the structural members and the ground interface and their relatively smaller areas.

More specifically, the maximum von Mises stress was observed at the axle–wheel interface, where the load was directly applied. This is consistent with expectations, as this location serves as the primary load bearing point and experiences both shear and bending effects. In addition to stress concentration, the simulation showed that the largest total deformation occurred at the upper hinge of the lower linkage assembly. This deformation pattern suggests that the structure experiences a combination of bending and rotational motion under load, with displacement propagating upward from the point of load application.

The eigenvalue buckling analysis further indicated that the structure was not susceptible to buckling under the applied loads, as the predicted critical buckling load exceeded the maximum applied load in the simulation. This result suggests that material yielding, rather than instability, would govern failure in the idealized model.  

During experimental testing, the physical prototype demonstrated the ability to support progressively increasing loads without immediate failure, confirming a degree of structural robustness. However, as the applied load approached higher magnitudes, localized weaknesses began to emerge. Unlike the simulation results, failure consistently occurred at the pin connections rather than at the hinge bodies or axle interface.  

The failure mode was characterized by deformation and eventual separation at the pinned joints, accompanied by the detachment of the adhesive used to secure the pins. The maximum load sustained by the physical model prior to failure was lower than the theoretical prediction obtained from ANSYS, indicating a discrepancy between the modeled and real world behavior. Despite this difference, the general deformation trends observed experimentally were qualitatively consistent with the simulation results.  

---

### 4.3 Interpretation

The differences observed between the theoretical predictions and experimental results highlight several important limitations and assumptions within the modeling and assembly processes.   

One primary source of discrepancy is the simplified representation of joints in the ANSYS model. In the simulation, idealized joint conditions were used to replicate pin connections, which do not fully capture the stress concentrations, contact interactions, and material imperfections present in physical pins. As a result, the simulation underestimated the chance of failure at these locations and instead predicted failure in the adjacent hinges.  

Additionally, the method used to secure the pins in the physical prototype introduced unintended weaknesses. The use of hot glue created non-uniform load transfer and stress concentrations at the pin interfaces. These factors significantly reduced the load-carrying capacity of the joints and contributed to premature failure during testing.   

Another important consideration is the difference between the idealized material properties used in the simulation and those of the actual 3D-printed components. 3D printing can include internal defects and reduced material strength compared to the homogeneous material assumptions used in ANSYS. These factors further contribute to the reduced experimental load capacity.   

It is also important to note that the applied loads in both the simulation and experimental testing were not intended to replicate the actual loads experienced by an F-14 Tomcat. Instead, the loads were scaled to suit the dimensions and materials of the prototype model. As such, the purpose of this analysis was not to directly simulate real-world operational conditions, but rather to evaluate the relative structural behavior, identify critical failure points, and validate general design assumptions.   

## 5. Comparison with Analytical and Simulation Predictions

### 5.1 Summary of Phase 2 Predictions

5.1 Summary of Phase 2 Predictions  

Reviewing the Phase 2 predictions, the calculations were originally based on a landing gear designed for an RC aircraft rather than a full-sized one, primarily due to time constraints and a lack of available variables required to conduct a proper stress analysis on the actual project. As a result, the loads used in Phase 2 were significantly smaller than what would be experienced in a real-world application. With the overall size and weight of the aircraft being scaled down, external forces such as the normal force were derived from a much lighter aircraft weight, producing results that were minimal and of limited practical use. To obtain more accurate and meaningful results for Phase 3, a stress analysis was conducted on a full-sized aircraft landing gear, yielding a von Mises stress of approximately 1377 psi and a factor of safety of approximately 6.82. Additionally, a buckling analysis was performed during Phase 3, which had been absent from the Phase 2 analysis entirely and contributed valuable insight to the overall structural evaluation.  

---

### 5.2 Experimental vs. Predicted Performance

The whole idea for this project stemmed from a YouTube short the group stumbled across showing a landing gear model with two degrees of freedom and some precise dynamic movement. That video was the main inspiration, and the goal from the start was to build something similar. Looking at the final result, the model moves dynamically in a way that closely matches what was seen in that original video, so in terms of dynamic performance, the project came out exactly as planned. As for comparing the simulation results from Ansys to the actual prototype, it's complex as the simulation was run on a full-sized landing gear using aircraft-grade metals and rubber, while the physical model was printed entirely out of PLA. So a direct one-to-one comparison of the numbers doesn't hold up. That said, the prototype still demonstrated a working suspension system through the spring mechanism and proved that the overall design concept translates well even at a smaller scale.  

---

### 5.3 Sources of Discrepancy

The primary source of discrepancy between the Phase 2 and Phase 3 predictions stems from the significant difference in scale and scope of the stress analysis. The Phase 2 calculations were based on an RC aircraft landing gear rather than a full-sized aircraft, resulting in substantially lower load values and a less representative factor of safety. As the project scaled and more accurate variables became available, the Phase 3 analysis produced a von Mises stress of approximately 1377 psi and a factor of safety of 6.82, highlighting how drastically the initial predictions underestimated real-world loading conditions though the model still was able to meet industry standards. Even though the original RC model displayed way smaller stresses, the scaling was quite accurate in comparison to the real world model.  

Another discrepancy lies in the material difference between the simulation model and the physical prototype. The Ansys simulation was conducted using full-sized aircraft-grade metals and rubber components, whereas the fabricated prototype was printed entirely in PLA. Since PLA has significantly different mechanical properties, including lower stiffness, yield strength, and density, a direct numerical comparison between the simulated stress results and the prototype's actual performance is not valid. This material mismatch means the simulation serves more as a proof-of-concept for structural behavior at scale rather than a direct predictor of the prototype's performance.

## 6. Failure Analysis and Lessons Learned

### 6.1 Observed Failures and Defects

The first prototype did not fail structurally, but it failed functionally, which in some ways was just as big of a problem. The main issue was that several parts simply did not fit together the way they were supposed to, especially around the moving joints. The joint holes were too tight, which made it nearly impossible to connect the parts while still allowing them to rotate freely. Since the whole point of the landing gear mechanism is smooth movement between links, this basically stopped the prototype from working the way it was designed to.   

The size of the first print made things worse. Everything was too small, which made alignment harder and made the parts more sensitive to even small printing errors. Trying to assemble something that small with tight tolerances by hand was frustrating and showed us quickly that what looks fine in CAD does not always translate the same way in real life. We also realized too late that we needed more than one prototype iteration, because the first version revealed problems that were not visible in the digital model at all. The team ended up solving the joint issue by using hot glue and toothpicks to hold the connections together while still giving the mechanism enough freedom to move. It was not the most elegant engineering solution, but it worked well enough for a prototype and allowed us to actually demonstrate the landing gear motion.   

---

### 6.2 Root Cause Analysis

The root cause of most of the early problems came down to the gap between what the CAD model showed and what the 3D printer actually produced. In the model, everything fit perfectly because the dimensions were exact. In reality, 3D-printed parts do not come out with perfect accuracy. Small holes tend to print slightly undersized, and mating parts can come out slightly oversized, which created interference at the joints and made assembly difficult from the start.   

The original design also did not account enough for the kind of clearance a moving mechanism actually needs. For a part that just sits in place, tight fits are fine. But for rotating joints, you need extra room to reduce friction and allow smooth motion. Without that clearance, the links could not rotate freely and the whole mechanism felt stiff and restricted during the first assembly attempt.   

The small scale of the first print made all of this worse. When you scale parts down, small dimensional errors become much more significant. A tolerance mistake that might be manageable at full size can completely lock up a joint at a smaller scale. That is ultimately why we had to resize and reprint, because the problems were not going to go away without changing the approach. 

---

### 6.3 Design and Fabrication Mistakes

The first clear mistake was not accounting for 3D printing tolerances when designing the joints. The holes were drawn too tight in the model, so when the parts came out of the printer, there was not enough clearance for the mechanism to move or even fully assemble. Going forward, the joint holes should be designed slightly larger, and pins should be given more clearance from the start to allow free rotation without forcing parts together.   

The second mistake was starting the 3D printing too late. Because the first prototype had so many fitment issues, we needed extra time to redesign, reprint, and test again. If printing had started earlier, there would have been more time to work through multiple versions and actually improve the design before the deadline instead of just fixing what we could at the end.   

Printing the first prototype too small was another mistake that cost us time. The small size made the joints harder to handle, more sensitive to printing errors, and harder to fix without reprinting everything. Once we scaled it up, the assembly became noticeably easier and the mechanism was much more manageable.   

The last fabrication mistake was assuming the printed geometry alone would be enough to create smooth joint motion. We learned that moving joints need a connection method that holds the parts together without locking them in place. The toothpick and hot glue fix worked for the prototype, but the real lesson is that proper pins, bolts, washers, or spacers should have been designed into the system from the beginning.  

---

### 6.4 Unexpected Outcomes and Insights

One of the most surprising things was how well the prototype worked after just a few small adjustments. The first assembly was discouraging because nothing moved the way it was supposed to. But after switching to the toothpick and hot glue joint method and making a few other fixes, the mechanism started to actually function and demonstrate the landing gear motion. It was a reminder that prototyping is not about getting it perfect the first time, it is about figuring out what is wrong and fixing it.   

The bigger insight for me was realizing how much a CAD model can hide. Looking at the digital assembly, everything seemed like it should work. The parts fit, the joints moved, the geometry looked right. But the physical prototype showed that friction, print tolerance, hole size, and alignment all interact in ways that are really hard to predict from a screen. Mechanical design is not just about having the right shape on paper. It is about making sure that shape can actually be built, put together, and used.   

The most important lesson from this whole process was that functional prototypes almost always need more than one iteration. The first print was not a failure, it was information. It told us exactly where the design fell short and what needed to change. After resizing, reprinting, and rethinking the joint connections, the final prototype performed significantly better. That experience reinforced something that I think applies beyond this project, which is that the willingness to go back, fix the problem, and try again is what separates a design that works from one that just looks good. 

---

## 7. Design Improvements for Future Iterations

<img width="776" height="510" alt="Screenshot 2026-05-01 at 13 00 03" src="https://github.com/user-attachments/assets/a580e103-edd5-46e0-8d1c-d9babab6ff60" />
<img width="776" height="510" alt="Screenshot 2026-05-01 at 12 59 51" src="https://github.com/user-attachments/assets/6bb531a7-9322-4118-a6c9-4d11e13bcdae" />
<img width="973" height="641" alt="Screenshot 2026-05-01 at 12 59 35" src="https://github.com/user-attachments/assets/d9156896-7ede-4222-82f4-30be9d1c1778" />
<img width="1018" height="552" alt="Screenshot 2026-05-01 at 12 59 21" src="https://github.com/user-attachments/assets/b3d44fa1-da31-47aa-8c50-7d2cb67e8650" />
<img width="989" height="552" alt="Screenshot 2026-05-01 at 12 59 00" src="https://github.com/user-attachments/assets/20213e69-f8dc-4796-9568-f169346f2ef0" />


### 7.1 Structural and Geometric Modifications

One of the main areas for improvement lies in the geometry of the main landing gear strut. The current design is strong enough for carrier operations, it exhibits areas of stress concentration at the main strut. The engineering analysis identified the critical stress region as the interface between the lower hinge with the main strut, where the load transfer concentrations are most severe under the computed normal force 56,700 lbs and drag force 26,649 lbs. Although the current factor of safety of 6.8254 confirms the design is structurally sound, the geometry at this junction could be refined to redistribute peak stresses more evenly. Introducing larger fillet radii and tapered cross-section transition at the lower strut connection would smooth the load path and reduce the risk of fatigue cracking under repeated high cycle arrested landing loads.  

The maximum deformation recorded in the analysis was 1.3835 inches, occurring under full carrier landing loads. While this falls within acceptable limits, reducing deformation at the critical region would improve the alignment precision of the wheel assembly relative to the trunnion axis during extension and retraction cycles. Thickening the web section of the main strut in the identified critical zone while keeping added mass minimal  would increase local stiffness and bring peak deformation closer to the 1.0 inch range without significantly impacting the total gear mass of 5,101 lbs.  

Additionally, the mesh size used in the finite element analysis was 3 inches, which is appropriate for a global stress overview but may not fully capture localized stress gradients at the lower link connection and hinge joint. A future structural iteration should employ a refined mesh in the critical region to improve result accuracy, and the geometry should be adjusted accordingly if higher fidelity analysis reveals stress concentrations not captured in the current model.  

---

### 7.2 Material and Manufacturing Improvements

The structural analysis was conducted using titanium alloy as the assigned material in the simulation environment. However, the physical prototype was fabricated using filament, which does not replicate the mechanical properties of titanium alloy. As a result, the physical model served primarily as a geometric and kinematic validation tool, and all quantitative conclusions, including the maximum stress of 1,254.3 psi and maximum deformation of 1.3835 inches, are derived solely from the simulation results.  

In future iterations, creating the prototype with materials that better match the simulation inputs would enhance the correlation between the analytical and experimental results. While machining with full titanium can be cost-prohibitive at the academic level, more feasible options printing using sintered metal processes could provide a more structurally representative physical model for validation.  

---

### 7.3 Assembly and Reliability Enhancements

The landing gear assembly consists of eight primary components: the wheel, wheel axle, rotating strut, fixed strut, suspension hinge links, suspension hinge, folding hinge, and fixed support  all connected through revolute joints and fixed constraints to achieve a single degree-of-freedom retraction motion. While this configuration successfully replicates the intended kinematic behavior, future iterations should focus on refining the pin connections and hole clearances at each hinge interface. Tighter tolerance control at these revolute joints would reduce unwanted play in the mechanism and improve the precision and repeatability of the retraction and deployment cycle.  

The folding hinge and suspension hinge components, which govern the inward collapsing motion of the linkage during retraction, represent the most kinematically sensitive elements of the assembly. Any misalignment at these interfaces during assembly can propagate into binding or uneven load distribution across the linkage system. Future designs should incorporate self-aligning spherical bearings at these critical pin joints to compensate for minor angular deviations introduced during fabrication or assembly, improving reliability without requiring high-precision manual adjustment.  

The fixed support, which anchors the entire system and represents the mounting interface to the aircraft structure, should also be revisited for improved load distribution. Since all reaction forces from the normal force of 56,700 lbs and drag force of 26,649 lbs are ultimately transferred through this component, future iterations should include a more distributed attachment footprint and gusset reinforcements to reduce stress concentration at the base mounting points. This would improve the structural reliability of the assembly under the dynamic loading conditions characteristic of carrier based operations.

## 8. Conclusion

This project successfully demonstrated the design, fabrication, and evaluation of an F-14–inspired landing gear system through a structured, multi-phase engineering approach. Beginning with conceptual design in Phase 1, progressing through detailed CAD modeling and analysis in Phase 2, and culminating in physical prototyping and testing in Phase 3, the project provided a comprehensive understanding of both theoretical and practical aspects of mechanical system design.

The analytical and simulation results established a strong baseline for structural performance, indicating that the design met expected strength and stability requirements under scaled loading conditions. However, the transition from simulation to physical implementation revealed important discrepancies, particularly in joint behavior, material performance, and manufacturing limitations. These differences highlighted the impact of real-world factors such as tolerances, friction, and assembly constraints, which are often simplified or idealized in computational models.

Despite these challenges, the final prototype was able to achieve the intended kinematic functionality, successfully demonstrating extension, load support, and retraction behavior. The iterative process of redesign, reprinting, and reassembly played a critical role in refining the system and improving overall performance. This process reinforced the importance of prototyping as a tool for identifying design flaws and validating assumptions beyond what can be observed in digital models.

Overall, the project emphasized the importance of integrating engineering analysis with practical fabrication considerations. It also demonstrated that successful mechanical design requires not only accurate calculations and simulations, but also adaptability, iteration, and attention to manufacturability and assembly. The insights gained from this work provide a strong foundation for future improvements and highlight key areas where design refinement and material selection can further enhance system performance and reliability.
