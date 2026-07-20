# Building Machine Learning Classifiers for Convective Triggering Using ERA5 and TOOCAN

## Project Overview
The existing convection trigger functions that are used in deep convection parametrizations in GCMs have deficiencies that significantly impact simulation results. Common issues include convection overprediction, which results in model simulations raining too frequently, as well as the misrepresentation of the diurnal cycle of precipitation. (Zhang et al., 2021)

This project aims to build off of the existing research on machine learning-based convection triggers. We use satellite-observed data from the TOOCAN GPM dataset along with global climate and weather data from ERA5 to train various machine learning classifiers. The goal is to compare the performance of these ML classifiers to that of existing trigger functions. We also use Explainable AI to explore the environmental variables that the models consider to be the most important for convection initiation.


### Outline
- Begin by exploring the TOOCAN GPM and ERA5 datasets.
  -> `dataset_exploration.ipynb`
  -> `toocan_era5_exploration.ipynb`
- Train simple Random Forest and Logistic Regression models on the data to predict convection onset from large-scale environmental variables.
  -> `model_training.ipynb`
- Train XGBoost and neural network models.
- Evaluate offline against TOOCAN labels 
