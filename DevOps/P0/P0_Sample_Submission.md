#[DevOps P0] Investigate a Product Workflow: Sample Submission

## Introduction

Use this sample submission as a guide as you create your own submission for the Improvement Plan project. The submission is based on a fictional company called ShoeBytes. The company has a total of six retail stores in three different cities, as well as an online store. The company has about 600 employees. The IT department is 80 people. The answers provided here are from the perspective of an engineer on the team that maintains the online storefront. This team of 12 people is part of the IT department. 

Your own submission should not replicate these answers about the ShoeBytes company. Rather, it should be based on your analysis of one of the fictional companies described later.

The goal of the project is to help you get into the mindset of a DevOps Engineer. To be successful, a DevOps engineer needs to have a good understanding of software development and deployment processes, the different stakeholders involved, and the common problems that might arise. From that perspective, **copying and pasting the answers from this sample submission, or making minor modifications to the wording of the sample answers while retaining their substance, is not sufficient to meet specifications for this project**. We encourage you to come up with answers in accordance with your own imagination, research, and experience. 


## Sample Submission

### What is the core function of your team? What is the core function of your company or organizational unit? Is the core function of your team well aligned with the function of the larger organizational unit or the company as a whole?

* Team goal: Provide an online shoe store for customers
* Organizational unit: Maintain web presence and IT infrastructure for company
* Company goal: sell customers shoes

Yes, the goals are in good alignment with each other.

### Who are your team's customers? Are they internal or external? What do they need?

* External customer: users of the online store. They need to be able to buy shoes.
* Internal customer: Accounting team. Need to receive daily totals of online purchase receipts.
* Internal customer: Warehouse team. Need to receive details of each transaction including exact shoe model, size, and color sold, and also shipping address so the shoes can be sent to the purchaser.
* Internal customer: Purchasing team needs summary report of shoe styles sold each week for forecasting and restocking purposes.

### What are all the internal teams or people that are involved in a product release, from start to finish? 

* Project manager
* Marketing
* Design 
* Developers (my team)
* Testers, QA
* Ops

### What is the current flow of software development and delivery in your team? List the main steps and whether they are manual or automated. 

* QA, Marketing, and other teams file issues in JIRA (manual)
* Feature requests, bug reports, etc. are checked every Monday and project manager determines priorities for the week (manual)
* Code gets written based on priorities (manual)
* Software gets checked into codebase (manual)
* Every Friday afternoon it gets deployed to a test server (manual) 
* QA team tests it and files bug reports or signs off as appropriate (manual) 
* Once a month codebase is sent to ops team for deployment into production (I don't know if it's automated or manual, but judging from ops usually staying late for the release days it's manual).

### How would you characterize communication within the organization? Do team members communicate well with each other? Is communication across teams smooth? How would you improve communication? 

* Does the company or team face any problems that would be avoided with better communication?
* Are both developers and operations involved when starting a new project? Do developers receive and act upon feedback from operations regarding how the software is performing?
* How do internal customers make their requirements known? Do they directly communicate with the developers?

We pretty much just talk within a team and with a manager and PM. The PM is responsible for gathering formal requirements and ensuring these are communicated to the team. I sometimes talk with other teams over lunch and usually find out a lot of interesting things that are even helpful at work. 

## Conclusion

That's it for the sample submission! Something like this would meet specifications for the project. However, the sample represents a typical effort, not the best. For instance, the sample does not provide any insight into steps that might be taken to remediate the problems in the software development lifecycle. The goal of the project is to get you started thinking like a DevOps Engineer, so the more concrete details you can give about problems and possible solutions, the better.

[Project Description](P0_Project_Description.md)

[Project Submission Template](P0_Template.md)

[Fictional Company Description](P0_Fictional_Company.md)