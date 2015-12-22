# For Reviewers
## How Grading Works

We have created a document that gives rubric specific instructions to help you grade this project.You can access the document here: [Interactive Resume - Best Practices](https://docs.google.com/document/d/1VX76xeWFXIroBzUMyzOCAwMQy6vK56B_YpmWTL3lBk0/pub)

It is VERY IMPORTANT that you read this document before you begin evaluating projects. Every review must follow the guidelines in this document.

# Project Overview

![Project Roadmap](http://i.imgur.com/DQAgBen.jpg)

## Project Overview
In this project you will write the JavaScript that powers your own online resume. 

This project is meant to be completed while taking the [JavaScript Basics course](https://www.udacity.com/course/viewer#!/c-ud804-nd). Throughout the course you'll build your resume by writing a JS script that will combine your personal information with pre-written HTML and CSS templates to generate your resume.

##Note
If you have successfully completed the project for the JavaScript Basics course in the past (which entails having graduated from the course and having access to your course certificate), simply email us at frontend-project@udacity.com with your passing evaluation and we'll give you credit for this project.

## Why this Project?
Once you've mastered the skills of a front end web developer you'll want to make a great first impression. You need a resume that stands out.

The resume you build will not only help you build important skills, but will also make it easy to show employers why you’re perfect for the job. As you progress through this nanodegree you can update this resume with your new skills and projects.

## What will I Learn?
You will learn basic JavaScript syntax, which includes manipulating data types (like JSON), building loops and creating functions. At the same time, you’ll learn some simple jQuery DOM manipulation methods to build your resume the moment a user opens your website.

## How does this Help my Career?
* It's a resume. Resumes help you get jobs.
* JavaScript is **the** language of web development.
* JavaScript lets you turn static web pages into dynamic applications.
* Since it runs on normal web browsers, JavaScript is one of the most accessible and flexible programming languages.

# Project Details
## How do I complete this project?
1. If you need a refresher on JavaScript syntax, go to the [Javascript Basics course](https://www.udacity.com/course/viewer#!/c-ud804-nd); if you would like to understand how this project is manipulating and traversing the DOM, check out [Intro to jQuery](https://www.udacity.com/course/ud245-nd).
2. Go through the videos and assignments in this course to learn the JavaScript necessary to build your resume.
3. Read all the project details outlined below and make sure you understand each part. If you are unsure of anything please check with your cohort or private message your cohorts coaches.
4. Fork the project repo from **[Github](https://github.com/udacity/frontend-nanodegree-resume)** and begin building you resume. 
5. Review your work against the Project Rubric (on the next page).
6. When you are satisfied with your project, submit it according to the Submission Instructions on the next page.

### By the end:
Your resume will look something like this
![](http://i.imgur.com/pWU1Xbl.png)

And your repository will include the following files:

* **index.html**: The main HTML document. Contains links to all of the CSS and JS resources needed to render the resume, including resumeBuilder.js.
* **js/helper.js**: Contains helper code needed to format the resume and build the map. It also has a few function shells for additional functionality. More on helper.js further down.
* **js/resumeBuilder.js**: This file is empty. You should write your code here.
* **js/jQuery.js**: The jQuery library.
* **css/style.css**: Contains all of the CSS needed to style the page.
* **README.md**: 
The GitHub readme file.
* and some images in the images directory.

## Your starting point...
### js/helper.js
Within helper.js, you’ll find a large collection of strings containing snippets of HTML. Within many snippets, you’ll find placeholder data in the form of `%data%` or `%contact%`.

Each string has a title that describes how it should be used. For instance, `HTMLworkStart` should be the first `<div>` in the Work section of the resume. `HTMLschoolLocation` contains a `%data%` placeholder which should be replaced with the location of one of your schools.

### Your process:
The resume has four distinct sections: work, education, projects and a header with biographical information. You’ll need to:

1. Build four JSON objects, each one representing a different resume section. The objects that you create need to follow the schema below exactly. Property names are case-sensitive. Make sure your JSON objects are formatted correctly using JSONlint.com.

* `bio` contains:
        
            name : string
            role : string
            contacts : an object with
                  mobile: string
                  email: string 
                  github: string
                  twitter: string (optional)
                  location: string
            welcomeMessage: string 
            skills: array of strings
            biopic: url
            display: function

* `education` contains:
      
            schools: array of objects with
                 name: string
                 location: string
                 degree: string
                 majors: array of strings
                 dates: string (works with a hyphen between them)
                 url: string
            onlineCourses: array of objects with
                 title: string
                 school: string
                 date: string (works with a hyphen between them)
                 url: string
            display: function

* `work` contains
          
            jobs: array of objects with
                 employer: string 
                 title: string 
                 location: string 
                 dates: string (works with a hyphen between them)
                 description: string 
            display: function

* `projects` contains:

            projects: array of objects with
                  title: string 
                  dates: string (works with a hyphen between them)
                  description: string
                  images: array with string urls
                  display: function


2. Iterate through each JSON object and append its information to index.html in the correct section.
 * First off, you’ll be using jQuery’s `selector.append()` and `selector.prepend()` functions to modify index.html. `selector.append()` makes an element appear at the end of a selected section. `selector.prepend()` makes an element appear at the beginning of a selected section.
   * Pay close attention to the ids of the `<div>`s in index.html and the HTML snippets in helper.js. They’ll be very useful as jQuery selectors for `selector.append()` and `selector.prepend()`
* You’ll also be using the JavaScript method `string.replace(old, new)` to swap out all the placeholder text (e.g. `%data%`) for data from your resume JSON objects.
* Here’s an example of some code that would add the location of one your companies to the page:
   * `var formattedLocation = HTMLworkLocation.replace("%data%", work.jobs[job].location);`
   * `$(".work-entry:last").append(formattedLocation);`
 * Use the mockup at the bottom of this document as a guide for the order in which you should append elements to the page.
3. The resume includes an interactive map. Do the following to add it. 
 * In resumeBuilder.js, append the googleMap string to `<div id=”mapDiv”>`.
 * In index.html, uncomment the Google script element: `<script type="text/javascript" src="http://maps.googleapis.com/maps/api/js?libraries=places"></script>`
 * In helper.js, at the bottom of the file, uncomment code to initialize map and set fitBounds.
4. All of your code for adding elements to the resume should be within functions. And all of your functions should be encapsulated within the same objects containing your resume data. For instance, your functions for appending work experience elements to the page should be found within the same object containing data about your work experience.
5. Your resume should also `console.log()` information about click locations. On line 90 in helper.js, you’ll find a jQuery onclick handler that you’ll need to modify to work with the `logClicks(x,y)` function above it.
6. It’s possible to make additional information show up when you click on the pins in the map. Check out line 174 in helper.js and the Google Maps API to get started.

# Evaluation and Submission
## Evaluation
Your project will be evaluated by a Udacity reviewer according to the rubric below. Be sure to review it thoroughly before you submit. All criteria must "meet specifications" in order to pass.

## Online Resume Project Rubric

![](http://i.imgur.com/5dXwGrh.png)

## Submission
1. The master branch is the default Github repository branch. If you wish to submit another branch, you'll need to set it as the new default branch inside your Github repository.
2. When you're ready to submit your project go back to your <a href="https://www.udacity.com/me" target="_blank">Udacity Home</a>, click on Project 2, and we'll walk you through the rest of the submission process. Due to the high volume of submissions we receive, please allow up up to **7 business days** for your evaluation to be returned.
3. If you are having any problems submitting your project or wish to check on the status of your submission, please email us at **frontend-project@udacity.com** or visit us in the <a href="http://discussions.udacity.com" target="_blank">discussion forums</a>.

## What's Next?
You will get an email as soon as your reviewer has feedback for you. In the meantime, review your next project and feel free to get started on it or the courses supporting it!


## Useful Links
- [Udacity Front End Javascript Style Guide](https://udacity.github.io/frontend-nanodegree-styleguide/javascript.html)
