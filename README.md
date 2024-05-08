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

#### using mean/median approach to handle missing value numerical columns like age, salary and projects

Imputing missing numerical values with the mean or median of the respective column.
Imputing missing categorical values with the mode of the respective column.

### Outliers Treatment
Outliers can significantly affect the statistical properties of a dataset and may distort analysis results. We will treat outliers by:

Identifying outliers using statistical methods such as Z-score or IQR.
Removing outliers or replacing them with a suitable value based on the context of the data.
Label Encoding
Label encoding is a process of converting categorical variables into numerical format. We will perform label encoding for categorical variables like the "Department" column.
