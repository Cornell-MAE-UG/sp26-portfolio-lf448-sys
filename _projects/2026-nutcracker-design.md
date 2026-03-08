---
layout: project
title: Nut Cracker Design
description: OLHW 5
images: assets/nutcracker-design.png
--- 

![Nutcracker design](/assets/nutcracker-design.png)

## Find
The goal of this assignment is to design a nutcracker that can crack a macadamia nut using a lever. To do so, it's necessary to find the lever dimensions so that the necessary amount of force to crack the nut can be generated.

## Given
- Avg macadamia nut diameter: 20 mm
- Grip strength: 300 N
- Force needed: 22.18 kg

## Approach
Assumptions:
- The nutcracker is a lever
- There is no friction
- The nut is set perfectly in the nutcracker

### Calculations / Thought Process

1. Moment balance about the pivot
 Sum Mp = 0
      Fout(0.02) - Fgrip(x) = 0
      2180(0.02) = 300x
      x = 0.144m
2. Mechanical advantage
   MA = Fout / Fin
MA = 2180 / 300 = 7.27
→ The lever must provide **7.27× mechanical advantage**

## Diagram
Refer to image above for design.

## Usability
Though this design is mechanically feasible, the usability is questionable:

1. The lever arm must be unrealistically long to generate enough force  
2. The nut must be placed very close to the pivot  
3. If the user’s grip strength is too small, they will not generate enough force
