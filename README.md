# Fitbit-Data-Sleep-score-Prediction. (BioMedical Decision Support Systems)
Sleep score prediction using ML Logistic regression and Kmeans and SHAP 
# Sleep Score Prediction Using Fitbit Data

## Project Overview
This project involves developing a machine learning model to predict the sleep score categories ('excellent', 'good', 'fair', 'poor') of Fitbit users based on their sleep efficiency. The model uses logistic regression to provide predictions and SHAP values to explain the feature contributions to these predictions.

## Dataset
The dataset includes Fitbit data from multiple participants, encompassing heart rate, calories burned, exercise, sleep, steps, and distance. The data is loaded from JSON files and processed to extract relevant features.

Data set is available at : https://datasets.simula.no/pmdata/
## Features
- `efficiency`: Calculated from the sleep data as the ratio of minutes asleep to time in bed, multiplied by 100.
- Other features like active minutes, heart rate, and exercise data are also considered in the broader analysis.

## Model Training
- A logistic regression classifier is trained to predict sleep score categories.
- The model is evaluated using accuracy, precision, recall, and f1-score metrics.
- A confusion matrix is used to visualize the performance of the model.

## Model Interpretation
- SHAP (SHapley Additive exPlanations) values are used to interpret the impact of the `efficiency` feature on the model's predictions.
- Summary plots provide a global interpretation of feature importance.

## Results
- The model shows a high accuracy in predicting sleep score categories, with perfect scores in some instances.
- SHAP values indicate that higher `efficiency` is associated with better sleep scores.

## Installation and Usage
To run this project, ensure you have the following dependencies installed:
- Python 3.6+
- Pandas
- NumPy
- scikit-learn
- matplotlib
- seaborn
- shap

Clone the repository, navigate to the project directory, and run the script:
```bash
git clone https://github.com/9158764767/Fitbit-Data-Sleep-score-Prediction..git
cd Fitbit-Data-Sleep-score-Prediction
pip install -r requirements.txt
python Final_BDSS.ipynb



## Acknowledgements
This project was developed as part of BioMedical Decision Support Systems at University of Verona.
Thanks to all the participants who provided their data for analysis.
Special thanks to Professor Dr. Pietro Sala for guidance and support.
Contact
For any queries regarding this project, please contact Abhishek Hirve at abhishek.hirve@yahoo.com
