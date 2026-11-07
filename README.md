# EPW-Zhou_lab
EPW internal version of Zhou lab
Updated and Maintained By a50844

Current Features
1. Hall Concentration Calculation
2. Accumulate Electron Thermal Conductivity and Conductivity v.s. Mean free path
3. Thermal_excited_carrier

Details
1. Hall Concentration Calculation
This feature contains module hall_rta_states.f90 & hall_crta_validation, and interface eval() function at use_wannier3.f90
hall_rta_states calculate first order response of Lorenz Force C under relaxation time approximation(RTA).
And the hall resistivity can be calculated by C/(sigma_xx*sigma_yy).

2. Accumulate ETC and COD
This feature is at bte_transpt.f90, aim to get accumulate ETC and COD v.s. mean free path.

3. Thermal_excited_carrier
This feature calculate thermal excited electron/hole concentration by assuming Fermi-Dirac Distribution.
Has function metal_char_dens. This feature use Sum{edos*f*dE}
N/V also.
