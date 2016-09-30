---
layout: default
title: Home
is_main: true
---

# Introduction

Aversive++ is a library that eases developpement of robotic applications for microcontrollers.
Its aim is to provide an interface simple enough to be able to create complex applications, 
and optimized enough to enable small microcontrollers to execute these applications.

# Why using Aversive++ ?

You like C++ ? You like robot programming ? You may like Aversive++ !

The library provides several features : 
 - Easy control system design (use PID, Quadramp, Average, and a lot of other filters).
 - An Inverse Kniematic able to run on very small microcontroller !
 - Some specific drivers for robots actuators and sensors.
 - Containers similar to STL, but with no heap allocation need.

# Why Aversive++ is different ?

Let's be clear, every framework for embedded systems has it's own difference. 
But here is a comparison of Aversive++ with other framework of the embedded world :

 - Aversive++ provides a build system (like a lots of similar frameworks), but try to be independent from it. 
Indeed, for example, a part of the library can be exported to Arduino.
