# **Project 3: Machine Learning Reconstruction of Surface Ocean pCO₂**

Team 3

**Please find the contribution statement in notebooks/README.md**

Our study:
1. Performs member-based analysis on **XGBoost-based pCO2-Residual reconstruction** across 3 ESM model testbeds - ACCESS, CanESM, MPI-ESM
2. Evaluates reconstruction performance using a Large Ensemble Testbed, with **RMSE, bias and correlation metrics** and suggests improvements to our pCO2-residual reconstruction ability.
3. Performs deeper analysis on the spatial and seasonal structure of model bias
4. Finds the largest sources of errors in distinct geographic errors and attempts to explain the dynamical impact of the upwelling in coastal regions: __abiotic__
5. Evaluates Chlorophyll as an important factor in the residual pCO2 story: __biotic__


This project reproduces and extends portions of the analysis presented by Gloege et al. (2020) and Heimdal et al. (2024), using machine learning to reconstruct surface ocean partial pressure of CO₂ (pCO₂) and evaluate reconstruction performance under sparse observational coverage.

The notebook implements a **pCO₂-Residual** approach with an **XGBoost** model to improve upon standard pCO₂ reconstructions by isolating and removing the temperature-driven signal prior to machine learning regression. It also evaluates performance using data from the **Large Ensemble Testbed (LET)**.


## **Folder Structure**

To reduce complexity in the main notebook, several helper functions and figures are modularized into the `lib/` directory. You may modify these as needed for your project.

```bash
Project3/
├── lib/                       # Helper scripts
│   ├── __init__.py
│   ├── bias_figure2.py        # Code for bias calculation and visualization
│   ├── corr_figure3.py        # Code for correlation calculation and visualization
│   ├── residual_utils.py      # Prepares data for ML, tools for dataset splitting, model evaluation, and saving files.
│   └── visualization.py       # Custom plotting class SpatialMap2 for creating high-quality spatial visualizations with colorbars and map features using Cartopy and Matplotlib.
├── notebooks/
│   └── Project3_Starter.ipynb # Main notebook containing full analysis & data story
|   ├── leappersistent_file_management.ipynb # check the size of files and clean up
|   ├── Project3_Data.ipynb  # Used for preprocessing data, if more than the 20 preprocessed ESM members are required. 
```

 ## **Objective**

This project aims to:
1. Implement an **XGBoost-based pCO₂-Residual reconstruction**.
2. Evaluate reconstruction accuracy using **bias and correlation metrics**.
3. Compare reconstructions against gridded output from the **Large Ensemble Testbed (LET)**.



## **References**

- **Gloege et al. (2020)**  
  *Quantifying Errors in Observationally Based Estimates of Ocean Carbon Sink Variability.*  
  [DOI: 10.1029/2020GB006788](https://doi.org/10.1029/2020GB006788)

- **Bennington et al. (2022)**
  *Explicit Physical Knowledge in Machine Learning for Ocean Carbon Flux Reconstruction: The pCO2-Residual Method*
   [DOI: 10.1029/2021ms002960](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2021MS002960)

- **Heimdal et al. (2024)**  
  *Assessing improvements in global ocean pCO₂ machine learning reconstructions with Southern Ocean autonomous sampling.*  
  [DOI: 10.5194/bg-21-2159-2024](https://doi.org/10.5194/bg-21-2159-2024)


## **Contributions and Collaboration**

We encourage collaborative version control using GitHub. If working in a team, please follow contribution guidelines (e.g., commit messages, branches).

You may find [this GitHub tutorial](https://github.com/leap-stc/LEAPCourse-Climate-Pred-Challenges/blob/main/Tutorials/Github-Tutorial.md) helpful for getting started.

-->
