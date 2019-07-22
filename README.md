# Predicting the Quality of Wine
<p align="center">
  <img width="460" height="300" src="images/winedata.jpg">
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

|     | Models Analysed |
| --- | ---             |
| Model | ![image.jpg](images/Models.jpg) |


#### Observation
##### By adding weights , standardised scale data ,include type and a new label qaulityclass (segment quality into 3 categories 1-poor, 2-good and 3-excellent) we see the accuracy increased. The best was for  KNN  88% for n = 16

##### The best score for Logistic regression and Decision Tree was model 4 with 82% and Model 8A with 84% respectively.

#### Conclusion
##### Model8A with KNN provides the highest accuracy of 87% with n=7 and hence that is selected.


[Jupyter Notebook](.WineQuality-Classification/EDA_ModelSelection/LogisticRegression_WineQuality_V1.ipynb)

