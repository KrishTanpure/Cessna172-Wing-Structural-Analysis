# Cessna172-Wing-Structural-Analysis



This project is a finite element analysis of a Cessna 172 full-wing under limit load conditions defined by FAR Part 23. The wing is modeled as a solid aluminum body and analyzed under a 3.8g positive limit load case to evaluate structural integrity, deformation behavior, and safety margins.



***NOTE: The FEA is performed on a simplified solid body geometry. The rib-spar CAD model is included to demonstrate structural layout understanding but was not used in the FEA due to meshing complexity.***







#### **Methodology**



###### **-Boundary Conditions**

* **Fixed support applied at the wing root surface simulates fuselage attachment**
* **Wingtip is left with no constraint**



###### **-Applied Loads**

* **Resultant lift force of 20694 N in +Y direction (upward), distributed across the wing body. This represents aerodynamic lift at 3.8g limit load.**
* **Standard earth gravity of 9.81 m/s^2 in -Y direction accounts for self weight of the structure.**





##### **Material Used**  

* **Aluminum alloy 2024-T3**

&#x20;   



##### **Results**



|**Result**|***Value***|
|-|-|
|Max Tip Deformation|41.97 mm|
|Peak Von Mises Stress|19.22 MPa|
|Max Principal Stress (Tensile)|19.93 MPa|
|Min Principal Stress (Compressive)|-18.3 MPa|
|Minimum Safety Factor|14.57|





###### **Why the safety factor is so high?**



\-The safety factor is so high because the body was solid. A real Cessna 172 wing is a hollow structure of thin aluminum skin over ribs and spars. The solid model has orders of magnitude more material cross-section than the actual wing, so stresses are artificially low. This analysis is valid for demonstrating load path behavior and deformation trends, but does not reflect real structural efficiency of the wing.

