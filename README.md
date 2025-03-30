# ACM-TASKS
Pokémon Mega Evolution Classification

Description
This project predicts whether a Pokémon has a Mega Evolution based on its attributes using a Random Forest Classifier.
The dataset is uploaded from local storage (Kaggle dataset) and processed in Google Colab.

Dataset

File Name:Pokemon.csv
Source: Kaggle (Manually uploaded in Google Colab)(dataset downloaded from Kaggle)
Description: Contains Pokémon attributes, including:
Name
Type 1, Type 2
Legendary
Various Stats (HP, Attack, Defense, etc.)
Features

Data Preprocessing:
One-Hot Encoding for categorical features (Type 1, Type 2).
Binary classification target (Mega_Evolution → 1: Yes, 0: No).
Model Training:
Uses Random Forest Classifier.
Splits data into training (80%) and testing (20%).
Model Evaluation:
Confusion Matrix
Confusion Matrix evaluates the model by showing:
True Positives (TP) – Correctly predicted Mega Evolutions.

True Negatives (TN) – Correctly predicted Non-Mega Evolutions.

False Positives (FP) – Wrongly predicted as Mega Evolution.

False Negatives (FN) – Missed Mega Evolutions.

ROC Curve
ROC Curve plots:
True Positive Rate (TPR) vs. False Positive Rate (FPR).

Shows how well the model distinguishes between classes.

Precision-Recall Curve
Precision-Recall Curve helps in cases with class imbalance.
Precision: % of correctly predicted Mega Evolutions out of all predicted Mega Evolutions.

Recall: % of actual Mega Evolutions correctly identified.

Final Output:
Saves predictions to pokemon_mega_classification.csv.
Provides a downloadable CSV file.
Installation & Setup
To run this project in Google Colab:

Upload the Pokemon dataset (Pokemon.csv) manually that is uploaded in the repository:
Language: python
from google.colab import files
uploaded = files.upload()
