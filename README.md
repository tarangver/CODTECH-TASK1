# Description for Data Cleaning, Transforming, and Preparing for AI Model Training.
Name: TARANG VERMA

Company: CODTECH IT SOLUTIONS

ID: CT08DS1310

Domain: ARTIFICAL INTELLIGENCE

Duration: "25th MAY 2024 to 25th JUNE 2024


Description:


1. Load the Data:
   
		i. Install necessary libraries.

		ii. Import the libraries: pandas, numpy, and scikit-learn.

		iii. Load the Titanic dataset using pd.read_csv.

		iv. Display the first few rows of the dataset to understand its structure.

2. Handle Missing Values:

		i. Check for missing values in the dataset using data.isnull().sum().

		ii. Fill missing values in the 'Age' column with the median age.

		iii. Fill missing values in the 'Embarked' column with the mode (most frequent value).

		iv. Fill missing values in the 'Cabin' column with the string 'Unknown'.

		v. Drop columns that have too many missing values or are not necessary for model training (e.g., 'PassengerId', 'Name', 'Ticket').

3. Feature Engineering:

		i. Create a new feature 'FamilySize' by summing 'SibSp' (siblings/spouses) and 'Parch' (parents/children) and adding 1.

		ii. Drop the original 'SibSp' and 'Parch' columns since they are now represented by 'FamilySize'.

		iii. Extract the title from the 'Name' column to create a new feature 'Title'.

		iv. Simplify the titles by grouping rare titles into a common category and standardizing similar titles (e.g., 'Mlle' and 'Ms' to 'Miss').

4. Encode Categorical Variables:

		i. Use LabelEncoder from scikit-learn to convert categorical variables into numerical format.

		ii. Encode the 'Sex', 'Embarked', and 'Title' columns to transform them into numerical values suitable for machine learning algorithms.

5. Scale Numerical Features:

		i. Use StandardScaler from scikit-learn to scale numerical features.

		ii. Normalize or standardize the 'Age', 'Fare', and 'FamilySize' columns to ensure they have a mean of 0 and a standard deviation of 1, which helps in stabilizing the training process of the machine learning model.

6. Split the Data:

		i. Separate the features (X) and the target variable (y).

		ii. Use train_test_split from scikit-learn to split the data into training and testing sets.

		iii. Specify the test size (20% of the data) and set a random state for reproducibility.

		iv. Display the shapes of the training and testing sets to verify the split.

This process covers essential steps in preparing raw data for AI model training, ensuring that the data is clean, transformed, and ready for use in machine learning algorithms.



# OUTPUTS:


![Screenshot 2024-06-25 113748](https://github.com/tarangver/CODTECH-TASK1/assets/122903177/6af7e937-b0c4-4481-a60b-ffe1e2a251a2)
![Screenshot 2024-06-25 113807](https://github.com/tarangver/CODTECH-TASK1/assets/122903177/51bf7b5e-5144-4ccb-b70b-8bbf0a1e3fc3)
![Screenshot 2024-06-25 113827](https://github.com/tarangver/CODTECH-TASK1/assets/122903177/ae90cff0-3b20-4357-8d2f-9fedcc5fc006)
![Screenshot 2024-06-25 113845](https://github.com/tarangver/CODTECH-TASK1/assets/122903177/9cc30f06-9b62-46fd-96ba-a0a1688a4a61)
![Screenshot 2024-06-25 113856](https://github.com/tarangver/CODTECH-TASK1/assets/122903177/c51befd8-60cf-4b92-9ca2-3b10e9052e8a)
