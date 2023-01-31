# Lasso_Ridge_Assign

## Table of contents:

  - Load Data
  - Dataset Cleaning
  - Data Visualization
  - Data Preaparation
  - Dummy Variables
  - Rescaling of Features
  - Splitting the Data into Training and Testing
  - Building and Evaluation of the model
    
    
### 1. Load Data:
First of all we just loaded the libraries and then loaded the dataset.

### 2. Dataset Cleaning:
Handeled missing values.
We removed the columns that are having more that 80% missing values.
Categorical Variable's missing value are imputed by mode.

### 3. Data Visualization:
After that visualization of continuous variablesis are done by plotting the pairplot and also heatmap is plotted to see the correlation between variables.

Dropped the variables that are highly correlated:

GarageCars and GarageArea are having correlation of 88%.

TotRmsAbvGrd and GrLivArea are having correlation of 83%.

TotalBsmtSF and 1stFlrSF are having the correlation of 82%.

Dropping 'TotalBsmtSF', 'TotRmsAbvGrd', 'GarageArea' columns.

### 4. Data Preparation:

Now it can be seen that some of the variables are having more than two levels. So we have to create dummy variables for them. To do so, those variables are converted into Categorical Variables. 

### 5.Dummy Variables:

After that, Dummy variables for all the categorical variable that are having more than two levels are added. and the first dummy variable for all the features are dropped because they were not needed. And after dropping them, we concatenate those dummy variables with the original dataset.
After That we dropped the original feature because we have created dummy variables for them.

### 6. Feature Scaling:
Scaling of the features is done after that.

### 7. Splitting the Data into Training and Testing:
After that, data is splitted into training and testing. Here 70% data is splitted into training set and 30% of data will be there for testing purpose.

### 8. Building and Evaluation of the model:
First of all we applied Linear regression model. and we saw that there was a problem of overfitting. 

To handle the overfitting, we applied Ridge and Lasso Regression.
We saw that r2 score for both the test data in case of both the models is improved.

Thus We handled overfitting problem.
