# Pharmaceutical Investment Analysis

Updated August 2026

Created by Ethan Tran (https://www.linkedin.com/in/tranethan/) for STAT 444 (Statistical Learning - Advanced Regression).

Data obtained from (https://aact.ctti-clinicaltrials.org).

## Summary

This project aims to predict clinical trial duration for pharmaceutical royalty investment analysis by building a regression tree model, using characteristics known at the time a trial is registered, to provide an estimate that could complement potential royalty investment evaluations. 

Target feature engineered using start and end date variables. Used phase/enrollment/sponsor as core structural drivers, num_sites/num_countries for geographic complexity, and design/eligibility fields as hypothesized secondary drivers.

Preprocessing involved pulling data from a PostgreSQL database. A LightGBM model with hyperparameter tuning and early stopping restriction was evaluated alongside a baseline linear regression model. Achieved significant model improvement (MAE 325.33 vs. 377.27; RMSE 444.02 vs. 640.28). SHAP analysis provided interpretable reasoning for predictions. The model’s output was connected to a pharmaceutical royalty investment use case, informing the timing assumptions that determine the present value of a contingent future royalty payment.

## Setup

Install requirements.txt

Run notebooks in order:
1. Preprocessing.ipynb
2. Modelling.ipynb

Feel free to contact me if you have any questions!
