# Machine Learning Project

## Team : Alpha (07)
202418005 Anandita Saolapurkar</br>
202418015 Deepanshi Acharya</br>
202418021 Jay Deshpande</br>
202418043 Chandan Pandit

</br>

## Project Overview
This project aims to develop a classification model capable of accurately predicting the outcomes of animals entering the Austin Animal Center. By analyzing historical data on animal intakes and outcomes, the model seeks to assist shelter staff in making informed decisions regarding animal care and placement.
The dataset used was derived from two separate datasets, representing different aspects of the shelter's operations: **Intake Data** and **Outcome Data**. The data from both these sources was cleaned, analyzed, and merged to create a comprehensive dataset. The final dataset included the following columns:

- **Intake_Type:** The type of intake (e.g., Stray, Owner Surrender).
- **Intake_Condition:** The condition of the animal upon intake (e.g., Normal, Medical).
- **Animal_Type:** The species of the animal (e.g., Dog, Cat).
- **Sex_Upon_Intake:** The sex of the animal upon intake (e.g., Neutered Male, Spayed Female).
- **Breed:** The breed of the animal (e.g., Beagle Mix, Domestic Shorthair Mix).
- **Intake_age:** The age of the animal upon intake (in years).
- **Outcome_Type:** The final outcome of the animal (e.g., Adoption, Euthanasia, Transfer).
- **Days_in_Shelter:** The number of days the animal spent in the shelter.

To understand the data and identify potential relationships between variables, we conducted exploratory data analysis (EDA). This involved visualizing the data through various plots, such as bar graph, boxplot and pie chart. Post exploring the data, several classification models were explored including Random Forest, LightGBM, and XGBoost. Hyperparameter tuning was conducted using Random Search Cross-Validation to identify optimal configurations for each model.

#### Dataset Source
Intakes: https://data.austintexas.gov/Health-and-Community-Services/Austin-Animal-Center-Intakes/wter-evkm/about_data </br>
Outcomes: https://data.austintexas.gov/Health-and-Community-Services/Austin-Animal-Center-Outcomes/9t4d-g238/about_data
</br></br>

## Model Development and Evaluation
The project employed a machine learning pipeline to develop and evaluate classification models for predicting animal outcomes. **Random Forest**, **LightGBM**, and **XGBoost** were integrated into the pipeline, and hyperparameter tuning was conducted using **Random Search Cross-Validation** to identify optimal model configurations. Based on comprehensive evaluation metrics, the **XGBoost** model consistently demonstrated superior performance, emerging as the most effective classifier for predicting animal outcomes.

To further enhance the model's predictive capabilities, a **stacking ensemble** was implemented. This approach leveraged the strengths of multiple models by combining their predictions through a meta-classifier. The individual models, including Random Forest, LightGBM, and XGBoost, were trained with their respective best hyperparameters as determined in the previous pipeline. A Random Forest model was employed as the meta-classifier to aggregate the predictions from the individual models.

The **stacking ensemble** achieved **80% accuracy**, showcasing the potential benefits of combining multiple models to improve overall performance.

</br>

## Practical Applications
A few real situations where this model can be deployed are:</br>

1. **Shelter Management:** The model can assist shelter staff in making informed decisions about resource allocation, such as prioritizing medical care or behavioral training for animals with higher risk of negative outcomes.
2. **Policy Development:** The model's insights can inform the development of shelter policies and practices aimed at improving animal welfare and reducing negative outcomes.
</br>

## Conclusion
This project successfully developed a classification model capable of accurately predicting animal outcomes in a shelter. By leveraging historical data on animal intakes and outcomes, the model provides valuable insights for shelter staff to make data-driven decisions regarding animal care and placement. The model's ability to predict outcomes offers a promising avenue for improving animal welfare and resource management within the shelter. This work represents a significant step towards optimizing shelter operations and enhancing the lives of animals in their care.
