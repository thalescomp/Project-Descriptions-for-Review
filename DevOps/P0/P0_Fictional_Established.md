# [DevOps P0] Investigate a Product Workflow: Established Small Company

## About This Resource

DevOps is about building processes that enable your company to thrive. This involves paying attention to the specifics of the company's situation and culture. A startup, a small but established company, and a large corporation pose different challenges for a DevOps engineer looking to establish good processes.

For this project, we have provided one fictional example of each of these three types of companies. You are encouraged to choose whichever of these three examples is closest to your real-life experiences (from your current position or from previous jobs), or whichever you find most interesting. You will be asked to return to this example for later projects, so please consider your choice carefully. 

This example is of a small but established company. **This description does not provide all the information needed for answering the questions in the project**. You will need to add fictional details of your own to complete the project. If you have not worked in a dev or ops position before, you might find these resources helpful: 
* Talk with friends who currently work in IT Ops or software development, asking about the software development and deployment process
* Search the web to get a sense of typical [processes](https://www.google.com/#hl=en&q=IT%20development%20typical%20processes) and [problems](https://www.google.com/#hl=en&q=IT+development+typical+processes+problems) around the software development lifecycle, and use them in your narrative
* Use the [sample project submission](https://github.com/udacity/Project-Descriptions-for-Review/blob/9d7b8dd2c0d6d23fe5ecf768351b68184835a443/DevOps/P0/P0_Sample_Submission.md) as a guide. 

## Introduction to Twisted Threads

Welcome to our fictional company, Twisted Threads. Twisted Threads ships cotton T-shirts on demand. The founder started the company 10 years ago from her basement, but it has since expanded to over 200 employees. There is a warehouse, several physical stores, and an e-commerce site. Customers love the high-quality materials and custom designs.

That’s the good news. Now for the bad news. 

## Forecasting

* Twisted threads has a home-grown inventory system, separate for each physical shop and the warehouse. 
* The demand varies per season in both the quantity of T-shirts ordered and the type of items that customers want.
* Because of this, the company has supply and inventory issues. Sometimes the company runs out of stock and customer order fulfillment is delayed by a week or more. At other times, Twisted Threads has ordered way too many T-shirts from its supplier. They have had to throw out merchandise to make room for newer, more popular styles. 

## IT Infrastructure

* Twisted Threads hosted servers for their internet shop in-house, but there was massive flooding in the city and their servers were damaged beyond repair. They decided to move to the cloud. 
* Since making this decision, there have been major issues with performance and cost on the cloud. Customers complain about the website being buggy. The site has gone down several times during periods of high traffic, like the holiday season. 

## Product Development

* The product team wants more features but the rollout of new features is painfully slow. The competition just launched personalization on their site which was a huge hit with customers. Twisted Threads is falling behind because their website is outdated. 
* Developers are unhappy because deployment of new features takes ages, and operations does not give them new servers. Operations is too overwhelmed with running in the cloud in general, and worry about what will happen if the cloud datacenter has a long outage or loses their data.

[Project Description](P0_Project_Description.md)

[Project Submission Template](P0_Template.md)

[Sample Project Submission](P0_Sample_Submission.md)
