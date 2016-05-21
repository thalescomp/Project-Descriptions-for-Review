# Project 2: Supervised Learning
## Building a Student Intervention System

## Project Description

As education has grown to rely more on technology, vast amounts of data has become available for examination and prediction. Logs of student activities, grades, interactions with teachers and fellow students, and more, are now captured in real time through learning management systems like **Canvas** and **Edmodo**. This is especially true for online classrooms, which are becoming popular even at the primary and secondary school level. Within all levels of education, there exists a push to help increase the likelihood of student success, without watering down the education or engaging in behaviors that fail to improve the underlying issues. Graduation rates are often the criteria of choice, and educators seek new ways to predict the success and failure of students early enough to stage effective interventions.

A local school district has a goal to reach a 95% graduation rate by the end of the decade by identifying students who need intervention before they drop out of school. As a software engineer contacted by the school district, your task is to model the factors that predict how likely a student is to pass their high school final exam, by constructing an intervention system that leverages supervised learning techniques. The board of supervisors has asked that you find the most effective model that uses the least amount of computation costs to save on the budget. You will need to analyze the dataset on students' performance and develop a model that will predict the likelihood that a given student will pass, quantifying whether an intervention is necessary.

Navigate to [Udacity's Machine Learning GitHub project repo](https://github.com/udacity/machine-learning/tree/master/projects), and download the projects for this Nanodegree. Once downloaded, unzip the archive and navigate to the `student-intervention` folder for the project files and refer to the `README.md` file for further instructions for opening the project notebook file `student_intervention.ipynb`. While some code has already been implemented to get you started, you will need to implement additional functionality to successfully answer all of the questions included in the notebook. You can find the included questions for reference below.

## Software and Libraries
 For this project, you will need to have the following software installed:
 
- [Python 2.7](https://www.python.org/download/releases/2.7/)
- [NumPy](http://www.numpy.org/)
- [pandas](http://pandas.pydata.org/)
- [scikit-learn](http://scikit-learn.org/stable/)
- [iPython Notebook](http://ipython.org/notebook.html)

## Deliverables

The following files should be included as your submission, and can be packaged as a single zip file for convenience:
- The `student_intervention.ipynb` file with fully implemented, functional code, with all code blocks executed and showing output.
- An HTML or PDF report of the project (you may either export the notebook as HTML with your answers included, or submit a separate PDF with only the questions and your answers).

## Questions and Report Structure

**Your model will be evaluated on three factors:**

- Its <a href="https://en.wikipedia.org/wiki/F1_score">F1 score</a>, summarizing the number of correct positives and correct negatives out of all possible cases. In other words, how well does the model differentiate likely passes from failures?
- The size of the training set, preferring smaller training sets over larger ones. That is, how much data does the model need to make a reasonable prediction?
- The computation resources to make a reliable prediction. How much time and memory is required to correctly identify students that need intervention?

### 1. Classification vs Regression

Your goal is to identify students who might need early intervention - which type of supervised machine learning problem is this, classification or regression? Why?

### 2. Exploring the Data
Can you find out the following facts about the dataset?
Total number of students
Number of students who passed
Number of students who failed
Graduation rate of the class (%age)
Number of features
Use the code block provided in the template to compute these values.

### 3. Preparing the Data
Execute the following steps to prepare the data for modeling, training and testing:
Identify feature and target columns
Preprocess feature columns
Split data into training and test sets
Starter code snippets for these steps have been provided in the template.

### 4. Training and Evaluating Models
Choose 3 supervised learning models that are available in scikit-learn, and appropriate for this problem. For each model:
What is both the theoretical space complexity to represent the model and the time for the algorithm to make a prediction? You can either provide the big-O notation, or list several the of major features that may affect the algorithm and state if the largest driving factor is constant, linear, logrithmic, polynomical, etc in nature.
What are the general applications of this model? What are its strengths and weaknesses?
Given what you know about the data so far, why did you choose this model to apply?
Fit this model to the training data, try to predict labels (for both training and test sets), and measure the F1 score. Repeat this process with different training set sizes (100, 200, 300), keeping test set constant.
Produce a <a href="https://docs.google.com/document/d/1Goxw-6M0umOCokCFqTr-g7SU_5f6MIm_wqXmh9Cnjhw/pub" target="_blank">table</a> showing training time, prediction time, F1 score on training set and F1 score on test set, for each training set size.<br>
**Note**: You need to produce 3 such tables - one for each model.

### 5. Choosing the Best Model
Based on the experiments you performed earlier, in 1-2 paragraphs explain to the board of supervisors what single model you chose as the best model. Which model is generally the most appropriate based on the available data, limited resources, cost, and performance?
In 1-2 paragraphs explain to the board of supervisors in layman’s terms how the final model chosen is supposed to work (for example if you chose a decision tree or support vector machine, how does it make a prediction).
Fine-tune the model. Use gridsearch with at least one important parameter tuned and with at least 3 settings. Use the entire training set for this.
What is the model’s final F1 score?

### Evaluation

Your project will be reviewed by a Udacity reviewer against **<a href="https://review.udacity.com/#!/projects/5446988865/rubric" target="_blank"> this rubric</a>**. Be sure to review it thoroughly before you submit. All criteria must "meet specifications" in order to pass.

### Submission
When you're ready to submit your project go back to your <a href="https://www.udacity.com/me" target="_blank">Udacity Home</a>, click on Project 2, and we'll walk you through the rest of the submission process.

If you are having any problems submitting your project or wish to check on the status of your submission, please email us at **machine-support@udacity.com** or visit us in the <a href="http://discussions.udacity.com" target="_blank">discussion forums</a>.

### What's Next?
You will get an email as soon as your reviewer has feedback for you. In the meantime, review your next project and feel free to get started on it or the courses supporting it!
