## Employee Dataset Preprocessing Project

This project involves preprocessing a dataset containing employee information. The dataset includes various features such as age, salary, department, etc. The preprocessing steps include handling missing values, treating outliers, and performing label encoding for categorical variables.

## Dataset Description
The dataset contains the following columns:

Age: Age of the employee.<br />
Salary: Salary of the employee.<br />
Department: Department in which the employee works.<br />
Years of Experience: Number of years of experience of the employee.<br />
Salary: Salary details of the employee.<br />
Education: Educational qualification of the employee<br />
Projects: Number of projects worked on by the employee<br />


| # |  Column     |  Non-Null Count | Dtype   |  
|---|  ------     | --------------  | -----   | 
| 0 |  Dept       |  31 non-null    | object  |
| 1 |  Age        |  30 non-null    | float64 |
| 2 |  Experience | 29 non-null     | object  | 
| 3 |  Salary     | 31 non-null     | float64 |
| 4 |  Education  | 31 non-null     | object  |
| 5 |  Projects   | 27 non-null     | float64 |



## Data Preprocessing

### Handling Missing Values
Missing values can impact the analysis and modeling process. We will handle missing values by:

-- Using mean/median approach to handle missing value in numerical columns like age, salary and projects. <br />
-- Converting experience column from object dtype to numeric. dtype<br />
-- masking ".","%","?" like characters in the experience column before converting to numeric. dtype<br />
-- Using mode approach to handle missing value in categorical columns like department and education.<br />

### Feature Engineering : Outliers Treatment
Outliers can significantly affect the statistical properties of a dataset and may distort analysis results. We will treat outliers by:

-- Identifying outliers using statistical methods such as Z-score or IQR.<br />
-- Outliers are treated using trimming method or capping method. Trimming method does not suit the requirement of our dataset as it trims almost half of the dataset.<br />


### Label Encoding
Label encoding is a process of converting categorical variables into numerical format. 

-- Label encoding is done for categorical columns  like the "Department" and "Education" using astype approach and sklearn label encoder.<br />
-- since the above methods may assign some relationship between the variable and label, it is not very useful if there is no hierarchy or relationship between variables.<br />
-- Instead we prefer one hot encoding method to label out categorical columns.<br />

