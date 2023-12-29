# Low-temperature Electrolysis for Hydrogen Generation in Multi-timescale Steady-state Simulation 
 This repository hosts the scripts to execute the multi-timescale steady-state simulation for low-temperature electrolysis (LTE) process to produce hydrogen from a nuclear-renewable hybrid energy system (N-R HES).

## How to use
Users can reconfigure any given N-R HES with minor modifications in the provided scripts and get insightful results by following the instructions below:
* "FESTIV_Secondary_Trial.m" is the main script to run. It can be run via MATLAB GUI or command line on a machine which has FESTIV already installed along with the sotware mentioned below.
* To have the new optimization models containing LTE-related constraints, replace the original .gms file in FESTIV repository.
* Since, the set-up of FESTIV automatically retains the model formulated in the 'FESTIV_MODEL-master\MODEL_RULES\GAMS_Model_Files', please make sure to comment out some initial scripts in the FESTIV.m file and load the multi-timescale simulation parameter through loading a MATLAB workspace variable. You can follow the process used in the provided 'FESTIV_Secondary_Trial.m' file.
### Dataset
The NREL-118 bus test network data was taken and modified to accommodate the proposed LTE process in an IES setting. 

### Environment & Necessary Software
The framework has been built on the existing FESTIV framework. Users are recommended to install FESTIV as per the FESTIV user manual installation instructions. As of now the the scripts have been executed on CentOS only.

### Software
```
MATLAB              R2020b
GAMS                32.2
CPLEX               12.8
```


## Publications
**If you use these scripts in your research, please cite our publications**:

Rahman, J., Jacob, R.A., and Zhang, J., “Multi-timescale Power System Operations
for Electrolytic Hydrogen Generation in Integrated Nuclear-Renewable Energy Systems (Under
Review)”, TechRxiv, 2023.


**Collaborations are always welcome if more help is needed.**
## License
MIT License, Copyright (c) 2022 Jubeyer Rahman & Jie Zhang

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.


## Contact

Jubeyer Rahman
jxr180022@utdallas.edu

Jie Zhang
jiezhang@utdallas.edu 

