# Project Focus on concrete strength prediction.
![giphy](https://user-images.githubusercontent.com/129647680/235920988-7b8cc1ce-93a0-4607-8d6e-4a403a4aa7df.gif)

**1 INTRODUCTION**

The Compressive Strength of Concrete determines the quality of Concrete. Project focuses on predicting the compressive strength of concrete.Concrete is the most important material in civil engineering. Compressive strength of concrete is a highly non-linear function of age and components.Goal is to develop a machine learning model to predict compressive strength accurately.

**2 SOLUTION STRATERGY** 

Problem solution follows the following steps:

**Step 1 Data description :**
The dataset for this project is related to the compressive strength of concrete. It contains information about the various components that make up the concrete mixture, such as cement, blast furnace slag, fly ash, water, superplasticizer, coarse aggregate, fine aggregate, and age.

**Step 2 Data Filtering :**
This step involves finding and removing the NaN value and unnecessary rows and columns that are not a part of the business. Removing the Outliers.

**Step 3 Exploratotry Data Analysis :**
This step follows the finding unique values, Data summary, co-relation of data.

**Step 4 Data Preparation:**
Spliting the data into test and train sets, Data Scaling involved.

**Step 5 Machine Learning Model:**
the aim of step 5 to train Machine learning model on various model like Linear Regression, decision tree, random forest and svm to find the best model suits.

**Step 6 Hyparameter fine tuning:**
firstly selected the best model to applied in the project. it's important to make a fine tuning of the parameters to improve its scores.

**Step 7 Conclusion :**
In conclusion stage which the generation capacity model is tested using unseen data.

**3 DATA INSIGHTS**

There are some Key details found that follows:
![Picture1](https://user-images.githubusercontent.com/129647680/235941184-1f42a310-1c22-43b4-936b-531d8a355770.png)

According to the pairplot it clearly visible that strength of concrete column is more depend on Type of cement used, superplasticizer, and age follows. 

**4 MACHINE LEARNING MODEL PERFORMANCE**
Linear Regression Model

MSE:  74.33225517537028

MAE:  6.759545500527257

R-squared:  0.7242065625693026


Random Forest Regression:

MSE:  26.23927191478157

MAE:  3.5997819047619037

R-squared:  0.9026449691324018

Decision Tree Regression:

MSE:  57.278166617589314

MAE:  4.780041224970553

R-squared:  0.7874819965582393

support vector regression (SVR):

MSE:  82.27210986983023

MAE:  7.12527978537328

R-squared:  0.6947474830119944

**5 CONCLUSION**

The Compressive Strength Data has been analyzed and Machine Learning techniques were applied to predict the Compressive Strength of Concrete. Different models, including Linear Regression and its variations, Decision Trees, and Random Forests were employed to make predictions, and their performances were compared. Among them, the Random Forest Regressor exhibited the lowest Root Mean Square Error (RMSE) of 5.35, indicating it to be a suitable model for this task. Additionally, the algorithm's performance could be further enhanced by fine-tuning the hyperparameters through techniques such as grid search or random search.
