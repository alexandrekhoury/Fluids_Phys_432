# Fluids_Phys_432

README

Alexandre Khoury

Version : Python 3.7


1.hydro.py

1-Dimension hydro solver
following the motion of a sound wave in a uniform density gas
using an initial gaussian perturbation in the density

I have also used reflective boundary conditions.

#Questions:
What happens as you increase the amplitude of the perturbation? 
Do you see a shock? 
If so, what do you think is setting the width of the shock? 

#Answers:
Having a larger width makes the wave seperation happen faster. (the initial gaussian density seperates in two blobs) 
Having a higher amplitude causes there to be a shock observed faster.
The waves reflect of the boundaries and steepen once they collide with each other (shock).
(when the waves collide, the numerical error is higher since it is steeper. )
This creates an artificial viscosity term that increases (reason behind the shock width), this viscosity term is generated by numerical errors and computational limits.
It is important to note that at small amplitudes this effect is not visible (except after huge amount of time).

My code simulates a gaussian amplitude of 0.2, which shows the transitions between no shock and shock as time increases.


Yes, I see a shock when the waves reflect of the boundaries and hit each other. 
The width of the shock is being set 

List of collaborators: 
-Mathieu Bruneault
-Ronan Legin
-Manuel Bolduc


2.advection.py

Applying FTCS and Lax-Friedrich method on a linearly increasing fluid quantity with fixed boundaries.

speed was set to -0.1
and time step was chosen to be smaller than dx/u (for stability condition)

List of collaborators:
-Mathieu Bruneault
-Ronan Legin
