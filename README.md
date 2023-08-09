# Reservoir_Pressure_Simulator
The code defines a class called PressureSolver. 

The __init__ method of the PressureSolver class takes the following arguments:

N: The number of grid points in the logarithmic coordinate system.
dt: The time step size.
t_final: The final time for the simulation.
well_data: A path to a file containing well pressure data.
rw: The radius of the well.
re: The outer radius of the reservoir.
h: The height of the reservoir.
phi: The porosity of the reservoir.
mu: The viscosity of the fluid in the reservoir.
ct: The compressibility of the reservoir rock and fluid.
Q: The flow rate at the well.
pi: The initial pressure in the reservoir.
The solve function: It solves for the pressure distribution in the reservoir. This method uses a finite difference method to solve the differential equation for
pressure.

The analytical_linesolution: This calculates the analytical solution for the pressure distribution in the reservoir. This solution is based on the assumption that
the well is fully penetrating.

The well_pressure method: calculates the well pressure. This method takes the pressure at the first grid point as an input, and subtracts half of the wellbore
radius from it.

The solve_time_analytical_and_numerical: solves for the pressure distribution in the reservoir and calculates the well pressure 
both numerically and analytically. This method plots the well pressure data from the well test data file, as well as the numerical and analytical solutions.

The pw_numerical_optimal: calculates the well pressure numerically for a given set of time points and reservoir properties. 
This method uses an optimized time step size to improve the accuracy of the solution.
