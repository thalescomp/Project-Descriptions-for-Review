# For Reviewer
## How Grading Works
We have created a document that gives rubric specific instructions to help you grade this project.You can access the document here: [Feed Reader Testing - Best Practices](https://docs.google.com/document/d/1cnNhclTpGAs0bpE9oJ5gDCgMmzniXvqX6k8zcKVJEhU/pub)

It is VERY IMPORTANT that you read this document before you begin evaluating projects. In order to meet specifications every review must follow the guidelines given in the document.

## Project Overview

![Project Roadmap](http://i.imgur.com/C3rq0yL.jpg)

In this project you are given a web-based application that reads RSS feeds. The original developer of this application clearly saw the value in testing, they've already included [Jasmine](http://jasmine.github.io/) and even started writing their first test suite! Unfortunately, they decided to move on to start their own company and we're now left with an application with an incomplete test suite. That's where you come in.

## Why this Project?

Testing is an important part of the development process and many organizations practice a standard of development known as "test-driven development". This is when developers write tests first, before they ever start developing their application. All the tests initially fail and then they start writing application code to make these tests pass.

Whether you work in an organization that uses test-driven development or in an organization that uses tests to make sure future feature development doesn't break existing features, it's an important skill to have!

## What will I learn?

You will learn how to use Jasmine to write a number of tests against a pre-existing application. These will test the underlying business logic of the application as well as the event handling and DOM manipulation.

## How will this help my career?

* Writing effective tests requires analyzing multiple aspects of an application including the HTML, CSS and JavaScript - an extremely important skill when changing teams or joining a new company.
* Good tests give you the ability to quickly analyze whether new code breaks an existing feature within your codebase, without having to manually test all of the functionality.

## Project Details
## How will I complete this project?

1. Take the JavaScript Testing [course](https://www.udacity.com/course/ud549)
2. Download the [required project assets](http://github.com/udacity/frontend-nanodegree-feedreader).
3. Review the functionality of the application within your browser.
4. Explore the application's HTML (*./index.html*), CSS (*./css/style.css*) and JavaScript (*./js/app.js*) to gain an understanding of how it works.
5. Explore the Jasmine spec file in *./jasmine/spec/feedreader.js* and review the [Jasmine documentation](http://jasmine.github.io).
6. Edit the allFeeds variable in *./js/app.js* to make the provided test fail and see how Jasmine visualizes this failure in your application.
7. Return the allFeeds variable to a passing state.
8. Write a test that loops through each feed in the allFeeds object and ensures it has a URL defined and that the URL is not empty.
9. Write a test that loops through each feed in the allFeeds object and ensures it has a name defined and that the name is not empty.
10. Write a new test suite named "The menu".
11. Write a test that ensures the menu element is hidden by default. You'll have to analyze the HTML and the CSS to determine how we're performing the hiding/showing of the menu element.
12. Write a test that ensures the menu changes visibility when the menu icon is clicked. This test should have two expectations: does the menu display when clicked and does it hide when clicked again.
13. Write a test suite named "Initial Entries".
14. Write a test that ensures when the loadFeed function is called and completes its work, there is at least a single .entry element within the .feed container.
15. Write a test suite named "New Feed Selection".
16. Write a test that ensures when a new feed is loaded by the loadFeed function that the content actually changes.
17. When complete - all of your tests should pass. 

## Useful Links
-[Udacity Front End Nanodegree JavaScript Style Guide](http://udacity.github.io/frontend-nanodegree-styleguide/javascript.html)

# Evaluation and Submission
## Evaluation
Your project will be evaluated by a Udacity reviewer according to the rubric below. Be sure to review it thoroughly before you submit. All criteria must "meet specifications" in order to pass. 
![rubric](http://i.imgur.com/79L92ou.png)

## Submission
1. If build tools are used, submit both your source and production code in the same repository in separate directories.  These directories are usually named ```src``` and ```dist``` respectively.
2. If build tools are used the gulp or grunt.js file as well as the package.json file must be included in the submission.
3. If build tools are used, the instructions for building the project and running the tool must be included in the README.md. You may find the short [Writing READMEs course](https://www.udacity.com/course/writing-readmes--ud777) helpful.
4. The node_modules directory may contain thousands of files and should not be contained in the submission. See the forum post [how to remove node_modules directory from Github repository](https://discussions.udacity.com/t/how-to-remove-node-modules-directory-from-github-respository/40929) for instructions.
5. The master branch is the default Github repository branch. If you wish to submit another branch, you'll need to set it as the [new default branch](https://help.github.com/articles/setting-the-default-branch/) inside your Github repository.
6. When you're ready to submit your project go back to your <a href="https://www.udacity.com/me" target="_blank">Udacity Home</a>, click on Project 6, and we'll walk you through the rest of the submission process. Due to the high volume of submissions we receive, please allow up up to **7 business days** for your evaluation to be returned.
7. If you are having any problems submitting your project or wish to check on the status of your submission, please email us at **frontend-project@udacity.com** or visit us in the <a href="http://discussions.udacity.com" target="_blank">discussion forums</a>.

## What's Next?
You will get an email as soon as your reviewer has feedback for you. In the meantime, review your next project and feel free to get started on it or the courses supporting it!
