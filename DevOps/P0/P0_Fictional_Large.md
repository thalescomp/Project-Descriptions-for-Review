# [DevOps P0] Investigate a Product Workflow: Large Company

## About This Resource

DevOps is about building processes that enable your company to thrive. This involves paying attention to the specifics of the company's situation and culture. A startup, a small but established company, and a large corporation pose different challenges for a DevOps engineer looking to establish good processes.

For this project, we have provided one fictional example of each of these three types of companies. You are encouraged to choose whichever of these three examples is closest to your real-life experiences (from your current position or from previous jobs), or whichever you find most interesting. You will be asked to return to this example for later projects, so please consider your choice carefully. 

This example is of a large, public company. **This description does not provide all the information needed for answering the questions in the project**. You will need to add fictional details of your own to complete the project. If you have not worked in a dev or ops position before, you might find these resources helpful for completing the project: 

* Talk with friends who currently work in IT Ops or software development, asking about the software development and deployment process. What works well? What is difficult? 
* Search the web to get a sense of typical [processes](https://www.google.com/#hl=en&q=IT%20development%20typical%20processes) and [problems](https://www.google.com/#hl=en&q=IT+development+typical+processes+problems) around the software development lifecycle, and use them in your narrative.
* Take a look at the [sample project submission](P0_Sample_Submission.md) that has been provided as a guide. The sample submission uses a different fictional company from the ones provided for your use. 

## Introduction to ChalkFull

ChalkFull is a well established educational technology company. The company's flagship product is an end-to-end student management solution for elementary and secondary schools:

* For teachers, ChalkFull provides a way to maintain the student roster, including test scores, attendance records, etc. 
* For students, ChalkFull allows them to keep track of all their assignments, look up their grades, and plan their classes each term. 
* For administrators, ChalkFull maintains student records, including parent/guardian information; health or medical condition information including learning disabilities; academic progress, etc. 

The software runs on servers to which users connect via a web browser. 

The market leader in this sector has 30% of the market share. By comparison, ChalkFull has around 12%. So ChalkFull is a respectable and recognized name but not the most prominent one in the field. The company is aggressively trying to enhance profitability by increasing market share and cutting costs.

ChalkFull is more than 25 years old. Today, the company has around 4,000 employees. About 600 of those are in technical roles distributed across several teams. Some of these teams are:

* Developers who work on new features
* An Operations team that maintains the servers (front and back end) on which the app runs
* A team that maintains legacy infrastructure
* A QA team that is also responsible for ensuring regulatory compliance
* Technical support for customers who use the software
* A team that maintains the public facing website
* Internal help desk for employees, etc.

Some of these teams follow agile practices, but there are also teams in which processes are entrenched and seem bogged down with red tape. The newly hired VP of Engineering has expressed her desire to have the entire company be nimble. However, there is not much of a company culture around DevOps yet. The knowledge and culture around good DevOps practices needs to be built. 

## Challenges

There are many competing pressures and constraints on the product.

* The desire to increase the customer base, which makes adding new features a priority. Sometimes the Sales team promises features to potential customers by a very short time frame that Development is not comfortable with. An example of such a feature is the ability to import grades directly from quizzes administered via [Moodle](https://moodle.org/) or other online learning management systems. This feature had to be implemented very rapidly and was pushed out without proper testing or QA, and customers were unhappy with the resulting bugs.
* The need to maintain legacy systems, e.g., a way to read information off [Scantron](http://www.scantron.com/) forms to populate new student data or to calculate test scores.
* The difficulty in getting the budget for new positions approved, given the desire to hold costs down.
* Compliance with regulations, as there are strict laws governing student record privacy and the privacy of minors. For example, ChalkFull employees cannot deal directly with a school's data set; it has to be anonymized before the employees can look at it, and ChalkFull is responsible for providing the mechanisms to anonymize the data
* A disparate customer base, with some schools preferring to run the software on servers located at the school site, and others wanting ChalkFull to host the servers. 

## Your Role and Perspective

You can choose **either** the developer perspective **or** the operations perspective as your own. Both perspectives are provided here, but you must choose just one of the two for this and subsequent projects. 

### Developer Perspective

You are a developer on the agile team that is responsible for the flagship product. Any new releases or features your team works on have to integrate with legacy apps such as the Scantron reading infrastructure. Your team is interested in following good practices, such as using Continuous Integration and writing automated tests. You also want to work together with Operations to define non-functional requirements, e.g., ensuring that the product does not require too much memory to run or that monitoring can be accomplished easily. However, the pressure from project managers and product owners to deliver more features quickly detracts from the focus on long-term quality and maintainability.

### Operations Perspective

You are a member of the Operations team that supports the infrastructure for the hosted application (i.e., for when schools want ChalkFull to run the app on its own servers instead of at the school site). You also support the infrastructure for schools that run the application on their own site to upgrade the software when bug fixes or new releases occur. Historically, your team is frustrated that the developer team often requires you to push out a new feature too quickly, which compromises testing and getting a signoff from QA. When such rollouts go well, Operations does not get recognition for its work; your team is visible only when something does not work. Things seem to be getting better, at least in terms of rhetoric, as the VP of Engineering has made efforts to include your team's input on requirements and to ensure that your team is notified about upcoming projects earlier. However, some of your team members are worried about her desire to implement a culture of DevOps; if developers will be responsible for operations functions as well, will the Ops team no longer be needed? 


[Project Description](P0_Project_Description.md)

[Project Submission Template](P0_Template.md)

[Sample Project Submission](P0_Sample_Submission.md)
