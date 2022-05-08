# CasaDi MPC to S-Function

This folder contains some examples on how to use CasaDi to generate an S-Function. The examples are specific for the Ball And Beam model.

- Run _mpc.ipynb_ to generate _f.c_ and _f.h_
- Edit f.c casadi_real_min definition from not defined to a low value (for ex 1e-8)
- Open MATLAB and run _mex s_function.c f.c_
```Matlab
mex s_function.c f.c
```
Note that IPOPT is not directly supported. To use IPOPT see: https://web.casadi.org/blog/mpc-simulink2/
