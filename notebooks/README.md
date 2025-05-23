# **Project 3: notebooks**

This folder contains notebooks and resources for **Project 3**, where we reconstruct surface ocean pCO₂ from sparse observations using Earth System Model (ESM) outputs and machine learning techniques.

- **`data_story_gr3.ipynb`**  
  Main notebook for running ML training and evaluation on pre-selected ESMs and members using preprocessed inputs. Recommended for most users seeking an efficient workflow.



- **Contribution Statement**
  - Sungjoon Park:
    - Led the evaluation of ensemble model performance in the ENSO region, with a focus on seasonal variation in surface pCO₂ reconstruction.
    - Through spatial diagnostics of RMSE, bias, and correlation across ensemble members and seasons, identified systematic over- and under-estimations tied to upwelling dynamics and ENSO-driven variability.
    - Highlighted the role of seasonal biases—especially during DJF and JJA—in shaping regional reconstruction accuracy.
    - Additionally, finalized the compilation of the full data story document, synthesizing findings into a cohesive narrative.
 
  - Catherine Lyu:
    - Conducted an evaluation of seasonal bias structures across ESMs, using gridded histograms and statistical summaries (mean, standard deviation, skewness) to characterize how reconstruction errors vary by model and season.
    - Performed a regional analysis of the Benguela Upwelling System (BUS) and quantified the mean reconstruction bias across ensemble members and highlighting model-specific tendencies toward cold bias.
 
  - Raphie:
    - Evaluated potential causes for the unusually high RMSE in the West coast of South America.
    - Partially explored outliers in biases across testbed models to evaluate individual testbed model performance and improve the accuracy of overall testbed.
    - Intitiated brainstorming of initial project ideas.
 
  - Kefeng Shi:
    - Compose the 7.1 biotic part of the notebook, made an adjustment in the XGBoost model to include a "Blended Model" to adjust a weight on Chl-a variable and adjust reconstruction process.
    - In the scenario of changed input, mapping the bias distribution by ESMs, and tried to do a time series analysis to see if the blended feature mimic the model truth.
    - Provide some climate science info and logic based on my own background.
