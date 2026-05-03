---
title: Nutcracker Problem + Deflection
layout: project 
description: Analysis and Design of a Nutcracker
---

{{ '/assets/images/nutcracker-FBD.jpg' | relative_url }}

Find: Dimensions of Nutcracker, Size of Nut, Average Force to crack nut, Mechanical Advantage 

Input Parameters: 
- Radius of Nut = 0.5 in 
- Force of Nut = 222.18 kg 
- Average Force of grip = 90.5 1bf
- Dimensions: W = 6.1 in; L = 1.77 in; Handle length = 3 in 

Plan: 
1. FBD of Macadamia Nut
2. Find F_crack, F_max, and F_grip strength, 
3. FBD of Nutcracker and Nut
4. Solve for Reactions forces at nutcracker fulcrum
5. Solve for Mechanical Advantage 
6. Linear Actuator 

Calculations: 
1. F_nut = (222.18 kg)(9.8m/s^2)=2177N
2. F_grip = (90.5 1bf)(9.8m/s^2)=402.6N
3. R_y = Sum for Force = R_y + 201.3 - 1088.5 = 0 
    R_y = 887.2N
4. MA: F_out/F_in = 1088.5/201.3 = 5.4 
5. Desired MA: 10 2177/10 = F_in = 217.7 N = 49 lbf 
    Linear Actuator: PA-MC2, Stroke: 2.8 in, F: 9-56 lbf

Reactions: In order to have the most optimum MA, the PA-MC2 linear actuator best meets our calculated F_in. 


Deflection of a Nutcracker 

![Image 2](/assets/nutcracker-design-updated2.jpg)

Input Parameters: 
- F_nut = 244.7 lbf
- Location_nut = 2.6 in
- F_grip = 45.25lbf
- Location_grip = 4.6 in
- M_R
- Location_M = 6.1 in
- L = 6.1 in

Find: 
- Location of the largest y_max in the nutcracker handle
- I and cross-sectional area when v_max = 0.02L  

Plan: 
a. FBD of nut cracker 
b. Max deflection @ F_nut, F_grip, and M_R using equations from appendix E (1 and 3)
c. 0.02L = y_max 

Assumptions: 
1. The nutcracker is made of Aluminum (E = 3.77e10^6 psi)
2. Same forces as the original nutcracker problem
3. Each part of the nutcracker features a fixed-free end structure

Calculations: 
1. Deflection of F_nut: fixed-free structure with an applied force (Equation 1 of Appendix E)
    y_max = (244.7)((2.6^3)-(3)(6.1)(2.6^2))/6EI = -4328.4/EI
2. Deflection of F_grip: fixed-free structure with an applied force (Equation 1 of Appendix E)
    y_max = (-45.25)((4.6^3)-(3)(6.1)(2.6^2))/6EI = 198.9/EI
3. Deflection of M_r: fixed free design with an applied moment (Equation 3 of Appendix E)
    y_max = -((455.2)(6.1^2))/2EI = -8469/EI

Results: The location of the biggest deflection is at 6.1 in, the end of the nutcracker, due to M_r causing the largest deflection value. 

4. 0.002L = 0.122 in = y_max
   0.122 = (8469)/((3.77e6)(I)
   I = 54.31 in^4
   Cross-section: circular -> I = ((pi)(r^4))/4
   r = 2.88 in

Results: Equating 2% of the length of the nutcracker handle and our max deflection found in part a, the I value to satisfy this inequality is 54.31 in^4. I decided to use a circular cross-section with a radius of 2.88 in to satisfy the inequality (see image 2 for details). 
   









