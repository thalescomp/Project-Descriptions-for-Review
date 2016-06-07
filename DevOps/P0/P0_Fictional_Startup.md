# [DevOps P0] Investigate a Product Workflow: Startup

## About This Resource

DevOps is about building processes that enable your company to thrive. This involves paying attention to the specifics of the company's situation and culture. A startup, a small but established company, and a large corporation pose different challenges for a DevOps engineer looking to establish good processes.

For this project, we have provided one fictional example of each of these three types of companies. You are encouraged to choose whichever of these three examples is closest to your real-life experiences (from your current position or from previous jobs), or whichever you find most interesting. You will be asked to return to this example for later projects, so please consider your choice carefully. 

This example is of a small startup. **This description does not provide all the information needed for answering the questions in the project**. You will need to add fictional details of your own to complete the project. If you have not worked in a dev or ops position before, you might find these resources helpful for completing the project: 

* Talk with friends who currently work in IT Ops or software development, asking about the software development and deployment process. What works well? What is difficult? 
* Search the web to get a sense of typical [processes](https://www.google.com/#hl=en&q=IT%20development%20typical%20processes) and [problems](https://www.google.com/#hl=en&q=IT+development+typical+processes+problems) around the software development lifecycle, and use them in your narrative.
* Take a look at the [sample project submission](P0_Sample_Submission.md) that has been provided as a guide. The sample submission uses a different fictional company from the ones provided for your use. 

## Introduction to Ungeneric

Ungeneric is a small software startup developing a SaaS (Software as a Service) solution for gamification. Ungeneric began as a game development company, with an emphasis on games that help the user maintain a physical workout regimen. After a couple of pivots, it has successfully found a good market fit working with companies on gamifying their wellness initiatives. Companies who are Ungeneric customers can use the product to:

* Set up and run interdepartmental challenges to see how many employees sign up for lunchtime yoga, or join the bike-to-work program, etc. 
* Offer small rewards such as gift cards for individual employees who complete certain milestones: exercising at the company gym regularly, having an ergonomic assessment of their workstations, etc. 
* Compete against other Ungeneric customer companies to see which company succeeds at a defined measure, e.g., total number of miles run by all employees during a particular week.

Ungeneric remains a small team. The company has fewer than 50 employees. The entire development team of seven people is responsible for all front- and back-end code and infrastructure. This includes the company website that provides information about the Ungeneric platform, as well as the websites where employees of customer companies track their wellness goals and initiatives, both as individuals and as administrators.

## Challenges

This new success has brought new challenges: 

* More customers means an increased load on servers
* The need to maintain existing SLA (service level agreements) regarding uptime and availability
* The desire to be responsive to customer requests for additional functionality and features
* The pressure to provide Android and iOS clients for individual employees instead of only a web-based client
* One large customer is a multinational company. Ungeneric's offerings are available only to US employees, and there is a proposal to make them available to employees worldwide. 

Meeting these challenges successfully is critical to the company's future. The team generally is well focused on them, but there are occasional problems. For example, when the head of Marketing mentioned that end-users were eager for a way to access the site on mobile devices, one of the engineers spent two days trying to make the website mobile friendly. During the weekly team meeting, this led to a spirited debate:

* Is providing smoother mobile access more important than some other bug fixes, for example, ensuring that end users who have left their companies can no longer log into the site?
* Is it worthwhile to spend effort on making the site mobile friendly, or is this a waste of time when the goal is to have iOS and Android apps? 

There were strong arguments and some hurt feelings as a result of this incident.

## Your Role and Perspective

The small developer team sees the urgent need to scale its offerings while maintaining reliability and speed. The CEO of the company, formerly the lead developer but now more involved with growing the client base, has asked you to focus on scaling up, reliability, and speed. You need to:

* Implement automated deployment
* Ensure a robust and stable production environment
* Identify, track, and handle bugs, outages, and other issues quickly. 

You know the development side well and are confident in your ability to code new features. But you are new to operations processes and challenges. You ended up being the one to deal with these aspects because the CEO trusts you.

[Project Description](P0_Project_Description.md)

[Project Submission Template](P0_Template.md)

[Sample Project Submission](P0_Sample_Submission.md)
