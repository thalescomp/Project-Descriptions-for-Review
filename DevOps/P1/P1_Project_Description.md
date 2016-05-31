#Migrate an Application Server to the Cloud

##Description
Imagine that your company is looking into moving some of their applications to the cloud. But there are many cloud providers, and each company has different needs. Company has to gather information before going into the implementation phase. Your task in this project has two parts:
- Written
- pick a use case. You may choose either a real application or service from your work or the one of the example applications we have provided
- pick 2 public cloud providers from AWS, Google Cloud Platform, or Microsoft Azure. (You can evaluate all 3, or even something else that has public information, but there is no extra credit for additional platforms)
- evaluate your organizational knowledge about these cloud platforms
- evaluate your server and application technical requirements
- evaluate how each cloud platform can fill these needs
- make a recommendation about which cloud platform to use, based on the evaluation
-Technical
- write a Packer config that would create a VM image according to a specification for a server we have given
##Written part
###Organizational

Does your organization already use services from these cloud platforms or related companies? For instance, MS SQL server would count for MS Azure, and Google Apps would count for Google Cloud Platform.

Do you have people internally who have experience with these cloud platforms? If so, ask them and rate their internal knowledge 1 to 10.

What is the benefit to using familiar services and having people familiar with a platform in the decision for which platform to use? Is it more or less important than the number of additional services and costs? Would that depend on the application in question or apply to all your applications?

What is the current actual server hardware and the application requirements? Please specify CPU speed, RAM and disk size, network bandwidth and in/out traffic usage. Are these enough, too much or just right - can the server handle load at all times, is it over- or underutilized most or some of the time? Are there any special hardware related requirements, eg it needs GPU, because you are running calculations in CUDA? Do you have specific regional requirements, eg need to serve clients in China?

What are the types of VM that would best serve the application needs on each of the cloud platforms? If there are several profiles (e.g. normal usage vs periodical high load), please provide that for all profiles along with approximate time distribution in each of these profiles (e.g.  normal usage 300 days a year, high usage 53 days a year, holiday season).

Given the above profiles, calculate the cost of running the application on each of the cloud platforms for a year, using current prices (add date and links to price pages).
###Recommendation

After answering the questions about your organization and the technical requirements, what recommendation would you give to your team about which cloud service to pick for this particular application migration? Please explain why that is your recommendation! (Should be around a paragraph.)
##Technical Part
###Sonar Server

Create a Packer configuration (that is, a packer file and scripts to be run) that would create an image that has the requirements for a working SonarQube server (Java JRE/JDK and either MySQL or Postgres database) but not the server itself. See version requirements ![here](http://docs.sonarqube.org/display/SONAR/Requirements).
###Example Server: Twisted Threads
(If you didn’t choose the Twisted Threads example in Stage 0, we suggest you take a look at the example to understand the background for this example.) Twisted Threads wants to move their internal warehouse inventory web server to the cloud, so that all shops and warehouse can access it with ease. Currently it's run on a fairly old server: P4 with 4 GB RAM. It does not have any other special hardware requirements. Most of the time the server handles the load well, actually around 10-20% load and the application uses around 500 MB RAM. However, sometimes over a year (i.e. when the season changes, when the inventory gets changed a lot), there are problems with performance and the server slows down. What’s more, the physical switch it was connected to died one time and that impeded all work until it got replaced 3 days later; the sysadmin who had access to the physical location was on vacation and had to be recalled.  HQ does not want to fund a new and much more powerful server, because the performance problems happen for about 3-4 weeks (not continuous) in a year. But it affects all the people involved with inventory management and restocking.

