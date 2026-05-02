---
layout: project
title: Nut Cracker Design
description: OLHW 5
images: "{{ 'assets/images/updated-nutcracker' | relative_url }}" 
--- 

![Nutcracker design]({{ 'assets/images/updated-nutcracker' | relative_url }})

## Find
The goal of this assignment is to modify the original nutcracker design by treating the handles as flexible beams, rather than rigid members. Now, the handles bend under the force from the nut and the linear actuator, so we msut find where the maximum beam deflection occurs and pcik a design that will limit the deflection to less than two percent of the handle length. 

## Given
- Avg macadamia nut diameter: 20 mm
- Nut location: 20 mm from pivot
- Actuator location: 50 mm from pivot
- Handle Length: 50 mm
- Actuator Force: 222.4 N
- Force needed: 217.6 N
- Allowable deflection: 1 mm

## Approach
Assumptions:
- The nhandle is effectively a cantilever beam fixed at the pivot
- The nut froce, and actuator force act transverse to the beam
- The actuator pushes down at the end of the handle and the nut pushes upwards
- Beam material behaves elastically
- There is no friction
- The nut is set perfectly in the nutcracker

### Calculations / Thought Process

1. Location of Max Deflection: Since we're treating the handle as a cantilever beam, the largest deflection occurs at the free end, so the maximum deflection is at the end of the handle where the actuator is attached
2. Beam Design
   Deflection = PL^3 / 3EI - Fa^2(#L-a) / 6EI
   P = 222.4 N
   F = 556 N
   L = 0.050 m
   a = 0.020 m
   E = 69 x 10^9 (aluminum)
   I = bh^3 / 12
3. Moment of Intertia
   b = 2 mm
   h = 8 mm
   I = (0.002)(0.008)^3 / 12
     = 8.53 x 10 ^-11 m^4
4. Put it all together --> Deflection = 0.755 mm, which is less than 1 mm

## Diagram
Refer to image above for design.

## Usability
This updated design is more feasible than the original because the actuator provides the input force, not the user. The use of an aluminum, lightweight beam keeps the deflection below the required limit, and is efficient as it increases the moement of inertia without adding material. 
