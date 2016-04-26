# [DevOps P0] Improvement Plan: Surajit Bose

## Organization Snapshot

#### Provide a brief description of your company and your team's role in it.

**April 25** 

Twisted Threads is a 10 year old company that ships cotton T-shirts on demand. The company has 200 employees. There is a warehouse, six brick and mortar stores, and one online store. 

#### What is the core function of your team? What is the core function of your company or organizational unit? Is the core function of your team well aligned with the function of the larger organizational unit or the company as a whole?

**April 25** 

* Core function of company: Sell T-shirts 
* Core function of team: Maintain e-commerce site for online sales

Yes, the two core functions are well aligned.

#### Who are your team's customers? Are they internal or external? What do they need?

**April 25** 

* External customer: users of the online store. They need to be able to view various T-shirt designs, place selected ones in a cart, and buy the items in the cart.
* Internal customer: Accounting team. Need to receive daily totals of online purchase receipts.
* Internal customer: Warehouse team. Need to receive details of each transaction including exact pattern, size, and color sold, and also shipping address so the shirts can be sent to the purchaser.
* Internal customer: Purchasing team needs summary report of shirt patterns sold each week for forecasting and restocking purposes.

#### What is the current flow of software development and delivery in your team? List the main steps and whether they are manual or automated. 

**April 25** 

All processes are manual. Each feature or bug fix takes up to two weeks to be deployed from the time development begins work on that feature or bug fix.
 
*Development cycle*

* On Monday morning, manager looks over bug reports, feature requests, etc. and determines priorities for the week 
* Code gets written over the week and checked into GitHub as completed.

*Testing and deployment cycle*

* On Monday morning the code written over the previous week is deployed to the test server.
* QA person tests throughout the week and files bug reports.
* On Friday morning the code that has passed tests is moved into production. 

#### What are all the teams or people that are involved in a product release, from start to finish? 

**April 25** 

* Dev team: 1 manager, 2 employees. Manager does coding too.
* QA and deployment team: It is actually the same team as IT Ops. They do all the tech support for the company as well as manage the cloud infrastructure. There is one dedicated QA person. Total of about seven people on that team.
* Marketing and Sales team. Not sure of the difference actually.
* Design team: Same team handles design for both website and shirts
* Warehouse team: Needs daily report of what to ship where.
* Customer service: Needs to be able to look up sales if a customer calls or emails with problems around an online order.

#### How is communication handled in your organization? 

**April 25** 

It is very informal. The manager has one weekly meeting with marketing and sales people and upper management. Otherwise the QA/ops people simply come to us. Even customer service people come to us if there is some problem with the site or something weird with the order. It is hard sometimes to tell whether the customer service people are reporting a bug or just don't understand how something works :-) but nowadays we try to send them to the IT team first, though it's not very clear to them what the difference between the IT and the Dev team is. Anyway there are lots of interruptions and informal conversations. 

## Quantitative Ratings

#### How satisfied are you with how other teams work and support the work that you do? (Scale: 1-10, 10 is best)

**April 25** 

Rating: 6. The people are nice but nothing is clearly communicated or prioritized. 

#### Do deployments go smoothly? (Scale: 1-10, 10 is best)

**April 25** 

Rating: 5. It varies. Sometimes everything works but at other times everything is cleared by QA but then the entire website crashes.

#### Do you have planned downtime for system upgrades or maintenance? 

**April 25** 

Every Monday at 7:30 AM for one hour the new code is deployed to production. The site is down during that hour. Sometimes it takes much longer, up to two hours. If there is a problem the system can be down for quite a while, even a full day or so. Just before Christmas we were down for a whole day. Ideally we would not have the site go down at all but work like Amazon or even our competitor NiceThreads, which doesn't appear to have any downtime at all. 

#### How much time does it take to set up the environment for a new project? 

**April 25** 

I don't understand what "set up the environment" means. The servers are in the cloud and don't need special setup to run our software. On our local machines we use Visual Studio and it doesn't take long to set up a new project on the machines. 

#### How often do you deploy to production? 

**April 25** 

Once a week (explained above)

#### How long does it take to deploy a new feature or bugfix from "code checked in to repository" to "feature is live to customers"? 

**April 25** 

Two weeks (explained above)

#### How easy is it to deploy a new feature or bugfix from "code checked in to repository" to "feature is live to customers"? (Scale: 1-10, 10 is best)

**April 25** 

Rating: 5. From our perspective once the code is checked in it's easy for us. Then it's the IT Ops team that has to handle it. Sometimes they get it right, sometimes they don't. Sometimes when they deploy the code on the test server it takes them several hours to get the new code properly integrated. 

#### How would you rate the quality of your software? (Scale: 1-10, 10 is best)

**April 25** 

Rating: 8. All three of us are really fast and efficient coders!

#### How easy it is to test your software? (Scale: 1-10, 10 is best)

**April 25** 

Rating: 5. 

Sometimes when the QA person deploys the code on the test server it takes several hours to get the new code properly integrated. And very often it still breaks something when deployed to production (maybe 3 out of every 10 deploys.)

#### How satisfied are your customers? (Scale: 1-10, 10 is best) 

**April 25** 

Rating: 8. They like the shirts and when the website works everything is great.