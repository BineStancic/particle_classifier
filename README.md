# Particle Classifier
particle classifier project done for PDAML course I took at the University of Edinburgh.

## 1) Geant Simulation
Using Geant4 on c++ to simulate an experiment. The experiment simulated is firing electrons and protons with energies 200MeV to 25.15 GeV in steps of 50MeV. The particles are fired at a detector of several layers of concrete, lead and liquid argon, all layers being able to measure the energy deposited by the scattered particles. For each particle the energies deposited in each layer are collected and saved in a .csv file.

## 2) Reconstruct Data
Using the pandas and scikit-learn libraries the data is calibrated to the true energy of the particle and a train test split used to generate the training and testing data.

## 3) Data Validation
In order to check the quality of the data histograms of $(calibrated energy - true energy)/true energy$ were plotted at each energy. This was used to form a 2d plot of the histogram spredas against energies for both electrons and protons. These plots were used to determine the standard deviation of the histograms hence the "quality" of the callibrated energy for each particle at each energy. This gives insight on the "qualit" of the detector to detect a range of scattered energies.

## 4) Machine Learning
Using a multi-layer preception clasifier to build a supervised NN to distinguish between the protons and electrons.
