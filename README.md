## Introduction ##

This repository contains code that implements a coupling map based calibration of 
measurement errors on quantum devices.

## Requirements ##

Minimum version requirements provided. Some more recent version of these 
libraries may have deprecated necessary functions (qiskit is likely the primary
 culprit).

 - Python             : 3.9.7
   - numpy            : 1.12.3
   - matplotlib       : 3.4.2
   - seaborn          : 0.11.1
   - qutip            : 4.6.3
   - scipy            : 1.7.1
   - qiskit           : 0.18.1
 - Jupyter
   - IPython          : 7.29.0
   - ipykernel        : 6.4.1
   - ipywidgets       : 7.6.5
   - jupyter_client   : 7.0.6
   - jupyter_core     : 4.9.1
   - jupyter_server   : 1.11.1
   - jupyterlab       : 3.2.1
   - nbclient         : 0.5.3
   - nbconvert        : 6.1.0
   - nbformat         : 5.1.3
   - notebook         : 6.4.6
   - qtconsole        : 5.1.1
   - traitlets        : 5.1.1

## Running ##

The notebooks in this repository may be invoked using the `jupyter notebook` 
command.

IBMQ Credentials are required for experiments that access those devices.


## Notebooks ##
All notebooks are standalone, some are demonstrative and further data may be
collected by changing the `backend` variable within the notebook. As device
backends are fickle the default backend may not be avaliable and may need 
changing.

 - Simulated Error Channels and Hinton Diagrams
   - Constructs simulated measurement error channels and provides code for the purposes of visualisation 
 - Simulated BV Range Experiments
   - Implements a range of measurement error mitigation techniques
   - Executes these techniques against simulated measurement errors constructed as per the `Simulated Error Channels and Hinton Diagrams` notebook.
   - Compares the performance of each of these techniques over a range of measurement shots.
 - BV and QFT Experiments
   - Implements a range of measurement error mitigation techniques
   - Constructs BV and QFT experiments (via circuits from the IBMQ documentation)
   - Compares the performance of each of these techniques over a range of circuits on a target device






