# Design and Analysis of F-14 Landing Gear System

MEE 342: Principles of Mechanical Design  
Touchdown Mechanics  

Aditya Sally, Anuj Shastry, Emily Lopez, Joshua Raya, Kevin Ruiz Lopez, Sanad Dababneh  
Yi Ren  
April 27, 2026  

---

# Table of Contents

1. Introduction  
2. Fabrication Process and Parameters  
 2.1 Material Selection and Filament Properties  
 2.2 3D Printer Specifications  
 2.3 Print Settings and Build Parameters  
 2.4 Iterations and Reprints  
 Slicing Tolerances and Printer Accuracy  
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

---

# 1. Introduction

Aircraft landing gear systems represent one of the most critical interfaces between an aircraft and its operating environment. During takeoff, landing, and ground operations, the landing gear must support the full weight of the aircraft, absorb significant impact energy, and maintain stability under varying and often unpredictable conditions. These demands make landing gear design a multidisciplinary challenge involving structural mechanics, kinematics, materials, and reliability. This complexity is even more pronounced in military aircraft, where higher loads, aggressive operating conditions, and strict space constraints push the design further.

The Phase 1 portion of this project focused on developing the conceptual design of an F-14–inspired landing gear mechanism. This included defining the overall system layout, identifying key subsystems, and understanding the kinematic behavior required for extension, retraction, and load support. The preliminary design established how the main strut, wheel assembly, and linkage members interact, while also considering fundamental design constraints and potential failure modes.

In Phase 2, the project transitioned from concept to a detailed and realistic representation. A complete 3D CAD assembly was developed to capture the geometry of individual components, their connections, and the motion of the mechanism. Greater emphasis was placed on practical design considerations such as part dimensions, tolerances, and manufacturability using 3D printing. Engineering analyses were also introduced to evaluate stresses, fatigue behavior, and overall structural performance, providing a basis for validating the design.

Phase 3 builds upon this foundation by moving from digital design to physical realization and testing. The finalized components were fabricated using additive manufacturing, assembled into a working prototype, and evaluated under experimental conditions. This phase focuses on understanding how the real system behaves compared to predictions, highlighting discrepancies between simulation and physical performance. Observations from fabrication, assembly challenges, and testing outcomes provide critical insight into design limitations, unexpected behaviors, and areas for improvement.

---

# 2. Fabrication Process and Parameters

## 2.1 Material Selection and Filament Properties

The ASU print lab supports multiple filament types including PLA, PETG, TPU, and Nylon-based materials. For this project, PLA was selected due to its ease of printing, dimensional stability, and compatibility with standard lab settings.

PLA provides:

- Good stiffness for structural representation  
- Low warping, improving dimensional accuracy  
- Ease of support removal for complex geometries  

However, it is noted that PLA has relatively low impact resistance and temperature tolerance compared to engineering-grade materials such as Nylon or PETG. Given the objective of prototyping rather than full structural validation, PLA was considered sufficient.

---

## 2.2 3D Printer Specifications

The ASU print lab utilizes printers compatible with 1.75 mm filament and supports a variety of materials including PLA, PETG, TPU, and Nylon variants. The maximum build volume is approximately:

- 250 mm x 210 mm x 210 mm  

The printers support:

- Breakaway Support Structures  
- Standard fused deposition modeling (FDM) processes  
- Moderate resolution suitable for functional prototypes  

---

## 2.3 Print Settings and Build Parameters

Print parameters were selected based on ASU lab defaults and adjusted for structural relevance to landing gear geometry.

Typical settings include but are not limited to:

- Infill: 10–20%  
- Layer height: ~0.2 mm (standard resolution)  
- Supports: Breakaway supports enabled  
- Filament diameter: 1.75 mm  

Some engineering considerations that would be included with these parameters in mind would be:

- Infill (10–20%)  
Chosen to reduce material usage and print time while maintaining basic internal structure. However, this limits load-bearing capability and makes the part more suitable for geometric validation rather than full mechanical testing.

- Part Orientation  
Critical to reduce layer-based weakness. The landing gear components were oriented to minimize stress across layer interfaces, improving resistance to bending and shear.

- Supports  
Required due to overhangs and complex geometry in the landing gear assembly. Breakaway supports allow easier post-processing but may affect surface finish.

- Wall Thickness  
Outer walls contribute more to strength than infill, so geometry was designed to rely more on shell thickness where possible.

---

## 2.4 Iterations and Reprints

Multiple iterations were required to address dimensional accuracy and fitment issues inherent to FDM 3D printing processes. Initial prints revealed discrepancies between nominal CAD dimensions and the as-printed geometry, particularly in mating features such as hole and shaft interfaces.

### Slicing Tolerances and Printer Accuracy

FDM printers such as Bambu Lab and Ender series machines exhibit dimensional deviations due to nozzle size, extrusion behavior, and thermal effects. While the nominal filament diameter is 1.75 mm, variations in extrusion and cooling lead to predictable inaccuracies:

- Hole undersizing (internal features print smaller than designed)  
- External feature oversizing (shafts print slightly larger)  

Typical dimensional tolerances for these printers are approximately:

- ±0.004 in to ±0.012 in  

Slicing software also introduces geometric approximation errors, especially in curved or small features, further affecting dimensional accuracy.

---

# 3. Assembly Procedure and Integration

## 3.1 Step-by-Step Assembly Process

The assembly process began with securing the base stand, which served as the primary support structure for the entire landing gear system. Establishing a stable reference frame at the start ensured proper alignment during subsequent steps.

The main strut was first positioned and fixed onto the stand. Once secured, the wheel axle was attached to the strut, forming the central load-bearing connection. The wheel was then mounted onto the axle, completing the primary rolling interface.

Following this, the attachment fitting for the suspension hinge was installed onto the strut assembly. The suspension hinges were then connected, allowing for vertical compliance and load absorption. Finally, the folding hinges were installed, enabling the mechanism to retract and fold inward, simulating the motion required for stowing the landing gear within an aircraft body.

All components were connected using quarter-inch screws. While effective for prototyping, future iterations would benefit from the use of bolts and precision pins to improve stability, reduce friction, and allow smoother rotational motion.

---

## 3.2 Fitment and Alignment Considerations

Initial assembly revealed significant fitment issues, primarily due to tight tolerances and high friction between mating components. Many parts required forceful insertion, indicating that the clearances were insufficient for a functional mechanism.

To address this, the components were redesigned with adjusted tolerances. Additionally, the overall model was scaled up by approximately 1.5 times the original dimensions to improve manufacturability and ease of assembly. This scaling also enhanced visibility and handling during testing.

Alignment was another major challenge in the initial build. The components did not align properly, resulting in restricted motion and instability. A redesigned version of the assembly improved alignment, and the addition of a dedicated stand further stabilized the system.

The motion of the mechanism was initially inconsistent and “janky,” largely due to friction and misalignment. After redesigning tolerances and simplifying the structure, the motion improved, although it was still not perfectly smooth.

---

## 3.3 Challenges Encountered During Assembly

The initial assembly attempt was largely unsuccessful, as most components did not function as intended. Tight tolerances prevented proper fitting, and the mechanism could not move freely.

Although no major structural failures occurred, excessive friction between parts led to noticeable wear during repeated assembly attempts. Additionally, variability in print quality introduced inconsistencies in part dimensions.

A significant design challenge involved the intended use of a universal joint. Due to limitations in modeling and implementation within the available timeframe, this design could not be successfully realized.

---

## 3.4 Solutions and Workarounds Implemented

To overcome fitment issues, manual post-processing was performed. Parts were sanded and epoxy was used where necessary.

The most significant workaround involved redesigning the strut mechanism into two interfacing components, allowing rotation within the assembly.

Multiple redesigns and reprints were carried out, and assembly was repeated approximately three times.

---

# 4. Experimental Testing and Evaluation

## 4.1 Procedure

The Testing and Evaluation procedure began with an Ansys simulation. Components were scaled and loads applied to match expected conditions.

- Static structural analysis performed  
- Eigenvalue buckling analysis performed  

After simulation, the prototype was assembled and tested physically with increasing loads until failure conditions were observed.

---

## 4.2 Results

The Ansys simulation showed that the critical points of the system would be at the connection between the two bottom hinges.

---

## 4.3 Interpretation

---

# 5. Comparison with Analytical and Simulation Predictions

## 5.1 Summary of Phase 2 Predictions  
## 5.2 Experimental vs. Predicted Performance  
## 5.3 Sources of Discrepancy  

---

# 6. Failure Analysis and Lessons Learned

## 6.1 Observed Failures and Defects

The first prototype did not fail structurally, but it failed functionally. The main issue was improper fit at joints, preventing rotation.

---

## 6.2 Root Cause Analysis

The root cause was the mismatch between CAD precision and real-world 3D printing tolerances.

---

## 6.3 Design and Fabrication Mistakes

- Did not account for tolerances  
- Printed too small  
- Started printing late  
- Did not include proper joint hardware  

---

## 6.4 Unexpected Outcomes and Insights

The biggest takeaway was that iteration is essential. The first prototype provided critical insight that led to improvements.

---

# 7. Design Improvements for Future Iterations

## 7.1 Structural and Geometric Modifications  
## 7.2 Material and Manufacturing Improvements  
## 7.3 Assembly and Reliability Enhancements  
