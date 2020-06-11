# Particle Classifier
particle classifier project done for PDAML course I took at the University of Edinburgh.

## 1) Geant Simulation
Using Geant4 on c++ to simulate an experiment. The experiment simulated is firing electrons and protons with energies 200MeV to 25.15 GeV in steps of 50MeV. The particles are fired at a detector of several layers of concrete, lead and liquid argon, all layers being able to measure the energy deposited by the scattered particles. For each particle the energies deposited in each layer are collected and saved in a .csv file.

## 2) Reconstruct Data
Using the pandas and scikit-learn libraries the data is calibrated to the true energy of the particle and a train test split used to generate the training and testing data.

## 3) Data Validation
In order to 


![equation](http://latex.codecogs.com/gif.latex?%5Cfrac%7BTotalTemplate%7D%7BTotalVolume%7D)  


.csv files created using a geant 4 simmulation of a detector with multiple solids
used ML to distinguish protons from electrons fired at the detector in the simulation
census_utils.py and dt_utils.py provided by professors
jupyter notebook format with annotations describing each step
