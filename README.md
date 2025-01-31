Sonar Dataset - Logistic Regression Classifier
This project demonstrates the application of a Logistic Regression model to classify sonar signals as either belonging to a mine (M) or rock (R) using the Sonar dataset.

Project Overview
The Sonar dataset consists of 208 samples of sonar signals. Each sample has 60 features (values between 0 and 1) representing the signal strength in different frequency bands, and a label at the 61st column indicating the class: either a mine (M) or rock (R).

This code loads the dataset, performs exploratory data analysis (EDA), preprocesses the data, and then trains a Logistic Regression model to predict whether the sonar signal corresponds to a mine or a rock.

Dataset Description
Features: 60 continuous values that represent sonar signal intensities.
Target: 1 class label (either M for mine or R for rock).
Requirements
Python 3.x
Pandas
NumPy
Scikit-learn
How to Run
Clone the repository:

bash
Copy
git clone https://github.com/your-username/sonar-logistic-regression.git
Install the necessary dependencies:

bash
Copy
pip install pandas numpy scikit-learn
Download the Sonar dataset sonar data.csv and place it in the same directory as the script.

Run the script to load the dataset, perform exploratory data analysis, split the data, and train a Logistic Regression model:

bash
Copy
python sonar_classifier.py
Explanation of the Code
Loading and Exploring the Data:

The dataset is loaded into a Pandas DataFrame using pd.read_csv().
The first 5 rows of the data are displayed with df.head().
The describe() method is used to explore the statistical details of the features.
Feature and Target Split:

The features (X) consist of the first 60 columns.
The target (Y) is the last column, which contains the class label (M or R).
Model Training:

The dataset is split into training and testing sets using train_test_split().
A Logistic Regression model is trained using LogisticRegression() from scikit-learn.
Model Evaluation:

The trained model’s accuracy is evaluated on the test data using accuracy_score().
Sample Output
mathematica
Copy
Accuracy of Logistic Regression model: 80.77%
