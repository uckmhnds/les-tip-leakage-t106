# Large eddy simulation of tip leakage flow in a linear turbine cascade

Abdurrahman G. Yavuz and Ayse G. Gungor
Department of Aeronautical and Astronautical Engineering, Istanbul Technical University

31st International Conference on Parallel Computational Fluid Dynamics (ParCFD 2019)

[Read the paper (PDF)](./parcfd2019-yavuz-gungor.pdf)

The conference link to this paper no longer works, so the PDF is hosted here.

## Summary

This study uses large eddy simulation (LES) to look at tip leakage flow over the T106 low-pressure turbine blade, and at how it interacts with secondary flows. The results show vortical structures near the tip casing wall. Tip leakage and secondary vortices interact and cause local adverse pressure gradients and separation on the suction surface. Horseshoe vortices form where the casing wall blocks the incoming flow.

## Case setup

- Solver: OpenFOAM, incompressible LES with the PISO algorithm and the Smagorinsky subgrid model
- Geometry: T106 blade with an unshrouded tip in an infinite linear cascade
- Mesh: fully structured hexahedral, 15 million cells
- Boundary conditions: cyclic in the pitch-wise direction, no-slip on the blade and tip end wall, symmetry at the hub end wall, uniform velocity at the inlet
- Reynolds number: 8x10^4, based on axial chord and inlet velocity

## Validation

- The time-averaged pressure coefficient at three cross-sections was compared with DNS and experimental data. It agrees on the pressure side and up to x/Cax < 0.6 on the suction side. Past x/Cax ≈ 0.8 it deviates, which is attributed to compressibility and inlet turbulence.
- The energy spectrum from a probe in the wake follows Kolmogorov's -5/3 law for about one decade.

## Citation

A. G. Yavuz and A. G. Gungor, "Large Eddy Simulation of Tip Leakage Flow in a Linear Turbine Cascade," 31st International Conference on Parallel Computational Fluid Dynamics (ParCFD 2019).
