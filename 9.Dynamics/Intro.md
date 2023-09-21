# Dynamics

This chapter deals with the dynamics of robot manipulators. 
- Kinematic Equations: describe the motion of the robot `without` consideration of the forces and moments producing the motion
- Dynamic Equations: explicitly describe the relationship between `force` and `motion`. 

The equations of motion are important to consider in the design of robots, as well as in simulation and animation, and in the design of control algorithms.

&emsp;
## Euler-Lagrange Equation
We introduce the so-called Euler-Lagrange equations, which describe the evolution of a mechanical system subject to holonomic constraints (this term is defined later on).

To motivate the Euler-Lagrange approach we begin with a simple derivation of these equations from Newton’s Second Law for a one-degree-of-freedom system. We then derive the Euler-Lagrange equations from the Principle of Virtual Work in the general case.

In order to determine the Euler-Lagrange equations in a specific situation, one has to form the Lagrangian of the system, which is the difference between the kinetic energy and the potential energy; we show how to do this in several commonly encountered situations. 

We then derive the dynamic equations of several example robotic manipulators, including a two-link cartesian robot, a two-link planar robot, and a two-link robot with remotely driven joints.

The Euler-Lagrange equations have several very important properties that can be exploited to design and analyze feedback control algorithms. Among these are: 
- explicit bounds on the inertia matrix
- linearity in the inertia parameters
- the so-called skew symmetry and passivity properties. 

We discuss these properties in Section 9.5.

This chapter is concluded with a derivation of an alternate the formulation of the dynamical equations of a robot, known as the Newton-Euler formulation which is a recursive formulation of the dynamic equations that is often used for numerical calculation.