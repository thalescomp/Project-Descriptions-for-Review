# Project 1: Model Evaluation and Validation
## Predicting Boston Housing Prices

## Project Description

The Boston housing market is highly competitive, and you want to be the best real estate agent in the area. To compete with your peers, you decide to leverage a few basic machine learning concepts to assist you and a client with finding the best selling price for their home. Luckily, you've come across the Boston Housing dataset which contains aggregated data on various features for houses in Greater Boston communities, including the median value of homes for each of those areas. Your task is to build an optimal model based on a statistical analysis with the tools available. This model will then used to estimate the best selling price for your client's home.
				
For this assignment, download the [machine learning projects](https://github.com/udacity/machine-learning) repo and navigate to the `boston_housing.ipynb` file in the *projects/boston_housing* folder. While some code has already been implemented to get you started, you will need to implement additional functionality to successfully answer all of the questions included in the notebook. You can find the included questions for reference below. Unless requested, do not modify code that has already been included.

## Software and Libraries
For this project, you will need to have the following software and Python libraries installed:

- Python 2.7
- NumPy
- scikit-learn
- iPython Notebook

## Deliverables
The following files should be included as your submission, and can be packaged as a single zip file for convenience:
- The `boston_housing.ipynb` file with fully implemented, functional code, with all code blocks executed and showing output.
- An HTML or PDF report of the project (you may either export the notebook as HTML with your answers included, or submit a separate PDF with only the questions and your answers).

## Project Report Questions
A description of the Boston Housing dataset can be found [here](https://archive.ics.uci.edu/ml/datasets/Housing). Use this slide as reference to the project questions you will encounter in the notebook. These questions (and your answers) must be present in your submitted report.

### Data Exploration
*This question is integrated into the project notebook output.*  
Using the NumPy library, calculate a few meaningful statistics about the dataset:

- How many data points (houses) were collected?
- How many features are present for each house?
- What is the minimum housing price? The maximum?
- What is the mean housing price? The median?
- What is the standard deviation of all housing prices?

1) Using your intuition, for each of the three features present in the dataset, do you think that an increase in the value of that feature would lead to an increase in the value of `'MDEV'` or a decrease in the value of `'MDEV'`? Justify your answer for each. 

### Developing a Model

2) For the hypothetical model presented in the project, would you consider this model to have successfully captured the variation of the target variable? Why or why not?

3) What is the benefit tosplitting a dataset into some ratio of training and testing subsets for a learning algorithm?

### Analyzing Model Performance

4) Choose one of the learning curves graphs presented in the project and state the maximum depth for the model. What happens to the score of the training curve as more training points are added? What about the testing curve? Would having more training points benefit the model?

5) When the model is trained with a maximum dpeth of 1, does the model suffer from high bias or from high variance? How about when the model is trained with a maximum depth of 10? What visual cues in the graph justify your conclusions?

6) Which maximum depth do you think results in a model that best generalizes to unseen data? What intuition lead you do this answer?

### Evaluating Model Performance
7) What is the grid search technique and how can it be applied to optimize a learning algorithm?

8) What is the k-fold cross-validation training technique and how is it performed on a learning algorithm?

9) What maximum depth does the optimal model that you have implemented have? How does this result compare to your guess in Question 6?

10) What price would you recommend each client sell his/her home at, given the data presented in the project? Do these prices seem reasonable given the values for the respective features?

11) In a few sentences, discuss whether the constructed model should or should not be used in a real-world setting.

## Evaluation
Your project will be reviewed by a Udacity reviewer against **<a href="https://review.udacity.com/#!/projects/5415419142/rubric" target="_blank"> this rubric</a>**. Be sure to review it thoroughly before you submit. All criteria must "meet specifications" in order to pass.

## Submission
When you're ready to submit your project go back to your <a href="https://www.udacity.com/me" target="_blank">Udacity Home</a>, click on Project 1, and we'll walk you through the rest of the submission process.

If you are having any problems submitting your project or wish to check on the status of your submission, please email us at **machine-support@udacity.com** or visit us in the <a href="http://discussions.udacity.com" target="_blank">discussion forums</a>.

## What's Next?
You will get an email as soon as your reviewer has feedback for you. In the meantime, review your next project and feel free to get started on it or the courses supporting it!
