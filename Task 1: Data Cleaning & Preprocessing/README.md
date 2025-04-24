1. Importing Libraries and Reading the Dataset:
Imported essential Python libraries like numpy, pandas, and matplotlib.

Loaded the Titanic dataset into a DataFrame using pd.read_csv.

2. Exploring the Dataset:
Used df.head(), df.shape, and df.info() to examine the dataset's structure, column data types, and missing values.

Checked missing values in each column using df.isnull().sum().

3. Handling Missing Values:
Age:

Replaced missing values with the mean of the Age column using df['Age'].fillna(df['Age'].mean()).

Cabin:

Replaced missing values with the mode of the Cabin column using df['Cabin'].fillna(df['Cabin'].mode()[0]).

Embarked:

Dropped rows with missing values in the Embarked column using df.dropna(subset='Embarked').

4. Converting Categorical Data to Numerical:
Used LabelEncoder to encode categorical columns:

Sex: Encoded male/female as 1/0.

Embarked: Encoded the embarkation points into numerical values.

5. Dropping Irrelevant Columns:
Removed columns not essential for analysis: Cabin, Name, Ticket, and PassengerId.

6. Preparing Features and Target Variable:
Separated features (X) and target variable (y):

X: Features excluding Survived.

y: Target column (Survived).

7. Standardizing Numerical Features:
Standardized columns like Age, SibSp, Parch, and Fare using StandardScaler to normalize the data for better model performance.

8. Visualizing Outliers with Box Plot:
Created box plots for Fare and Age to identify and visualize outliers.

9. Handling Outliers Using IQR:
Calculated the Interquartile Range (IQR) and defined upper and lower bounds:

Removed rows where Fare or Age values fell outside these bounds.

Verified outliers were removed by ensuring no points were beyond the whiskers in subsequent box plots.

Final Outcome:
The processed DataFrame now has no missing values, and outliers have been removed for Fare and Age.

The dataset is ready for further analysis or model building.
