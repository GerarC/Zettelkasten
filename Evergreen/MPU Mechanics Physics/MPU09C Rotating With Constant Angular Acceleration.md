---
reference: "[[SZPs09A Rotation With Constant Angular Acceleration]]"
date: 11/05/2023
type: 1 #evergreen
alias: MPU09C, Rotating With Constant Angular Acceleration, MCUA
tags: mechanics_physics, physics
code: MPU09C
---
# MPU09C Rotating With Constant Angular Acceleration

A body **Rotating With Constant Angular Acceleration** is when the body follows a circular trajectory and its [[MPU09B Angular Acceleration|Angular Acceleration]] doesn't vary. This type of movement is so similar to the [[MPU02D Motion With Constant Acceleration|Motion With Constant Acceleration]], but it's also possible to calculate it's tangential values and the normal acceleration. ^1

|**Function**|**Equation**|
|:----------:|:----------:|
|Distance|$\theta = \theta_0 + \omega_{0z}t + \frac{1}{2}\alpha_zt^2$|
|Velocity|$\omega_z = \omega_{0z} + a_zt$|
|Acceleration|$\alpha_z = \frac{\omega_{2z} - \omega_{1z}}{t_2 - t_2}$|
|Time|$t = \frac{\omega_z - \omega_{0z}}{\alpha_z}$|
|Equation without Acceleration|$\Delta \theta = \frac{1}{2}(\omega_{0z} + \omega_z)t$ ^2|
|Equation without Time|$\omega_z^2 = \omega_{0z}^2 + 2\alpha_z(\Delta\theta)$| ^2


# Links
<<[[MPU09B Angular Acceleration|MPU09B]]|[[MPU09D Moment of Inertia|MPU09D]]>>

**Related notes:**
- [[]] 