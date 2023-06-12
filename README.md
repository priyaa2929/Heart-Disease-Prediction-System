
# Heart Disease Prediction System

The aim of this project is to implement the heart disease prediction application. Many people all over
the world nearly 60% of the world’s population are now-a-days suffering from heart disease. 
Proposed system consists of an intelligent system which works on different data mining techniques and machine learning algorithms like, “Logistic Regression", " Naïve Bayes", "Support Vector Machine", "K-Nearest Neighbors", "Decision Tree", "Random Forest" to predict the heart disease based on some health parameters.

<br />

## Keywords

Logistic Regression, Naïve Bayes, Support Vector Machine, K-Nearest Neighbors, Decision Tree, Random Forest
<br />

## Dataflow Diagram
<br />
![image](https://github.com/priyaa2929/Heart-Disease-Prediction-System/assets/130492957/2dc32686-26c9-493f-83a2-b6f6364e37a3)
<br />

<br />
## Dataset Description

The heart data set originated from Kaggle website, which contains medical information of patients, including their
1. age
2. sex
3. chest pain type (4 values)
4. resting blood pressure
5. serum cholestoral in mg/dl
6. fasting blood sugar > 120 mg/dl
7. resting electrocardiographic results (values 0,1,2)
8. maximum heart rate achieved
9. exercise induced angina
10. oldpeak = ST depression induced by exercise relative to rest
11. the slope of the peak exercise ST segment
12. number of major vessels (0-3) colored by flourosopy
13. thal: 0 = normal; 1 = fixed defect; 2 = reversable defect The names and social security numbers of the patients were recently removed from the database, replaced with dummy values.

<br />

## Methodolgy

In this section we shall learn about the various classifiers used in machine learning to predict heart disease. We shall also explain our proposed methodology to improve the accuracy. The different methods used are defined below. The output is the accuracy metrics of the machine learning models. 

We performed exploratory data analysis (EDA) on the dataset to gain insights into the data and visualize the distribution of the features. We then split the data into training and testing sets. Heart dataset containing 303 cases.
<br />

![image](https://github.com/priyaa2929/Heart-Disease-Prediction-System/assets/130492957/0195ec08-21b8-434c-9164-4d6e3b3eee68)
<br />

➔ The heart data set consists of 303 data points, with 14 features each.
➔ “target” is the feature we are going to predict, 0 means No disease, 1 means heart disease.
<br />
![image](https://github.com/priyaa2929/Heart-Disease-Prediction-System/assets/130492957/60138479-1a41-4439-b9d6-72c1ef4dd03d)
<br />
➔ There is no null values in dataset.
<br />

#Correlation Matrix:
<br />
![image](https://github.com/priyaa2929/Heart-Disease-Prediction-System/assets/130492957/e1130491-a8e1-4f5a-b1a3-1400038e53a7)
<br />

#Heatmap:
<br />
![image](https://github.com/priyaa2929/Heart-Disease-Prediction-System/assets/130492957/705214c9-1977-425b-82a2-f76b6a130cca)
<br />

#EDA for TARGET class:
The above graph shows that the data is biased towards datapoints having target value as 0 where it means that heart disease was not present actually. The number of heart patients is almost same as the number of diabetic patients.
<br />
![image](https://github.com/priyaa2929/Heart-Disease-Prediction-System/assets/130492957/143b55e9-3926-429e-b365-ca0cb9fee2ad)
<br />

#Analyzing the ‘sex’ feature:
<br />
![image](https://github.com/priyaa2929/Heart-Disease-Prediction-System/assets/130492957/6da39b74-34d0-44bf-b73f-91982dc02dfa)
<br />

#Analyzing the ‘chest pain type’ feature:
<br />
![image](https://github.com/priyaa2929/Heart-Disease-Prediction-System/assets/130492957/2ce3cb20-519d-4535-93f5-4a42c8e3b545)
<br />

#Analyzing the ‘fbs’ feature:
<br />
![image](https://github.com/priyaa2929/Heart-Disease-Prediction-System/assets/130492957/0db539dc-1129-4ee9-b61a-fae9e49dd534)
<br />

#Analyzing the ‘thal’ feature:
<br />
![image](https://github.com/priyaa2929/Heart-Disease-Prediction-System/assets/130492957/76e3ceee-675c-4c7a-8e82-b12e63fd6346)
![image](https://github.com/priyaa2929/Heart-Disease-Prediction-System/assets/130492957/bef09305-e6c6-4208-88b3-1c7c5fce873a)
<br />

#Train Test Split (Training And Validation)
<br />
![image](https://github.com/priyaa2929/Heart-Disease-Prediction-System/assets/130492957/2c50e96d-58ac-4987-874e-d8640ee97ad1)
<br />

#Model Fitting:
<br />
![image](https://github.com/priyaa2929/Heart-Disease-Prediction-System/assets/130492957/2f164a2c-0d5f-4e12-b5f6-0da709d92b72)
<br />

#Algorithms Used:
#k-Nearest Neighbors:
The k-NN algorithm is arguably the simplest machine learning algorithm. Building the model consists only of storing the training data set. To make a prediction for a new data point, the algorithm finds the closest data points in the training data set, its “nearest neighbors.”
The accuracy score achieved using KNN is: 67.21 %
<br />
![image](https://github.com/priyaa2929/Heart-Disease-Prediction-System/assets/130492957/01fe5b09-d4a2-4a30-964d-d32a6786deb9)
<br />

#Logistic regression:
Logistic Regression is one of the most common classification algorithms.
The accuracy score achieved using Logistic Regression is: 85.25 %
<br />
![image](https://github.com/priyaa2929/Heart-Disease-Prediction-System/assets/130492957/ee712949-8379-43db-b17f-7d98ba8f8cb8)
<br />

#Decision Tree:
This classifier creates a decision tree based on which, it assigns the class values to each data point. Here, we can vary the maximum number of features to be considered while creating the model.
The accuracy score achieved using Decision Tree is: 81.97 %
<br />
![image](https://github.com/priyaa2929/Heart-Disease-Prediction-System/assets/130492957/c18800ab-b007-40c3-8dd1-9da860383c8c)
<br />

#SVM:
Support Vector Machine is a supervised learning algorithm used for classification and regression analysis. It works by finding the hyperplane that maximally separates the different classes of data. The hyperplane is found by maximizing the margin between the support vectors, which are the data points closest to the decision boundary. The accuracy score achieved using Linear SVM is: 81.97 %
<br />
![image](https://github.com/priyaa2929/Heart-Disease-Prediction-System/assets/130492957/bb55c7a2-808f-4f55-945a-a02a1d64eef3)
<br />

#Naïve Bayes:
Naive Bayes is a probabilistic machine learning algorithm based on Bayes' theorem. It is used for classification and is popularly used for text classification and spam filtering.
The accuracy score achieved using Naive Bayes is: 85.25 %
<br />
![image](https://github.com/priyaa2929/Heart-Disease-Prediction-System/assets/130492957/34cf85ce-4a11-4bed-aae2-beedce2bef8a)
<br />

#Random Forest:
This classifier takes the concept of decision trees to the next level. It creates a forest of trees where each tree is formed by a random selection of features from the total features.
The accuracy score achieved using Decision Tree is: 90.16 %
<br />
![image](https://github.com/priyaa2929/Heart-Disease-Prediction-System/assets/130492957/91347152-25f0-4193-8f3a-6daefcc39d76)
<br />

#Accuracy Comparison:
<br />
![image](https://github.com/priyaa2929/Heart-Disease-Prediction-System/assets/130492957/9cb922f4-0d2f-4dc0-b55f-73e8e5f41765)
<br />

#Graph Comparing Different Algorithms:
<br />
![image](https://github.com/priyaa2929/Heart-Disease-Prediction-System/assets/130492957/18c2e9f7-e546-4930-84d3-09f2726ea84e)
<br />

This shows the accuracy values for all six machine learning algorithms.
It shows that Random forest algorithm gives the best accuracy with 90.16% accuracy.
<br />
## Result and Future Scope

Based on the observations, it seems that the Random Forest algorithm is the best performing model with an accuracy of 90.16%. Logistic Regression and Naive Bayes have similar performance with an accuracy of 85.25%, followed by Support Vector Machine and Decision Tree with 81.97%, and finally K-Nearest Neighbors with 67.21%.

To further improve the model, feature selection and engineering techniques can be applied to identify the most important features for predicting heart disease. This can lead to more accurate models with better generalization. Additionally, hyperparameter tuning can be performed to optimize the model performance.
Furthermore, exploring other machine learning algorithms or ensemble methods like Gradient Boosting or Neural Networks can also improve the accuracy of the model. Finally, the model can be deployed as a web application or mobile application for easy access and use by healthcare professionals or individuals.

The future scope of a heart disease prediction system using machine learning is vast and promising. Some potential areas of development and advancement include:

1. Integration with wearable technology: With the increasing popularity of wearable devices such as smartwatches and fitness trackers, integrating a heart disease prediction system with these devices can provide real-time monitoring and early detection of heart disease. This can allow for timely intervention and preventive care, improving patient outcomes.

2. Use of advanced machine learning algorithms: While the current models used in heart disease prediction are effective, there is scope for further improvement using more advanced machine learning algorithms. For example, deep learning models such as neural networks can be used to capture more complex relationships between the features and the target variable, leading to more accurate predictions.

3. Personalized risk assessment: Machine learning algorithms can be used to develop personalized risk assessment models based on the individual's medical history, lifestyle, and other relevant information. This can provide more accurate risk estimates and tailored treatment recommendations.

4. Integration with electronic health records (EHRs): Integrating the heart disease prediction system with EHRs can provide a comprehensive view of the patient's medical history, allowing for more accurate risk assessment and treatment planning.

5. Mobile application development: Developing a mobile application for heart disease prediction can improve access to healthcare services, especially in rural or remote areas where healthcare facilities are limited. This can provide early detection and intervention for heart disease, reducing healthcare costs and improving patient outcomes.

Overall, the future of heart disease prediction using machine learning is promising, and there is ample scope for development and advancement. With further research and development, these systems can become an essential tool in preventive care and personalized treatment planning.

