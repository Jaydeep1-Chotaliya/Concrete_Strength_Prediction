# Project Focus on concrete strength prediction.
![darryl-low-pXqZs5TG2HU-unsplash](https://github.com/Jaydeep1-Chotaliya/Concrete_Strength_Prediction/assets/129647680/1eea7415-cf06-418a-87aa-4cb0f7234d66)

# **INTRODUCTION**

The Compressive Strength of Concrete determines the quality of Concrete. The project focuses on predicting the compressive strength of concrete. Concrete is a fundamental construction material known for its strength and durability, making it a cornerstone of modern infrastructure. The power of concrete plays a critical role in ensuring the safety and stability of structures. Predicting concrete strength accurately is essential for engineers and builders to design and construct resilient and safe buildings. Traditional methods of predicting concrete strength often rely on extensive testing and empirical formulas, which can be time-consuming and costly.

## **Outline of the problem to solve** ##

* Objective: Develop an accurate and reliable Machine Learning (ML) model for predicting concrete strength.
* Importance: Vital in the construction industry, impacting safety, durability, and overall quality of structures.
* Applications: Design structures meeting safety standards, Optimize material usage, and Ensure structural longevity.

# **Methodology:** 

1. The dataset used focuses on concrete mixture parameters essential for predicting strength.

| **Attribute** | **Feature's Meaning** |
| ------------- | :--- |
| Cement  | Amount of cement is mixed (kg in a m3 mixture) |
| Slag  | Amount of Slag is mixed (kg in a m3 mixture) |
| Flyash  | Amount of FlyAsh is mixed (kg in a m3 mixture) |
| Water  | Amount of Water used (kg in a m3 mixture) |
| Superplasticizer  | Amount of Superplasticizer is mixed (kg in a m3 mixture) |
| Coarseaggregate  | Amount of Coarse aggregate is mixed (kg in a m3 mixture) |
| Fineaggregate  | Amount of Fineaggregate is mixed (kg in a m3 mixture) |
| Age  | Time till inspection Day (Days 0-360) |
| csMPa  | Compressive Strength of Column (Target) |

2. Utilized Pandas, and sns to perform exploratory data analysis (EDA), and seamlessly imported the CSV files for comprehensive analysis and further insights extraction.

3. Demonstrated proficiency by developing a dynamic web page showcasing the prediction of User input.

# **Results/Insights:** #

1 According to the observed plot, it is evident that the strength of a concrete column is highly dependent on the type of cement used, superplasticizer content, and age of the concrete.
* These factors play a significant role in determining the overall strength and durability of the concrete structure.

```
fig, ax = plt.subplots(figsize=(10,8))
sns.barplot(x=sorted_correlations.index, y=sorted_correlations,ax=ax)
plt.xticks(rotation=90)
plt.xlabel('Features')
plt.ylabel('Absolute Correlation')
plt.show()
```
![download](https://github.com/Jaydeep1-Chotaliya/Concrete_Strength_Prediction/assets/129647680/9c7f2621-7067-4728-8c72-3bfac3b0ac8e)

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

2 The distribution of concrete strength within the dataset indicates a predominant concentration of data points ranging between 30 csMPa to 50 csMPa. This interval appears to be the most common range for concrete compressive strength.
* Understanding this distribution is crucial, as it provides valuable insights into the typical strength levels observed within the dataset.
* However, it's essential to note that concrete strength can vary significantly based on multiple factors, and analyzing a broader range of strengths is important for a comprehensive understanding of the material's behavior and properties.

```
sns.displot(df, x="csMPa",height=8, aspect=1.5)
plt.show()
```
![disc_plot](https://github.com/Jaydeep1-Chotaliya/Concrete_Strength_Prediction/assets/129647680/ecb01590-1436-4ac6-b362-63acad91e749)

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

3 MACHINE LEARNING MODEL PERFORMANCE

| **Model Name** | **Mean Squared Error (MSE)** | **Mean Absolute Error (MAE)** | **Coefficient Of Determination** |
| ------------- | :---: | :---: | :---: |
| Linear Regression Model  | 74.33 | 6.75 | 0.72 |
| Random Forest Regression | 26.23 | 3.59 | 0.90 |
| Decision Tree Regression | 57.27 | 4.78 | 0.78 |
| Support Vector Regression | 82.27 | 7.12 | 0.69 |

# **Deployment of our project:** #

![Concrete_Strength_Prediction_Video](https://github.com/Jaydeep1-Chotaliya/Concrete_Strength_Prediction/assets/129647680/6ada7331-db6a-4ab4-bc67-198ccd5af754)


* Deployment transitions a project from development/testing to the live production environment.
* Goal: Make the project fully operational for intended users and stakeholders.
* Successful deployment ensures smooth function and value delivery.

# **CONCLUSION**

* The study extensively analyzed Compressive Strength Data.
* Diverse Machine Learning techniques were employed to predict Concrete Compressive Strength.
* Models like Linear Regression, Decision Trees, and Random Forests were utilized and compared.
* The Random Forest Regressor stood out with the lowest RMSE of 5.35, suggesting its high effectiveness.
* This finding underscores the potential of Random Forest for precise compressive strength prediction.

# **Summary of limitations/challenges faced**

* Finding concrete strength is challenging due to the complexity of terminology and processes.

* Essential understanding of terms like aggregate composition, curing conditions, mix proportions, and hydration phases is required.

* Expertise in materials science and civil engineering is necessary for accurate assessment.

* Interpreting testing results and conducting statistical analyses pose additional challenges.

* Correlating findings with real-world applications requires a multidisciplinary approach.

* The provided feature set may not cover all factors influencing concrete strength.

* Factors like structure design, construction methods, and curing environment significantly impact concrete strength.

* Limited features may restrict predictive accuracy and fail to capture all relevant variables.





