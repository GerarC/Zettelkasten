---
reference: "[[University Physics - Sears and Zemansky's]]"
date: 26/08/2023
type: 1 #evergreen
alias: TDP06, Kinetic-Molecular Model
tags: thermo_physics, physics
code: TDP06
---
# TDP06 Kinetic-Molecular Model

The **Kinetic-Molecular Model** born due to the necessity to know, since a microscopical view, why [[TDP01C Pressure|Pressure]], [[TDP01E Volume#TDP01E Volume|Volume]] and [[TDP01A Temperature|Temperature]] behave as by the [[TDP05 Equation of Ideal Gas State|Equation of Ideal Gas State]]. Basically, it's understand macroscopic event since its smallest pieces, it means, *Atoms*. ^1

Using [[MPU04 Force|Force]], [[MPU08 Momentum|Momentum]] and [[MPU02B Velocity]] We can find relations between Macro and Micro points. From momentum we have that the $\Delta p_x = 2mv_x$, the particle lasts to displace side to side $\Delta t = \large\frac{2L}{v_x}$ and it's known that $F_x = \large\frac{\Delta p_x}{\Delta t}$ so $F = \large\frac{mv_x}{L}$. Approximating the velocity of $y$ and $z$ axes to $x$, using [[MPU01A Vector Components|Vector Components]] the medium velocity $\vec{V}_{med}^2 = 3v_x^2$ so $F=\frac{\vec{V}_{med}^2}{3L}$, [[TDP01C Pressure|Pressure]] depends on the Force and the Area thus $P = F/A = \large\frac{m\vec{V}_{med}^2}{3L^3}$. All this only for a particle. ^2

For $N$ Particles, the pressure made is $P = \large\frac{Nm\vec{V}_{med}^2}{3L^3}$. Remembering about [[MPU06A Kinetic Energy#MPU06A Kinetic Energy|Kinetic Energy]] and doing some tricks, the Equation we obtain is $PL^3 = \frac{2}{3}NE_k$, how $L^3$ is a [[TDP01E Volume|Volume]] and using [[TDP05 Equation of Ideal Gas State|Equation of Ideal Gas State]], $NkT = = \frac{2}{3}E_K$ Finally we obtain that $E_k = \frac{3}{2}kT$ what's a relation between [[TDP01A Temperature#TDP01A Temperature|Temperature]] and Kinetic Energy of the particles. ^3

# Links
<<[[TDP05 Equation of Ideal Gas State|TDP05]]|[[TDP06A Heat Capacities]]>>

**Related notes:**
- [[TDP03 Heat|Heat]]
- [[TDP01D Total Energy|Total Energy]]
- [[TDP03D Specific Heat|Specific Heat]]