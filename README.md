# Predicting the Quality of Wine
<p align="center">
  <img width="460" height="300" src="images/TRAIsNewRules.jpg">
</p>


## INTRODUCTION
The goal is to predict quality of wine amongst the list of red and white wines using Logistic regression, KNN and Decision Tree. 
The dataset consists of the information about physicochemical tests on the different varieties of wines. 
Various variables present in the dataset includes data of fixed acidity, volatile acidity, citric acid, ph, alcohol etc. 
The dataset comprises of (red wine - 1599 observations; white wine - 4898 observations) with 12 columns. 
Below is a table showing names of all the columns and their description.

## DATA
| Column Name           | Description                                              |
| -------------         |-------------                                             | 
| fixed acidity         | Fixed acidity content                                    | 
| volatile acidity      | Volatile acidity content                                 |  
| citric acid           | citric acid content in ml                                | 
| residual sugar        | Residual sugar content                                   |   
| chlorides             | Chlorides content                                        |
| free sulfur dioxide   | Free sulphur dioxide content                             |
| total sulfur dioxide  | Total Sulphur dioxide content                            |
| density               | Density                                                  |
| pH                    | pH value                                                 |
| sulphates             | sulphate content                                         |
| alcohol               | alcohol content in ml                                    |
| quality               | Output Variable - score between 0 and 10                 |


## PROJECT ANALYSIS
| Description | Analysis |
| --- | --- |
| Channels_Data.head | ![image.png](images/PrimaryMasterData.png) |
| Sample_Data | ![image.png](images/SampleUsers.png) |


### CONCLUSION
| Model | ModelName|Scaled?|	Outliers?|	Include Type?|	Added Qlty Cat?|	Added Wts?|	Logit_score|	KNN_score|	DTREE_score |         | ------|----------|-------|-----------|---------------|-----------------|------------|------------|-----------|--------------|
|0	|Model 1	|No	  |Yes	|No	  |No	  |No	  |0.522308	|0.482308	|0.585385|
|1	|Model 1A	|No	  |Yes	|No	  |No	  |Yes	|0.441538	|0.601538	|0.600000|
|2	|Model 2	|No	  |Yes	|Yes	|No	  |No	  |0.517692	|0.480800	|0.590000|
|3	|Model 2A	|No	  |Yes	|Yes	|No	  |Yes	|0.433846	|0.616200	|0.585385|
|4	|Model 3	|No	  |Yes	|Yes	|Yes	|No	  |0.819231	|0.803800	|0.845385|
|5	|Model 3A	|No	  |Yes	|Yes	|Yes	|Yes	|0.790769	|0.870000	|0.833846|
|6	|Model 4	|No	  |Yes	|No	  |Yes	|No	  |0.820769	|0.804600	|0.837692|
|7	|Model 4A	|No	  |Yes	|No	  |Yes	|Yes	|0.790769	|0.870800	|0.840769|
|8	|Model 5	|No	  |No	  |No	  |No	  |No	  |0.545455	|0.483700	|0.617829|
|9	|Model 5A	|No	  |No	  |No	  |No	  |Yes	|0.422771	|0.620500	|0.590468|
|10	|Model 6	|No	  |No	  |Yes	|No	  |No	  |0.547220	|0.481900	|0.599294|
|11	|Model 6A	|No	  |No	  |Yes	|No	  |Yes	|0.429832	|0.618700	|0.607237|
|12	|Model 7	|No	  |No	  |Yes	|Yes	|No	  |0.807590	|0.815500	|0.833186|
|13	|Model 7	|No	  |No	  |Yes	|Yes	|Yes	|0.778464	|0.857900	|0.849956|
|14	|Model 8	|Yes	|No	  |Yes	|Yes	|No	  |0.817299	|0.847300	|0.832304|
|15	|Model 8A	|Yes	|No	  |Yes	|Yes	|Yes	|0.776699	|0.885300	|0.849956|

#### Observation
##### By adding weights , standardised scale data ,include type and a new label qaulityclass (segment quality into 3 categories 1-poor, 2-good and 3-excellent) we see the accuracy increased. The best was for  KNN  88% for n = 16

##### The best score for Logistic regression and Decision Tree was model 4 with 82% and Model 8A with 84% respectively.

#### Conclusion
##### Model8A with KNN provides the highest accuracy of 87% with n=7 and hence that is selected.


[Jupyter Notebook](.WineQuality-Classification/EDAReport/EDAnotebookTRAI-Usecase-Ver3.ipynb)

