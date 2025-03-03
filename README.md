# Exploratory-Data-Analysis-on-the-Titanic-Dataset
📚 Project Overview This project involves performing Exploratory Data Analysis (EDA) on the Titanic dataset to uncover insights about passenger demographics, survival rates, and correlations among features. The analysis aims to explore survival patterns and provide business-use insights like customer segmentation, risk assessment, and profiling.

The dataset contains the following columns:

Column Description Data Type PassengerId Unique identifier for each passenger int64, Survived Survival status (0 = No, 1 = Yes) int64, Pclass Passenger class (1 = 1st, 2 = 2nd, 3 = 3rd) int64, Name Passenger's full name object, Sex Passenger's gender object, Age Passenger's age in years float64, SibSp Number of siblings/spouses aboard int64, Parch Number of parents/children aboard int64, Ticket Ticket number object, Fare Fare paid for the ticket float64, Cabin Cabin number object, Embarked Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton) object .

⚙️ Project Workflow

1.Data Loading Imported the Titanic dataset using Pandas. 
2.Displayed the structure and summary of the dataset.
3.Data Cleaning Handled Missing Values: Imputed missing Age values using the median. Filled missing Embarked values with the mode. Treated missing Cabin values as 'Unknown.' Removed Duplicates. Converted Categorical Data: Columns like Sex, Embarked, and Pclass were converted to categorical data types.
4.Univariate Analysis Visualized distributions of features using: Count plots for categorical features (Survived, Pclass, Sex, Embarked). Histograms and KDE plots for numerical features (Age, Fare).
5.Bivariate Analysis Explored relationships between survival and: Gender (higher survival rate for females). Class (passengers in 1st class were more likely to survive). Age and Fare using scatterplots and boxplots.
6.Multivariate Analysis Examined survival patterns by: Gender and Class using stacked bar charts. Correlation Matrix for numerical features.
7.Feature Engineering Created new features: Title: Extracted titles (e.g., Mr., Mrs., Miss) from the Name column. FamilySize: Combined SibSp and Parch (FamilySize = SibSp + Parch + 1). FareRange: Grouped Fare into ranges (low, medium, high).
8.Insights and Conclusions Summarized key findings: Females had a significantly higher survival rate than males. Passengers in 1st class were more likely to survive compared to those in 3rd class. Young children had a higher likelihood of survival. Larger families tended to have lower survival rates. 
🛠️ Technologies Used 
Python: Data analysis and visualization 
Pandas: Data manipulation
Matplotlib and Seaborn:Data visualization 
NumPy: Numerical computations 
📊 Key Insights Survival by Gender: Females had more Survival rate than males. 
Survival by Class: 1st class passengers had more survival rate compared to other class passengers. 
Family Size: Smaller families had better survival rates. 
Fare: Higher fares correlated with higher chances of survival.
