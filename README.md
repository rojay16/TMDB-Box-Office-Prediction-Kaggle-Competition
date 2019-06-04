# TMDB-Box-Office-Prediction-Kaggle-Competition in R

The R script in this repostiory was used to generate an entry to the TMDB Box Office Prediction Kaggle Competition.
The entry places in the top 56% of entries. This entry and script demonstartes many aspects of data science. The original data set
required a lot of pre-processing, such as extracting individual actors, directors and producers, from a single string (one string represented the 
entire cast. Thus heavy string manipulation was performed using the package stringr. In additon to this the number of factor levels had
to be reduced (as you have hundreds of actors by algorithms such as random forest can only take a certain number of factor levels). This 
technqiues were used to replace actors, directors, producers ect. with ranks based on the amount of money their movies generated. Other stasitical 
techniques were used such Box-cox transformation to normailize the continous vairables, and multiple imputation using chain equations
to impute missing data. Finally techniques of ensemble modelling were used where a stacked model was generated using several different, random forest, 
gradient boisting and elastic-net regression. 