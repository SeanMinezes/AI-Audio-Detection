# AI-Audio-Detection
The Dataset can be accessed from the below links:

AI Audio: https://www.kaggle.com/datasets/andreadiubaldo/wavefake-test

Human Audio: https://keithito.com/LJ-Speech-Dataset/

![MFCC new](https://github.com/user-attachments/assets/4fff29e4-d92f-4831-aa1a-37f5b6172e30)

***Feature Extraction***: Using the librosa library, extracted 45 features:

MFCCs (20 features)

Tonal Centroids (6 features)

Spectral Contrast (7 features)

Chromagram (12 features)




***Data Preparation***: Converted 2D feature arrays to 1D by taking the mean across frames.



***Handling Imbalanced Data***: Applied SMOTE to balance the dataset (117,983 AI vs. 13,100 human samples), resulting in 235,966 samples.



***Models Trained:***

Random Forest (Best performer: 98% accuracy)

Decision Tree

XGBoost

Naive Bayes

K-Nearest Neighbors (KNN)

Logistic Regression




***Evaluation:*** Used 10-fold cross-validation with metrics including accuracy, precision, recall, and F1 score.

***Results***

The ***Random Forest*** model outperformed others with:





Accuracy: 98%



Precision: 97%



Recall: 100%



F1 Score: 98%
