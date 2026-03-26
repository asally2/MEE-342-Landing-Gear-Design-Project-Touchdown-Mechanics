Design and Analysis of F-14 Landing Gear System
MEE 342: Principles of Mechanical Design
Touchdown Mechanics
Aditya Sally, Anuj Shastry, Emily Lopez, Joshua Raya, Kevin Ruiz Lopez, Sanad Dababneh
Yi Ren
March 25, 2026
Table of Contents
1. Introduction	3
2. Final Design Overview	4
3. CAD Assembly and Modelling	5
3.1 Overall Assembly	5
3.2 Component-Level Design	9
3.3 Exploded View	10
3.4 Motion Study	11
4. Design for Additive Manufacturing	13
4.1 Part Consolidation	13
4.2 Geometry Optimization	13
4.3 Support & Overhanging Features	13
4.4 Material and Tolerance Considerations	14
5. Engineering Analysis	15
5.1 Loading Assumptions	15
5.2 Static Stress Analysis	16
5.3 Fatigue Analysis	17
5.4 Simulation Results	18
6. Iterations and Improvements	23
7. Risks and Limitations	24
8. Conclusion	25
9. Future Work	26

1. Introduction
Aircraft landing gear systems represent one of the most critical interfaces between an aircraft and its operating environment. During takeoff, landing, and ground operations, the landing gear must support the full weight of the aircraft, absorb impact energy, and maintain stability under varying and often unpredictable conditions. These demands make landing gear design a multidisciplinary problem involving structural mechanics, kinematics, materials, and reliability, especially in military aircraft, where higher loads and stricter space constraints further complicate the design.

Figure 1: An F-14A Tomcat aircraft gains altitude after takeoff, its landing gear still down.
The Phase 1 portion of this project focused on developing the conceptual design of an F-14–inspired landing gear mechanism. This included defining the overall system layout, identifying key subsystems, and understanding the kinematic behavior required for extension, retraction, and load support. The preliminary design captured how the main strut, wheel assembly, and linkage members interact, while also considering basic design constraints and possible failure modes.
In Phase 2, the project moves from a conceptual design to a more detailed and realistic model. The main focus is on building a complete 3D CAD assembly that represents the actual geometry of components, how they connect, and how the mechanism moves. At this stage, more attention is given to practical considerations such as part dimensions, clearances, and how the design can be manufactured using 3D printing.
This report presents the final CAD model of the landing gear system and explains how the assembly was developed to match the intended motion and structure of the mechanism. It also sets up the engineering analysis used to evaluate stresses, fatigue behavior, and overall performance, which helps justify the final design choices.
2. Final Design Overview
The final design consists of a complete 3D CAD assembly of an F-14–inspired landing gear system, developed to capture both the structural and kinematic behavior of a retractable mechanism. The assembly includes key components such as the wheel, wheel axle, rotating strut, fixed strut, suspension hinge links, folding hinge elements, and a fixed support structure. Each of these parts was modeled individually and then combined into a fully constrained assembly to replicate the intended motion and load transfer within the system.

Figure 2: Preliminary Sketch from Phase 1
The design maintains the primary functional objectives defined in Phase 1, which include supporting loads in the deployed configuration and enabling controlled motion during retraction. The rotating strut acts as the central load-bearing member, while the linkage system, composed of suspension hinges and folding hinge components, guides the motion of the assembly. The wheel and axle subsystem allows for rotational motion during operation.
Compared to the preliminary concept, the final design introduces more defined geometry, including realistic part thicknesses, pin connections, and interface features. Components that were previously represented schematically have been converted into manufacturable parts with proper dimensions and clearances.
3. CAD Assembly and Modelling
3.1 Overall Assembly
The landing gear system was modeled as a multi-component assembly consisting of eight primary parts: the wheel, suspension hinge link, wheel axle, rotating strut, fixed strut, fixed support, suspension hinge, and folding hinge. Each part was created as an individual solid model and then assembled using appropriate mates to represent real mechanical connections.
Revolute joints were implemented at key connection points, particularly at hinge interfaces, to allow rotational motion between components. Fixed constraints were applied to the support structure to anchor the system, while the remaining components were allowed to move relative to one another based on the defined joint conditions. This setup enabled the assembly to replicate the single-degree-of-freedom motion established in the conceptual design. All the following dimensions are in inches.

Figure 3: Main Strut

Figure 4: Rotating Strut

Figure 5: Wheel

Figure 6: Wheel Axle

Figure 7: Suspension Hinge Link

Figure 8: Folding Hinge

Figure 9: Suspension Hinge

3.2 Component-Level Design
Each component in the assembly was designed with a specific mechanical function, contributing either to load support or controlled motion of the system. Additionally, each part was designed with consistent hole sizes and clearances to ensure proper fit between mating parts.
The wheel was modeled with a defined outer diameter and width to represent realistic ground contact. Its geometry allows it to rotate freely about the axle while maintaining alignment with the strut assembly.
The wheel axle serves as the connection between the wheel and the suspension system. It was designed as a cylindrical shaft with an appropriate diameter to support the wheel while fitting within the mating components. The axle also provides a mounting point for the rotating strut.
The rotating strut acts as the primary structural member of the system. It supports the vertical load transferred from the wheel and serves as the main axis about which parts of the mechanism rotate. Features such as pin holes and connection points were added to allow integration with hinge components.
The fixed strut provides additional structural support and helps guide the motion of the system. It works in conjunction with the rotating strut to maintain alignment and stability during both deployed and retracted configurations.
The suspension hinge links and suspension hinge components form part of the linkage system that controls motion. These parts include pin connections and fork-like geometries to allow rotational movement while maintaining structural connectivity between components.
The folding hinge components enable the compact motion of the system during retraction. Their geometry allows the linkage system to collapse in a controlled manner, mimicking the inward folding behavior seen in aircraft landing gear.
The fixed support serves as the base of the assembly and represents the mounting interface to the aircraft structure. It remains fully constrained and provides a reference for the motion of the rest of the system.
3.3 Exploded View
An exploded view of the assembly was created to clearly show the spatial relationship between all components and to illustrate the assembly sequence. The view separates the wheel, axle, strut components, and linkage elements along their axes, making it easier to understand how each part connects within the system.
This assembly strategy ensures that components can be manufactured individually and then assembled in a logical sequence. It also allows for easier troubleshooting and replacement of parts if needed, which is important for a prototype system where multiple iterations may be required.



3.4 Motion Study
A motion study was used to simulate the behavior of the landing gear mechanism and verify that the assembly achieves the intended kinematic motion. The system operates with a single degree of freedom, where rotation at the hinge joints drives the movement of the entire assembly.
The main strut incorporates a suspension feature that represents the shock absorption behavior during landing. This allows the system to account for vertical load transfer and energy absorption when the wheel makes contact with the ground. While simplified in the CAD model, this feature reflects the role of suspension systems in reducing impact forces and protecting the structural components.
During retraction, the rotating strut enables the wheel assembly to change orientation so that it can tuck inward and become more horizontal. This motion is guided by the linkage system, which ensures that the wheel follows a controlled path without interfering with other components. The folding hinge and suspension links work together to coordinate this movement, allowing the mechanism to transition smoothly between deployed and retracted configurations.
Additionally, the pivot at the fixed support acts as the primary reference point for the system and allows the entire mechanism to rotate inward during retraction. This rotation is essential for achieving a compact stowed configuration, similar to real aircraft landing gear systems where space constraints require efficient folding mechanisms.
Although a formal animation was not generated, the motion was verified directly within the CAD environment using assembly mates and manual manipulation of the mechanism. This approach allowed the full range of motion to be observed and validated, ensuring that the system operates as intended without interference between components.
4. Design for Additive Manufacturing
4.1 Part Consolidation
For all the parts that make up the Landing Gear System, most components would be printed as their own part, and no subassemblies could be printed as one piece for the purpose of functionality, consideration of design for assembly, inhibition of calculations as one part instead of multiple parts, and for aesthetics. Therefore, processing will involve fitting as many parts as possible on the printing plate, so that there are two or three distinct cycle times based on the parts on the bed, printing speed, and other printer configurations. Printing one part at a time will cause delays and redundant operations if revisions need to be made.
4.2 Geometry Optimization
S. Nos. 2, 6, 7, and 8 have symmetrical, linear features that cause no abrupt changes or overhangs,, generating print-friendly parts that would result in little to no support or error during the additive manufacturing process. However, for the wheel, the printing process will optimize the flat side surface as the base of the print, meaning the outward arch from the base, will require supports. These supports will have no effect on functionality but will add to the cycle time.
In addition, S. No 3, 4, and 5 will most likely have the longest cycle times due to the length of their geometry and the different features included, such as cylinders, fillets, overhangs, and a variety of geometry changes. Printing these parts together will result in the longest cycle time and will determine the appropriate takt time for completing all prints.
4.3 Support & Overhanging Features
As mentioned earlier in Geometry Optimization, S. No 3–5 will have the most overhanging features, and S. No 1 will be oriented to keep the base of the wheel flat while also supporting the tread features. This configuration should not cause any major issues during printing.
4.4 Material and Tolerance Considerations
For the showcase of the system, PLA or PETG will be used based on availability and quantity. It is intended that all parts will be printed using the same material to maintain consistency and achieve an appropriate aesthetic. There is no specific requirement for material properties to enhance functionality, as materials such as carbon fiber or TPU would provide improved flexibility or durability, but these properties are not necessary for the scope of this assignment.
Therefore, tolerance considerations will focus on the cylindricity of through or blind holes in S. No 1–5 and No 7, particularly during assembly. Attention will also be given to hole sizing where shafts or extruded features are inserted to ensure proper fit and alignment.


5. Engineering Analysis
5.1 Loading Assumptions
	Due to the complexity of the landing gear assembly, the loading analysis was focused on the main strut, as forces acting on other components were determined to be negligible in comparison. A free body diagram (Figure 1) was constructed to identify and represent all loads acting on the system during the critical landing condition.
The system was analyzed under the assumption that the landing gear is attached to a medium-sized RC aircraft with an estimated gross landing weight of 5.92 lb. This estimate was derived from the measured assembly volume of 6.56 in³, which corresponds to a total gear weight of approximately 0.296 lb for FDM-printed PLA (ρ = 0.0451 lb/in³). Since landing gear mass typically represents approximately 5% of total aircraft weight, the gross aircraft weight was back-calculated accordingly.
Under this loading scenario, the critical forces acting on the system during touchdown were identified as follows: the normal ground reaction force and drag force at the wheel axle, the support reactions at the upper strut attachment point, and the axial force in the drag brace linkage. The brace force was deemed negligible relative to the magnitude of the other forces and was excluded from the primary stress calculations.
The two main gear struts were assumed to collectively carry 90% of the total aircraft weight, with the remaining 10% supported by the nose gear. The load sustained by a single main strut under static conditions is therefore:
Wstrut = (0.90 × 5.92) / 2 = 2.664 lb
During touchdown, a dynamic load factor of n = 3.0 was applied in accordance with standard RC aircraft landing gear design practice, amplifying the effective load on the strut. The resulting normal force is:
N = 3.0 × 2.664 = 7.992 lb
The spin-up drag force was estimated using the MIL-A-8863 standard, which specifies drag as 47% of the normal force:
D = 0.47 × 7.992 = 3.756 lb
Applying static equilibrium to the free body diagram, the support reactions at the upper attachment point were determined. The vertical reaction force was found to equal the normal force (Ay = 7.992 lb), and the horizontal reaction force was found to equal the drag force (Ax = 3.756 lb), consistent with the assumption that the brace force contribution is negligible.
Figure 1: Free Body Diagram
5.2 Static Stress Analysis
The main strut was identified as the critical component of the landing gear assembly, as it is subjected to the most significant combined loading during landing. Specifically, the strut experiences simultaneous bending and torsional stresses resulting from the ground reaction force and the lateral offset of the wheel axle relative to the strut centerline.
Using fundamental mechanics of materials, the bending stress was computed as  =McI  where M is the maximum bending moment occurring at the drag force application point i.e the bottom of the main strut, as shown in the ANSYS results as well, c is the outer radius of the strut cross-section, and I is the second moment of area of the hollow circular cross-section. This yielded a bending stress of 1173.75  psi.
The torsional shear stress was similarly determined using  = TCJ, where T is the applied torque due to axle eccentricity, and J is the polar moment of inertia. This produced a torsional shear stress of 416 psi.
To assess the combined stress state, the Von Mises failure criterion was applied:
VM = b2+ 32 = 1,377.49 psi
Comparing this equivalent stress against the yield strength of PLA (S_y = 5,800 psi), the factor of safety against yielding is:
FS = SyVM = 4.216
A factor of safety of 3.05 indicates that the main strut has adequate resistance to yielding under the expected landing loads, with sufficient margin to account for impact variability and material inconsistencies inherent to FDM-printed PLA components. These calculations also do not account for the shock-absorbing spring expected to absorb some of the weight attached to the inside during additive manufacturing meaning that the current geometry and materials are more than efficient enough for landing.
5.3 Fatigue Analysis
	The main strut was once again selected as the component of interest for the fatigue assessment, as it experiences repeated loading with each landing cycle. During operation, the strut undergoes a zero-based stress cycle, transitioning from a zero stress state while airborne to a peak stress state at the moment of touchdown. The maximum stress in the strut was previously established as the Von Mises equivalent stress of 1,377.49 psi, while the minimum stress is taken as 0 psi during flight. For a zero-based cycle, the mean and alternating stresses are equal by definition, each equal to half the maximum stress, giving values of 688.75 psi respectively.
Since PLA is a thermoplastic polymer, it does not exhibit a true endurance limit as observed in metals. The endurance limit was therefore estimated as 40% of the ultimate tensile strength, yielding an approximate value of Se = 0.40 × 7,250 = 2,900 psi. The Modified Goodman criterion was selected as the fatigue failure criterion, as it is the industry standard approach for combined mean and alternating stress states, offering a balance between accuracy and conservatism.
Using the formula:
altSe+ meanSUT = 1FSf

The factor of safety against fatigue is calculated to be about 3, which is less than the static factor of safety but expected and still safe for landing.
5.4 Simulation Results
Displacements


Displacement boundary conditions were applied to selected faces of the model using the global coordinate system to restrict motion in specific directions. The vertical (Y) and lateral (Z) displacements were constrained to zero on designated faces, while the remaining directions were left free to allow realistic deformation under load. This approach prevents rigid body motion while accurately representing the attachment of the landing gear to the aircraft structure. By selectively constraining degrees of freedom, the simulation ensures that load transfer and structural response closely mimic real-world boundary conditions.
Von Mises Stress

The Von Mises stress plot shows that the maximum stress occurs near the lower region of the main strut, which is expected due to the combined bending and torsional loading at the wheel connection. The peak stress value is significantly below the yield strength of PLA, confirming that the design is safe under the applied loading conditions.
Factor of Safety

The factor of safety distribution indicates that the minimum factor of safety occurs in the same critical region of the strut. The minimum value remains above 1, with most regions significantly higher, confirming that the structure maintains adequate safety margins.
Fatigue Factor of Safety

The fatigue safety factor plot shows that the design can withstand repeated loading cycles associated with landing. The minimum fatigue safety factor is above 2, indicating acceptable fatigue performance for the intended application. This does not match up with the hand calculations, due to the fatigued parts being fixed in the simulation.
Fatigue Life

The fatigue life results indicate that the structure can endure a large number of loading cycles before failure. This confirms that the landing gear is suitable for repeated use under the assumed loading conditions.
Normal Stress along the y-axis

The normal stress distribution in the vertical direction highlights tensile and compressive regions along the strut. The highest stresses are concentrated near the connection points, which aligns with the expected load path.
Total Deformation

The total deformation plot shows that the maximum displacement occurs at the wheel region, while the upper support remains fixed. The overall deformation is small, indicating sufficient stiffness of the design.




6. Iterations and Improvements
Improvements that can be made include developing specifications that tie features such as hole tolerancing to established industry standards, such as ASME, ANSI, or ISO dimensioning and tolerancing practices, in order to better account for manufacturability across different scales. In addition, more detailed information can be provided on the drawings to account for dimension tolerances as well as material or plating tolerances. This can be achieved by including notes on the drawings that reduce ambiguity, improve clarity of information, and ensure appropriate takt time during manufacturing.

A design iteration that would help reduce the need for redesign is scaling publicly available reference designs of other landing gear systems that include specifications, certificates of conformity, and testing documentation. These references could be used as a baseline for the design, allowing for a more defined starting point. This approach would make it easier to establish a calculative goal and adjust from that, rather than developing a scaled prototype from scratch and then attempting to justify the design and mechanical properties afterward.
7. Risks and Limitations
Several key factors influence the structural performance of landing gears and must be carefully considered throughout the design process. Finite Element Analysis (FEA) using ANSYS was used to evaluate and improve the reliability of the landing gear design.
One of the most significant risks in landing gear design is fatigue failure, which results from repeated cyclic loading during each landing cycle. Over time, this can lead to crack initiation and eventual structural failure. Structural integrity is equally important, as the landing gear must support the full weight of the aircraft on the ground while also absorbing impact forces generated during landing and takeoff. Shock absorption is another critical area, as the struts must effectively manage impact energy to prevent excessive load transfer to the rest of the structure.
The retraction mechanism also presents a potential risk, since any misalignment or mechanical failure during retraction could affect aerodynamic performance or prevent proper deployment before landing. Additionally, the wheels and tires must withstand high loads while providing sufficient friction for safe braking, meaning any weakness in this subsystem could lead to instability or failure.
While the design and analysis provide a solid foundation for understanding landing gear behavior, several limitations must be acknowledged. One primary limitation is that the FEA simulation did not incorporate the exact material properties of the filament used for 3D printing. As a result, the stress and deformation results may not fully represent the actual behavior of the physical prototype.
Furthermore, the reduced scale of the 3D printed model introduces additional limitations. Scaling effects can lead to dimensional inaccuracies that influence how the component performs under load. The wheel geometry is also a concern, as minor imbalances or surface imperfections from the printing process could result in uneven contact with the ground, affecting overall stability. Finally, the simulation assumed ideal static loading conditions, which do not fully capture the complex dynamic forces experienced during real landing events. While these limitations do not invalidate the results, they should be considered when interpreting the analysis outcomes.
8. Conclusion
This project demonstrates the design, analysis, and manufacturing preparation of a landing gear assembly through a structured engineering approach. The model was developed using CAD,, covering the overall assembly, component-level design, exploded views, and motion study, providing a comprehensive visual and mechanical representation of the system.
Engineering analysis played a central role in validating the design. Loading assumptions were established and used to perform static stress and fatigue analyses, along with supporting simulations. Key values such as bending stress, maximum bending moment, and torsional shear stress were calculated analytically and compared with software results, allowing for meaningful verification of the model. Boundary conditions were applied to prevent rigid body motion, and simulation outputs, including Von Mises stress, normal stress, total deformation, fatigue life, and factor of safety, were evaluated to assess structural integrity. Design iterations were carried out throughout the process, refining the assembly based on analysis results and identifying opportunities for improvement.
Finally, the risks and limitations of the project were acknowledged. Factors such as differences between simulated and printed material properties, scaling effects, and simplified loading conditions represent constraints of the current analysis. While these limitations do not invalidate the results, they define the scope within which the conclusions of this study should be interpreted.


9. Future Work
Future work for this project would focus on improving both the functionality and realism of the landing gear system through further development, testing, and validation. One of the primary areas of improvement is the creation of a detailed animation of the mechanism. While the motion of the system was verified within the CAD environment, generating a formal animation would provide a clearer representation of the retraction and deployment sequence. This would improve visualization, allow for better communication of the design intent, and help identify any subtle motion inconsistencies that may not be obvious through manual manipulation alone.
Another major area of future work involves the physical manufacturing and testing of the designed components. Printing all parts using additive manufacturing methods such as PLA or PETG would allow for the validation of assembly fit, clearances, and real-world motion behavior. Once printed, the prototype can be assembled and tested under basic loading conditions to observe structural performance, joint behavior, and any issues related to tolerance stacking or part deformation. This step would provide valuable insight into how closely the simulation and analytical results align with actual performance.
Design iterations would naturally follow from physical testing. Based on observed issues such as misalignment, excessive play in joints, or unexpected deformation, modifications can be made to improve the design. This may include adjusting hole tolerances, reinforcing high-stress regions, modifying geometry to reduce stress concentrations, or optimizing link lengths to improve motion. Iterative redesign would help refine the system and improve both reliability and performance over multiple cycles.
Further improvements could also include incorporating more accurate material properties into the analysis and expanding simulations to better represent dynamic loading conditions during landing. This would provide a more realistic assessment of fatigue life and structural response.
Overall, future work would focus on bridging the gap between simulation and physical validation, allowing the design to evolve from a functional prototype into a more refined and reliable mechanical system.
