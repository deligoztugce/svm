# svm
Iris Dataset Analysis using SVM

This project demonstrates the use of Support Vector Machines (SVM) to classify iris species based on their physical characteristics. The analysis includes data preprocessing, model training, evaluation, and visualization.

Table of Contents

Dataset Overview

Modeling Approach

Results and Visualization

Dependencies

How to Run the Project

Notes

License

Dataset Overview

The Iris dataset consists of 150 records with the following features:

Sepal Length (cm)

Sepal Width (cm)

Petal Length (cm)

Petal Width (cm)

Species: Target variable with three classes:

Setosa

Versicolor

Virginica

The dataset is balanced, with each species represented by 50 samples.

Modeling Approach

1. Data Preprocessing

Feature Scaling: Standardized all features using StandardScaler.

Train-Test Split: Split the data into training (80%) and testing (20%) sets.

2. SVM Model

Kernel: Linear kernel.

Training: The model was trained using the standardized training data.

3. Evaluation Metrics

Accuracy: Overall accuracy of the model.

Classification Report: Precision, recall, and F1-score for each class.

Confusion Matrix: Heatmap of true versus predicted labels.

Results and Visualization

Accuracy

Full Feature Model: Achieved 96.67% accuracy.

Visualization Model: Also achieved 96.67% accuracy using only the first two features (Sepal Length and Sepal Width).

Classification Report (Full Feature Model)

              precision    recall  f1-score   support

      setosa       1.00      1.00      1.00        10
  versicolor       1.00      0.89      0.94         9
   virginica       0.92      1.00      0.96        11

    accuracy                           0.97        30
   macro avg       0.97      0.96      0.97        30
weighted avg       0.97      0.97      0.97        30

Decision Boundary

Visualized decision boundaries using only Sepal Length and Sepal Width.

Confusion Matrix

A heatmap of the confusion matrix illustrates the model's performance on the test set.

Dependencies

Python 3.9+

Required Libraries:

numpy

pandas

scikit-learn

matplotlib

seaborn

How to Run the Project

Clone the repository:

git clone <repository-url>
cd <repository-folder>

Install dependencies:

pip install -r requirements.txt

Run the script:

python main.py

View outputs:

Classification reports and accuracy metrics in the terminal.

Decision boundary visualization and confusion matrix plots displayed during execution.

Notes

The SVM model performed exceptionally well on the Iris dataset.

Additional kernels (e.g., RBF) can be tested for further insights.

Use cross-validation for more robust evaluation.

License

This project is licensed under the MIT License. See the LICENSE file for details.
