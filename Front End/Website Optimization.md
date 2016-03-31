##[Project Rubric](https://review.udacity.com/#!/projects/2735848561/rubric)


# For Reviewer
## How Grading Works
We have created a document that gives rubric specific instructions to help you grade this project.You can access the document here: [Website Performance Optimization - Best Practices](https://docs.google.com/document/d/1-Ir6Io9wzmULKn9ldaeFohB0aMMvCWybXdbQWNHLUUs/pub)

It is VERY IMPORTANT that you read this document before you begin evaluating projects. In order to meet specifications every review must follow the guidelines given in the document.

#Project Overview

![Project Roadmap](http://i.imgur.com/AHvCOx3.jpg)

##Project Overview
You will optimize a provided website with a number of optimization- and performance-related issues so that it achieves a target PageSpeed score and runs at 60 frames per second.

##Note
If you have successfully completed the project for the Website Performance Optimization course in the past (which entails having graduated from the course and having access to your course certificate), simply email us at frontend-project@udacity.com with your passing evaluation and we'll give you credit for this project.

## Why this project?
As web applications become increasingly interactive and accessed on a variety of devices there are a variety of opportunities in which performance issues can hinder the user experience. This project presents a number of those performance issues and provides an opportunity to showcase your skills in identifying and optimizing web applications.

## What will I learn?
You will learn about the critical rendering path, the process by which the browser receives HTML, CSS and JavaScript and the required processing to turn them into rendered pixels. You’ll also start to think of your work as a continuously running web application that requires a consistent framerate to produce the most enjoyable user experience.

## How will this help my Career?
* As the number of devices users can access an application from continues to grow, ensuring a quality user experience across those devices is important.
* Understanding lower-level concepts regarding how the browser works and interprets your code enables you to produce highly performant applications.


#Project Details
## How will I complete this project?
1. Review our course on [Website Performance Optimization](https://www.udacity.com/course/viewer#!/c-ud884-nd) using Google PageSpeed.
1. Download the <a href="https://github.com/udacity/frontend-nanodegree-mobile-portfolio" target="_blank">required project assets</a>.
2. Use Chrome Developer Tools to review the current state of various pages within the application and identify areas for improvement.
3. Review the code powering the website and identify areas where you believe modifications are warranted.
4. Iteratively make changes and test those changes using the tools available to you to determine if they are a performance gain or loss.
5. The PageSpeed score of 90 is for index.html (both Mobile and Desktop scores should be at least 90). 
6. The frame rate of 60fps should be obtained for the pizza.html page (views/pizza.html). The file you need to study and change is views/js/main.js.
7. Comments should be added to main.js to indicate the optimizations implemented in the pizza.html page.
8. Please do not forget to update the README file and make sure you outline all of your optimizations done in main.js for the pizza.html page.
9. It's recommended to not measure performance in a virtualized environment. We recommend you measure the FPS performance of pizza.html in your native operating system using Chrome Developer Tools.
10. Here is a picture of what the [target timeline](http://i.imgur.com/cI6zwUo.jpg) may look like. Evaluators will focus their attention on the timeline rather than the FPS meter due to varying hardware factors that may affect FPS.

##Useful Links
- [Effective Optimizations for 60FPS](https://github.com/udacity/fend-office-hours/tree/master/Web%20Optimization/Effective%20Optimizations%20for%2060%20FPS)
- [Writing READMEs](https://www.udacity.com/course/writing-readmes--ud777)

#Evaluation and Submission
## Evaluation
Your project will be evaluated by a Udacity reviewer according to the rubric below. Be sure to review it thoroughly before you submit. All criteria must "meet specifications" in order to pass. 

#[Project Rubric](https://review.udacity.com/#!/projects/2735848561/rubric)

## Submission
1. Submit both your source and production code in the same repository in separate directories.  These directories are usually named ```src``` and ```dist``` respectively.
2. If build tools are used the gulp or grunt.js file as well as the package.json file must be included in the submission.
3. If build tools are used, the instructions for building the project and running the tool must be included in the README.md. You may find the short [Writing READMEs course](https://www.udacity.com/course/writing-readmes--ud777) helpful.
4. The node_modules directory may contain thousands of files and should not be contained in the submission. See the forum post [how to remove node_modules directory from Github repository](https://discussions.udacity.com/t/how-to-remove-node-modules-directory-from-github-respository/40929) for instructions.
5. The master branch is the default Github repository branch. If you wish to submit another branch, you'll need to set it as the [new default branch](https://help.github.com/articles/setting-the-default-branch/) inside your Github repository.
6. When you're ready to submit your project go back to your <a href="https://www.udacity.com/me" target="_blank">Udacity Home</a>, click on Project 4, and we'll walk you through the rest of the submission process. Due to the high volume of submissions we receive, please allow up up to **7 business days** for your evaluation to be returned.
7. If you are having any problems submitting your project or wish to check on the status of your submission, please email us at **frontend-project@udacity.com** or visit us in the <a href="http://discussions.udacity.com" target="_blank">discussion forums</a>.

## What's Next?
You will get an email as soon as your reviewer has feedback for you. In the meantime, review your next project and feel free to get started on it or the courses supporting it!
