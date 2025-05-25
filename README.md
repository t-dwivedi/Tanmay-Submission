# CampusPulse (Machine Learning-Task 1) CodingWeek 2025
## Objective
To predict using academic and behavioral pattern that a student is in a romantic relationship using predictive modelling.
Along the way implementing process to clean the data and deriving certain relations between different parameters realising and discovering trends and how data behaves.
## Technologies Used
- Python
- pandas , numpy
- seaborn,matplotlib
- scikit-learn
- SHAP
- Jupyter Notebook
## Task Breakdown
### LEVEL 1: Feature identification
Used EDA (heatmap) to guess the meaning of anonymised features :  Feature_1 , Feature_2 , Feature_3.
The process to identify involved first isolating out the categories with numerical value and then making a correlational heatmap out of them . The columns that were majorly related with each of the feature were combined and collectively used to derive a calculative and intiutional conclusion of what each feature would mean. 
### LEVEL 2: Data pre-processing
Like every survey data the dataset has numerous missing data.The first task was to identify how many colums to deal with missing values.The logic to predict the null values was different for each column. For example - The missing values of Fedu , Fedu was closely related to Medu to visualise that a violinplot was made the made the relation clear. KNN was used to predict the missing values of Fedu. Some columns which did not have any important_feature affecting them , were filled with mode to ensure data regularity.
### LEVEL 3: Insightful Questions
The main objective was to visualise and get to know the data better by asking some questions.Five question which seemed relevant to the data as well as had importance over campus life and could be visualised were chosen. Though most of the data was regular , answers to some question turned out to be completely opposite of what was thought.Dominance in relation of few columns was observed. For example- Over the whole dataset Mother was found to be the primary guardian no other factor weighing just plain trend.
### LEVEL 4: Prediction Model
At the end a predictive model was to be decided to check whether the student selected is in a romantic relationship or not. A few model like Logistic regression , SVM , RandomForest were used and then there accuracy score was checked . RandomForest out of all was the winning model with the accuracy of 6.07.
### LEVEL 5: Explanibility
For the optimal model, which in this case was the Random Forest Classifier, SHAP was used to interpret its predictions.

As shown in the Summary Plot, factors such as sex, freetime, health, … were prominently weighted in the predictions.

Local Explanations (Force plots) helped explain the model's rationale for a single "Yes" and "No" prediction, which enabled visualizing the individual logic behind these decisions.

## KEY INSIGHTS
- Social activity (`goout`) was the most predictive of relationship status
- Absences and an anonymized feature (`Feature_1`) also had high influence
- Students with higher `goout` and `Feature_1` scores were more likely to be in a relationship

## HOW TO RUN THIS PROJECT
1. Open the notebook: `Project.ipynb`
2. Run all cells in order
3. Upload the dataset file if prompted
4. Install SHAP (`pip install shap`) to run the explainability part

## Credits
Project developed for:
**Coding Week 2025 – Machine Learning Task 1**  
Organized by Coding Club, IIT Guwahati
