# Project 1: Model Evaluation and Validation
## Pedicting Boston Housing Prices

## Project Description

The Boston housing market is highly competitive, and you want to be the best real estate agent in the area. To compete with your peers, you decide to leverage a few basic machine learning concepts to assist you and a client with finding the best selling price for their home. Luckily, you?ve come across the Boston Housing dataset which contains aggregated data on various features for houses in Greater Boston communities, including the median value of homes for each of those areas. Your task is to build an optimal model based on a statistical analysis with the tools available. This model will then used to estimate the best selling price for your client?s home.
				
For this assignment, download the (machine learning projects)[https://github.com/udacity/machine-learning] repo and navigate to the `boston_housing.ipynb` file in the *Predicting Boston Housing Prices* folder. While some code has already been implemented to get you started, you will need to implement additional functionality to successfully answer all of the questions included in the notebook. You can find the included questions for reference below. Unless requested, do not modify code that has already been included.

## Software and Libraries
For this project, you will need to have the following software and Python libraries installed:

- Python 2.7
- NumPy
- scikit-learn
- iPython Notebook

## Deliverables
The following files should be included as your submission, and can be packaged as a single zip file for convenience:
- The `boston_housing.ipynb` file with fully implemented, functional code, with all code blocks executed and showing output.
- A PDF report of the project (you may either save the notebook as a PDF with your answers, or submit a separate document with only the questions and your answers).

## Project Report Questions
A description of the Boston Housing dataset can be found (here)[https://archive.ics.uci.edu/ml/datasets/Housing]. Use this section as reference to the project questions you will encounter in the notebook. These questions (and your answers) must be present in your included PDF report.

### Statistical Analysis and Data Exploration
*This question is integrated into the project notebook output.*  
Using the NumPy library, calculate a few meaningful statistics about the dataset:

- How many data points (houses) were collected?
- How many features are present for each house?
- What is the minimum housing price? The maximum?
- What is the mean housing price? The median?
- What is the standard deviation of all housing prices?

1) Of the available features for a given home, choose three you feel are significant and give a brief description for each of what they measure. 

2) Using your client's feature set `CLIENT_FEATURES` in the template code, which values correspond to the chosen features?

### Evaluating Model Performance
3) Why do we split the data into training and testing subsets? 

4) Which performance metric below is most appropriate for predicting housing prices and analyzing error? Why?

- Accuracy
- Precision
- Recall
- F1 score
- Mean Squared Error (MSE)
- Mean Absolute Error (MAE)

5) What is the grid search algorithm and when is it applicable?

6) What is cross-validation and how is it performed on a model? Why would cross-validation be helpful when using grid search?

### Analyzing Model Performance
7) Choose one of the learning curve graphs your code creates. What is the max depth for the model? As the size of the training set increases, what happens to the training error? Describe what happens to the testing error.

8) Look at the learning curve graphs for the model with a max depth of 1 and a max depth of 10. When the model is using the full training set, does it suffer from high bias or high variance when the max depth is 1? What about when the max depth is 10?

9) From the model complexity graph, describe the training and testing errors as the max depth increases. Based on your interpretation of the graph, which max depth results in a model that best generalizes the dataset? Why?

### Model Prediction
*To answer the following questions, it is recommended that you run your notebook several times and use the median or mean value as your result.*

10) Using grid search, what is the optimal max depth for your model? How does this result compare to your initial intuition?

11) With your parameter-tuned model, what is the best selling price for your client?s home? How does this selling price compare to the statistics you calculated on the dataset? 

12) In a few sentences, discuss whether you would use this model or not to predict the selling price of future clients? homes in the Boston area.

## Evaluation
Your project will be reviewed by a Udacity reviewer against **<a href="https://docs.google.com/document/d/1b3u3HV2xMBAH7SQxdMPzr2QUaBJU8oeiCNdNh3AWLVY/pub?embedded=true" target="_blank"> this rubric</a>**. Be sure to review it thoroughly before you submit. All criteria must "meet specifications" in order to pass.

## Submission
When you're ready to submit your project go back to your <a href="https://www.udacity.com/me" target="_blank">Udacity Home</a>, click on Project 1, and we'll walk you through the rest of the submission process.

If you are having any problems submitting your project or wish to check on the status of your submission, please email us at **machine-support@udacity.com** or visit us in the <a href="http://discussions.udacity.com" target="_blank">discussion forums</a>.

## What's Next?
You will get an email as soon as your reviewer has feedback for you. In the meantime, review your next project and feel free to get started on it or the courses supporting it!
