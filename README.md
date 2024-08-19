# credit-risk-classification
![alt text](image.png)


__Instructions__

In this Challenge, you’ll use various techniques to train and evaluate a model based on loan risk. You’ll use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.


_Part 1: Split the Data into Training and Testing Sets_

Open the starter code notebook and use it to complete the following steps:
1. Read the `lending_data.csv` data from the Resources folder into a Pandas DataFrame.
2. Create the labels set (`y`) from the “loan_status” column, and then create the features (`X`) DataFrame from the remaining columns.
3. Split the data into training and testing datasets by using `train_test_split`.


_Part 2: Create a Logistic Regression Model with the Original Data_

Use your knowledge of logistic regression to complete the following steps:
1. Fit a logistic regression model by using the training data (`X_train` and `y_train`).
2. Save the predictions for the testing data labels by using the testing feature data (`X_test`) and the fitted model.
3. Evaluate the model’s performance by doing the following:
    * Generate a confusion matrix.
    * Print the classification report.
4. Answer the following question: How well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels?


_Part 3: Write a Credit Risk Analysis Report_

Write a brief report that includes a summary and analysis of the performance of the machine learning models that you used in this homework. You should write this report as the `README.md` file included in your GitHub repository.

Structure your report by using the report template that `Starter_Code.zip` includes, ensuring that it contains the following:
1. An overview of the analysis: Explain the purpose of this analysis.
    * The logistic regression helps estimate the probability of input by using a binary classification of 0 in 1. In this case 0 is the probability of healthy loans & 1 is the probability of high risk loans. It also helps analyze features and identifying which are of importatnce. Train, test, split is also ran to split, model, & evaulate the data. It allows reproducibility of our data to test multiple times and attempt to prevent overfitting.
2. The results: Using a bulleted list, describe the accuracy score, the precision score, and recall score of the machine learning model.
    * The overall accuracy for the model was 99%
    * Precision for predicitng correct healthy came in at 100%. There was a 99% recall for this model meaning that there is a high case of detecting positive cases & reducing false negatives.
    * precision and recall are also both reliable for our high risk loans with precision coming in at 85% accuracy & 91% recall.The overall instances of our model predicting positive for high risk loans is less than the percentage of healthy loans but it is important to note that there was a higher amount of healthy loans in our data so this may explain the percentage.
3. A summary: Summarize the results from the machine learning model. Include your justification for recommending the model for use by the company. If you don’t recommend the model, justify your reasoning.
    *The logistic regression is able to predict over 85% in accuracy for predicts of 0 (healthy loans) & 1 (high-risk loans). Total accuracy is 99% but users of this data must take into consideration that the model sees a higher number of representation for 0 (healthy loans). The 18765 supports compared to the 619 is something to keep in mind when looking at the 100% precision. Overall, I would recommend using this model with multiple predicition and training sets.

