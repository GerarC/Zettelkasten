---
reference: 
- "[[SZPs08D Collisions]]"
- "[[SZPs08F Elastic Collisions]]"
- "[[SZPs08E Completely Inelastic Collisions]]"
date: 11/05/2023
type: 1 #evergreen
alias: MPU08B, Collisions, Inelastic Collison, Elastic Collision
tags: mechanics_physics, physics
code: MPU08B
---
# MPU08B Collisions

A **Collision** is an interaction between two or more bodies. There are two types of collision: [[#MPU08B/1 Inelastic Collisions|Inelastic]] and [[#MPU08B/2 Elastic Collisions|Elastic]]. As the [[MPU04 Force|forces]] between the colliding bodies usually are larger than any external forces, so we can ignore the external ones, and can be applied the [[MPU08 Momentum|Conservation of momentum]]. ^1

# MPU08B/1 Inelastic Collisions

in this type of [[#MPU08B Collisions|collisions]] the acting bodies stick together after the collision. As they  have the same final velocity $\vec{v}_2$, the conservation of momentum just has three velocities instead of four, i.e., $m_A\vec{v}_{A1} + m_B\vec{v}_{B1} = (m_A + m_B)\vec{v}_{2}$. ^2

# MPU08B/2 Elastic Collisions

If the forces between the colliding bodies are [[MPU07B Conservative Force|Conservative]], so no mechanical energy is lost or gained, the [[#MPU08B Collisions|Collision]] is called a **Elastic Collision**. The general equations used to calculate this interactions are [[MPU06A Kinetic Energy|Energy]] conservation and [[MPU08 Momentum#MPU08/1 Conservation of Momentum|Conservation of momentum]]. But those equations are difficult, then in a lot of problems a body is initially at rest. ^3

**A body initially at rest**
The equations are:
	- $\frac{1}{2}m_A\vec{v}_{A1x}^2 = \frac{1}{2}m_A\vec{v}_{A2x}^2 + \frac{1}{2}m_B\vec{v}_{B2x}^2$
	- $m_A\vec{v}_{A1x} = m_A\vec{v}_{A2x} + m_B\vec{v}_{B2x}$
based on them we obtain that
	- $\frac{1}{2}m_A\vec{v}_{A1x}^2 = \frac{1}{2}m_A\vec{v}_{A2x}^2 + \frac{1}{2}m_B\vec{v}_{B2x}^2$
	- $m_A\vec{v}_{A1x} = m_A\vec{v}_{A2x} + m_B\vec{v}_{B2x}$ ^4

# Links
<<[[MPU08A Impulse|MPU08A]]|[[MPU08C Center of Mass|MPU08C]]>>

**Related notes:**
- [[MPU04 Force|Force]]
- [[MPU08 Momentum|Momentum]]