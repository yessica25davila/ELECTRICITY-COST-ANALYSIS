# ELECTRICITY-COST-ANALYSIS
ACS PUMS HOUSING DATA (2011-2015) Oregon State University | March 2022, June 2025

This report investigates electricity costs in Oregon households using data from the 2015 American Community Survey (ACS) PUMS dataset. Two core questions guided the analysis: 

(1) Whether apartment residents pay less for electricity than those living in houses. The findings showed that residents living in an Oregon household pay, on average, $19.47 more per month than Oregon apartment residents.  
(2) Whether electricity costs can be reliably predicted using household and structural characteristics. I developed a model to estimate household electricity costs in Oregon and found the model's predictions were within about $67 of actual costs. 


For the explanatory analysis, multiple linear regression models were used to compare electricity costs between apartments and houses while adjusting for number of bedrooms and household size.

<img width="430" height="225" alt="image" src="https://github.com/user-attachments/assets/08467a1d-753e-48a3-8553-4f89317e141a" />


<img width="430" height="225" alt="image" src="https://github.com/user-attachments/assets/017fa829-eaa7-4f90-9acc-0d2b4cbb55e8" />


After refining the model through backward elimination and validating assumptions with residual diagnostics, the reduced model showed strong evidence that residents of houses pay, on average, $19.47 more per month than apartment residents. The 95% confidence interval ($15.96–$22.99) and a p-value < 0.001 confirm that this difference is statistically meaningful.


For the prediction analysis, the dataset was cleaned and reduced to relevant predictors before being split into training and validation sets. Best subset selection using BIC and 10-fold cross-validation identified a 13-predictor model as the strongest candidate. This model achieved an RMSE of $66.93, indicating moderate predictive accuracy. Expanding the model to include interaction terms between NP × BDSP and HFL × RMSP resulted in a slightly lower RMSE of $66.89. Although the numerical improvement is small, ANOVA results (F = 7.404, p < 0.001) show that the interaction terms significantly enhance model fit.

Overall, the analysis provides clear evidence of cost differences between housing types and demonstrates that electricity expenses can be predicted with reasonable accuracy using household characteristics. The findings support both explanatory insight and practical predictive modeling for electricity cost estimation in Oregon.
