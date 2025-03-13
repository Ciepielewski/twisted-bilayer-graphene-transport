![PythonVersion](https://img.shields.io/badge/python-3.8-succes)
[![License https://github.com/trainindata/feature-engineering-for-time-series-forecasting/blob/master/LICENSE](https://img.shields.io/badge/license-BSD-success.svg)](https://github.com/trainindata/feature-engineering-for-time-series-forecasting/blob/master/LICENSE)


# Quantum transport simulations of twisted bilayer graphene

## Research goals

In this project, we implement quantum transport simulations of a tight-binding model of twisted bilayer graphene. In particular, we are interested in studying the relation between the energy-resolved conductance and the density of states of twisted bilayer graphene near the first magic angle $\theta_m \approx 1.05^\circ$. 

Objectives and questions:
* Simulate a large mesoscopic device of twisted bilayer graphene attached to four electrodes
* Calculate the spectrum of near-magic angle twisted bilayer graphene
* Calculate the energy-resolved conductance of near-magic angle twisted bilayer graphene at a range of energies that includes the moiré spectrum
* Analyze signatures in the energy-resolved conductance and see if they relate to features in the moiré spectrum.

## Results:
* The results of this work were published in Physical Review Research: https://journals.aps.org/prresearch/abstract/10.1103/PhysRevResearch.4.043145
* The code and data used to produced the figures in our publication can be found in the following zenodo repository: https://zenodo.org/records/7356429
* We establish a correspondence between features in the wide-junction conductance and the presence of van Hove singularities in the density of states
* The conductance depends on the size of the device in a non-trivial way
* Near the magic angle, twisted bilayer graphene is an extremely sensitive material, specially in regards to the twist angle
* We propose that twisted bilayer graphene could be used in high-frequency device applications and as a sensitive detector
  

## Remarks
- The folder `./code` contains code and Jupyter notebooks to perform the quantum transport simulations. The functionality of each file is the following:
    - Notebook `./code/TBG_area_spectrum.ipynb` can calculate the spectrum of twisted bilayer graphene in a surface of the reciprocal lattice. It also has a function to calculate the electron density of states
    - Notebook `./code/TBG_linear_spectrum.ipynb` can calcualte the spectrum of twisted bilayer graphene in a line defined on the reciprocal lattice (typically a line that crosses high-symmetry points of the Brillouin Zone).
    - Notebook `./code/TBG_conductance.ipynb` can calculate the four-terminal conductance of a finite scattering region of twisted bilayer graphene
- The file `./code/requirements.txt` contains the essential packages required to run the code in the Jupyter notebooks
