---

# **Heat Conduction Simulation Using Finite Difference Method**

This project implements a numerical solution for steady-state heat conduction in a two-dimensional plate. The simulation utilizes the **Finite Difference Method (FDM)** to calculate temperature distributions across the plate, considering boundary conditions and material properties.

## **Features**
- **Customizable Grid Resolution**: The simulation allows for fine control over grid density in both x and y directions to achieve the desired accuracy.
- **Boundary Conditions**:
  - Fixed temperature boundaries.
  - Convective heat transfer at specified surfaces.
- **Material Properties**: Supports varying thermal conductivities for different regions of the plate.
- **Central and Edge Node Calculations**: Incorporates specific equations for handling central nodes, boundary nodes, and corner nodes.
- **Error Tolerance**: Iterative computation continues until the error falls below a specified threshold.

## **Key Variables**
- Plate dimensions, thickness, and thermal properties (`L`, `t`, `k`).
- Boundary conditions such as ambient temperature (`T_inf`) and convective heat transfer coefficient (`h`).
- Grid resolution in the x and y directions (`N_x` and `N_y`).
- Temperature updates using iterative methods.

## **How It Works**
1. The plate is divided into a grid using the defined resolution.
2. Temperature at each grid point is calculated iteratively based on neighboring nodes, thermal properties, and boundary conditions.
3. The process continues until convergence is achieved within the defined error tolerance.

## **Applications**
- Heat transfer simulations in engineering systems.
- Studying thermal behavior in materials.
- Optimization of cooling and heating designs.

## **Dependencies**
- **Python 3.x**
- **NumPy**: Used for matrix and array operations.

## **Getting Started**
Clone the repository and run the script using Python:

```bash
git clone https://github.com/Navid2266/Heat_Transfer-II-.git
cd Heat_Transfer-II-
python heat_conduction_simulation.py
```

Modify the variables in the script to adapt the simulation to your specific case.

---
