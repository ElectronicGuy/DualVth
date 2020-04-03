# DualVth
![](https://img.shields.io/badge/Development-Stopped-red)

This project consist in a plug-in for Synopsis's PrimeTime: the script, written in TCL, implements a post-synthesis leakage power minimization procedure.
The leakage power consumption reduction is obtained by employing two techniques:
- DualVth cell assignment: swapping non-time-critical cells with higher voltage threshold ones
- Transistor resizing: selected cells maybe resized to further lower power consumption or improve slack. 

The savings obtained from swapping LVT cells with HVT cells is obtained as follows

 savings = (start_power - end_power) / start_power

Allowed input values may range from 0 (no leakage minimization) to 1 (maximum leakage savings). Every cell have to keep the same cell footprint during the optimization.

Circuits such as https://s2.smu.edu/~dhoungninou/Benchmarks/ISCAS85/VERILOG/c1908.v and https://s2.smu.edu/~dhoungninou/Benchmarks/ISCAS85/VERILOG/c5315.v were used as benchmarks.


## Award winning
The project was part of the "Synthesis and Optimization of Digital Systems" course at Politecnico di Torino. The script scored the best result in 2018/2019 academic year.
 
## Tools

For this project the following tools were used
- Prime time - Synopsys

## Report

For further informations refer to the report.pdf.
