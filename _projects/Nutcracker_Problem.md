---
title: Nutcracker Problem
layout: project 
description: Analysis and Design of a Nutcracker
---

![Nutcracker Free Body Diagram](/assets/nutcracker-FBD.jpg)
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









