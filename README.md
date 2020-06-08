# qsim: A Quantum Optimal Control Package

## Introduction
In current quantum computer prototypes information is stored an processed in 
quantum bits or qubits which are controlled by electric pulses. In order to 
find the optimal control pulse for a given operation, this package simulates 
the system under control and applies optimization algorithms to the pulses. 
These include gradient based algorithms generalizing the GRAPE algorithm [1].

The package sets a focus on realistic noise models to enable noise mitigation
through pulse tailoring. Imperfections of the control electronics can also be
included in the simulations.

The implementation was inspired by the optimal control package of 
[QuTiP](http://qutip.org/).

## Installation
To avoid difficulties, QuTiP needs to be installed first. To do so, follow 
[their instructions](http://qutip.org/docs/latest/installation.html) and 
install all recommended dependencies. Then install the 
[filter_functions package](https://github.com/qutech/filter_functions) and two
remaining dependencies by:

    conda install pandas simanneal
    pip install filter_functions

Then download the source code and use
`python setup.py develop` to install using symlinks or 
`python setup.py install` without.

## Documentation
The documentation features an API documentation and an introduction in the 
form of jupyter notebooks demonstrating how to utilize the package.

## References
[1]: Khaneja, N., Reiss, T., Kehlet, C., Schulte-Herbrüggen, T., Glaser, S.
(2004). Optimal control of coupled spin dynamics: design of NMR pulse sequences
gy gradient ascent algorithms 
[https://doi.org/10.1016/j.jmr.2004.11.004](https://doi.org/10.1016/j.jmr.2004.11.004)