# Predict_body_fat_Lasso_regression
The main purpose of this task is to understand that when applying a machine learning model to analysing a data set,
model hyper-parameters may impact the performance of the model and so it is very important to select these hyper-parameters.

The main objectives of using this data for clinical purposes could be summarized as follows:
1. Prediction: to predict the body fat using other measurements
2. Inference: to infer which measurements would impact body fat of men

3. We choose multiple linear regression models for our prediction and inference purposes. Although there are enormous number of regression models available, we choose to use Lasso regression. Remember Lasso regression is to optimize the following problem:
min∑𝑁𝑁 �𝑦𝑦−𝛽𝛽−∑𝑝𝑝 𝑥𝑥𝛽𝛽�2+𝜆𝜆∑𝑝𝑝 |𝛽𝛽|,
𝑖𝑖=1 𝑖𝑖 0 𝑖𝑖=1 𝑖𝑖𝑖𝑖 𝑖𝑖 𝑖𝑖=1 𝑖𝑖
where 𝜆𝜆 is a hyper-parameter for Lasso, and is called complexity parameter.
When using Lasso regression model, the complexity parameter 𝜆𝜆 would influence the performance greatly. Therefore, it is important to choose the best complexity parameter. In our experiments, we want to choose the best 𝜆𝜆 from 0.00, 0.01, 0.02, ⋯ ,0.98,0.99,1.0. Cross validation (CV) should be used for choosing 𝜆𝜆. 

