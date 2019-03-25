# ML_codebasics
Simple tasks on Machine Learning algorithms
## Content
### 1. linear regression
Using *canada_per_capita_income.csv* file build a regression model and predict the per capita income for canadian citizens in year 2020

### 2. multivariate linear regression
File *hiring.csv* contains hiring statics for a firm such as experience of candidate, his written test score and personal interview score. Based on these 3 factors, HR will decide the salary. Given this data, you need to build a machine learning model for HR department that can help them decide salaries for future candidates. Using this predict salaries for following candidates:
* 2 yr experience, 9 test score, 6 interview score
* 12 yr experience, 10 test score, 10 interview score

### 3. gradient descent
Being given *test_scores.csv* file with Mathematical and Computer Science student's test scores you are to find out the correlation between scores of these subjects.
* For test scores in .csv file, run gradient descent algorithm to find out value of m, b and appropriate learning rate
* On each iteration, compare previous cost with current cost. Stop when costs are similar (use *math.isclose* function with *1e-20* threshold)
* Now using sklearn.linear_model find coefficient (i.e. m) and intercept (i.e. b). Compare them with m, b generated by your gradient descent algorithm

### 4. one hot encoding
The *carprices.csv* file has car sell prices for 3 different models. First plot data points on a scatter plot chart to see if linear regression model can be applied. If yes, then build a model that can answer following questions:
* Predict price of a mercedez benz that is 4 yr old with mileage 45000
* Predict price of a BMW X5 that is 7 yr old with mileage 86000
* Tell the score (accuracy) of your model (hint: use LinearRegression().score())

### 5. logistic regression
Using the *HR_comma_sep.csv* file downloaded from [Kaggle](https://www.kaggle.com/giripujar/hr-analytics) with employee retention dataset solve the following tasks:
* Do some exploratory data analysis to figure out which variables have direct and clear impact on employee retention (i.e. whether they leave the company or continue to work)
* Plot bar charts showing impact of employee salaries on retention
* Plot bar charts showing corelation between department and employee retention
* Now build logistic regression model using variables that were narrowed down in step 1
* Measure the accuracy of the model

### 6. multiclass logistic regression
Use *sklearn.datasets* iris flower dataset to train your model using logistic regression. You need to figure out accuracy of your model and use that to predict different samples in your test dataset. In iris dataset there are 150 samples containing following features:
* Sepal Length
* Sepal Width
* Petal Length
* Petal Width

Using above 4 features you will clasify a flower in one of the three categories:
* Setosa
* Versicolour
* Virginica

### 7. decision tree
Using the *titanic.csv* file with passengers dataset, specifically fields *Survived, Pclass, Sex, Age, Fare*, predict the survival rate based on specified features.

### 8. svm
Train SVM classifier using sklearn digits dataset (i.e. *from sklearn.datasets import load_digits*) and then:
* Measure accuracy of your model using different kernels such as *rbf* and *linear*
* Tune your model further using regularization and gamma parameters and try to come up with highest accurancy score
* Use 80% of samples as training data size

### 9. random forest
Use famous iris flower dataset from *sklearn.datasets* to predict flower species using random forest classifier.
* Measure prediction score using default n_estimators (10)
* Now fine tune your model by changing number of trees in your classifer and tell what best score you can get using how many trees
