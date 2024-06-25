# Description for Data Cleaning, Transforming, and Preparing for AI Model Training.

Name: TARANG VERMA

Company: CODTECH IT SOLUTIONS

ID: CT08DS1310

Domain: ARTIFICAL INTELLIGENCE

Duration: "25th MAY 2024 to 25th JUNE 2024

Description:

1. **Load the Data**: 
    - Install necessary libraries.
    - Import the libraries: `pandas`, `numpy`, and `scikit-learn`.
    - Load the Titanic dataset using `pd.read_csv`.
    - Display the first few rows of the dataset to understand its structure.

2. **Handle Missing Values**:
    - Check for missing values in the dataset using `data.isnull().sum()`.
    - Fill missing values in the 'Age' column with the median age.
    - Fill missing values in the 'Embarked' column with the mode (most frequent value).
    - Fill missing values in the 'Cabin' column with the string 'Unknown'.
    - Drop columns that have too many missing values or are not necessary for model training (e.g., 'PassengerId', 'Name', 'Ticket').

3. **Feature Engineering**:
    - Create a new feature 'FamilySize' by summing 'SibSp' (siblings/spouses) and 'Parch' (parents/children) and adding 1.
    - Drop the original 'SibSp' and 'Parch' columns since they are now represented by 'FamilySize'.
    - Extract the title from the 'Name' column to create a new feature 'Title'.
    - Simplify the titles by grouping rare titles into a common category and standardizing similar titles (e.g., 'Mlle' and 'Ms' to 'Miss').

4. **Encode Categorical Variables**:
    - Use `LabelEncoder` from `scikit-learn` to convert categorical variables into numerical format.
    - Encode the 'Sex', 'Embarked', and 'Title' columns to transform them into numerical values suitable for machine learning algorithms.

5. **Scale Numerical Features**:
    - Use `StandardScaler` from `scikit-learn` to scale numerical features.
    - Normalize or standardize the 'Age', 'Fare', and 'FamilySize' columns to ensure they have a mean of 0 and a standard deviation of 1, which helps in stabilizing the training process of the machine learning model.

6. **Split the Data**:
    - Separate the features (X) and the target variable (y).
    - Use `train_test_split` from `scikit-learn` to split the data into training and testing sets.
    - Specify the test size (20% of the data) and set a random state for reproducibility.
    - Display the shapes of the training and testing sets to verify the split.

This process covers essential steps in preparing raw data for AI model training, ensuring that the data is clean, transformed, and ready for use in machine learning algorithms.


# OUTPUTS:


![Screenshot 2024-06-25 115958](https://github.com/tarangver/CODTECH-TASK1/assets/122903177/d06ac6e9-065e-4e9a-952d-f0606c78381a)
![Screenshot 2024-06-25 120010](https://github.com/tarangver/CODTECH-TASK1/assets/122903177/00d03897-d0f9-4ec8-9078-184b78d7a6b8)
![Screenshot 2024-06-25 120019](https://github.com/tarangver/CODTECH-TASK1/assets/122903177/23c1ba82-de1d-4fbf-a28b-05e7bdfc8a10)
