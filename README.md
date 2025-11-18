# ELECTRICITY-COST-ANALYSIS
ACS PUMS HOUSING DATA (2011-2015) Oregon State University | March 2022, June 2025

This report investigates electricity costs in Oregon households using data from the 2015 American Community Survey (ACS) PUMS dataset. Two core questions guided the analysis: (1) whether apartment residents pay less for electricity than those living in houses, and (2) whether electricity costs can be reliably predicted using household and structural characteristics.

For the explanatory analysis, multiple linear regression models were used to compare electricity costs between apartments and houses while adjusting for number of bedrooms and household size. After refining the model through backward elimination and validating assumptions with residual diagnostics, the reduced model showed strong evidence that residents of houses pay, on average, $19.47 more per month than apartment residents. The 95% confidence interval ($15.96–$22.99) and a p-value < 0.001 confirm that this difference is statistically meaningful.

For the prediction analysis, the dataset was cleaned and reduced to relevant predictors before being split into training and validation sets. Best subset selection using BIC and 10-fold cross-validation identified a 13-predictor model as the strongest candidate. This model achieved an RMSE of $66.93, indicating moderate predictive accuracy. Expanding the model to include interaction terms between NP × BDSP and HFL × RMSP resulted in a slightly lower RMSE of $66.89. Although the numerical improvement is small, ANOVA results (F = 7.404, p < 0.001) show that the interaction terms significantly enhance model fit.

Overall, the analysis provides clear evidence of cost differences between housing types and demonstrates that electricity expenses can be predicted with reasonable accuracy using household characteristics. The findings support both explanatory insight and practical predictive modeling for electricity cost estimation in Oregon.
