# fashion-retail-price-optimisation
Demand Prediction and Price optimisation solution for online retail developed in S2DS Mar 2022

Developed by Elaine Thomas, Aminah Ali, Nathanaël Bullier, Sam Chien, Batyr Garlyyev

# Price optimisation model

This repo contains the implementation of a fashion retail price optimisation model created during S2DS .

# Directory structure: 

```
├── notebooks          <- Jupyter notebooks of various models.
│
├── src                <- Complete model pipeline for this project.

```

# Notebook descriptions

- 1.0-data_cleaning_selection.ipynb - * Notebook contains code for preparing and cleaning data for next steps.
- 1.1-data_synthesis_manual.ipynb - * Notebook contains steps for resampling original data and visualisation of resampled data.
- 1.2-append_synth_engin_cols.ipynb - * Notebook contains steps for data preparation, including aggregating data by week, generating engineered columns, appending synthetic star rating and sentiment columns, and adding google trend data for items in the subdepartment of interest and the colour of items considered.
- 1.3-decision_tree.ipynb - Notebook contains an initial exploration of the use of decision trees to predict demand.
- 1.4-random_forest.ipynb - Notebook contains an initial exploration of the use of random forests to predict demand. Final selection of the best random forest model is carried out in ‘1.5_optimised_random_forest.ipynb’.
- 1.5-optimised_random_forest.ipynb - * Notebook contains steps getting to final optimised random forest model for demand prediction.
- 1.6-randomsearchCV_v_rf_comparison.ipynb - Notebook contains workup of splitting training data for cross validation and comparison of random forest manually optimised verses hyperparameter tuned.
- 1.7-optimisation-lp-mip.ipynb - * Notebook contains LP/MIP solver using the methodology described in **Analytics for an Online Retailer: Demand
Forecasting and Price Optimization** [link to the paper](https://pubsonline.informs.org/doi/10.1287/msom.2015.0561)
- 1.8-predict_demand_optimise_price.ipynb - * Notebook brings together the POC model, including the demand prediction and price optimisation step. Currently, the step that builds the demand matrix is slow and therefore we do not recommend searching a price space that is too large. 




# Running the complete pipeline
 
The star * indicates which notebooks are directly used in the final pipeline file in the src folder: price_optim.py



------------------------------------------------------------------------------------------------------------------------------

### Installing development requirements
------------

    pip install -r requirements.txt

