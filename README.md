# Health-Insurance-Cross-Sell-Prediction
![health-insurance-comparison](https://github.com/Sid-9823/Health-Insurance-Cross-Sell-Prediction/assets/125801958/9ea8f700-afbc-4bef-86c3-844f4b3ecd3a)


<H2>Problem Statement</H2>

Our client is an Insurance company that specializes in various types of insurance, and now they need our help in building a model that will predict if a policyholder (an existing customer) with Health Insurance is also interested in vehicle insurance.

To build this model, we have data regarding each customer, such as ID, Gender, age, driving license, vehicle age, vehicle damage, etc.

<H2>Project Summary</H2>

<H3>Data collection</H3>

* In the early stages of this project, we loaded and collected our data, stored it in the data frame, and performed some basic analysis like checking out shape, dimensions, etc.

<H3>EDA</H3>

* In the process of EDA, we followed the thumb rule of analysis, i.e., UBM (univariate, bivariate, and Multivariate Analysis).

* In Univariate analysis, we checked out the distributions of each numerical feature independently with the help of a distplot and histogram, 
  whereas we used a countplot for categorical features.

* In Bivariate analysis, we plotted our target variable 'res' against each independent feature with the help of a count plot and histogram to 
  derive valuable insights.

* In Multivariate analysis, we used the Python library 'sweetviz' to perform multivariate analysis, and we also used 'correlation Heatmap'.

<H3>Hypothesis Testing</H3>

We performed our Hypothesis on these 3 statements :

* The average yearly rate for auto insurance is more than 15,000.

* The average consumer is over 29 years old.

* The yearly premium standard deviation is 15,000.

We used Z-test and chi2 test to derive our conclusions.

<H3>Feature engineering and Data preprocessing</H3>
  
* No outliers were detected in our independent numerical features, excluding 'Annual Premium'.

* We used the trimming technique for our outlier treatment.

</H4>In our 'Data preprocessing' part:</H4>

* We used the VIF (Variance Inflation Factor) method to check out the correlation between numerical features but found none.

* We performed 'One Hot Encoding' on our dataset and removed the first encoded feature to avoid multicollinearity, and we also dropped the 
  'Driving Licence column.

* Our target variable was heavily imbalanced, so to reduce the difference between both classes, we used the SMOTE technique to balance our 
  dataset.

<H3>Model Training</H3>

* We performed a train-test split of 80:20 in our dataset.

* In the next step, we scaled our data with the help of StandardScaler().

<H4>Model Implementation :</H4>

* In the data frame below are all the evaluation metrics and models that we implemented on our dataset:

* In the model implementation part, we used 5 models on our datasets: Logistic Regression, Decision Tree, Random Forest, Naive Bayes, and 
  Gradient Boosting.

**Logistic Regression**

**Accuracy score = 81%, F1 - score = 83%, Roc Auc score = 81%**

**Decision Tree**

**Accuracy score = 81%, F1 - score = 81%, Roc Auc score = 81%**

**Random Forest**

**Accuracy score = 87%, F1 - score = 87%, Roc Auc score = 87%**

**Naive Bayes**

**Accuracy score = 80%, F1 - score = 82%, Roc Auc score = 80%**

**Gradient Boosting**

Accuracy score = 83%, F1 - score = 84%, Roc Auc score = 83%

*The Random forest Classifier has the highest F1 score of 87% for the test Set among all models. There is no evidence of overfitting.

*No overfitting is seen.

Finally, the insurance business may apply a machine learning model based on the Random Forest Classifier to forecast if an existing health insurance client would be interested in a motor insurance policy. The firm may increase the conversion rate by taking initiatives to encourage individuals to get automobile insurance by giving incentives or simplifying the application and claim settlement procedures. Because the client acquisition cost stays zero, cross-selling may be an efficient way to boost earnings.
