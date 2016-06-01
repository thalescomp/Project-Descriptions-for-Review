# Migrate an Application Server to the Cloud

This project has two parts: analytical and technical. 

* For the analytical portion, you will examine a scenario where certain services are to be migrated to the cloud, and make a recommendation about which cloud provider to use. 
* For the technical portion, you will write a Packer config file to create a virtual machine image for a server. We will provide the server specifications.

## Analytical Section Description

Our fictional companies are evaluating their cloud computing strategies. Each company is facing a different situation. Your goal in the analytical portion of the project is to analyze the situation in one of those companies, and make a recommendation about the cloud provider and platform to adopt. 

For this project you are encouraged, but not required, to use the same company that you picked for you P0 submission. As with that project, the scenarios may need to be augmented with details from your own experience, research, and imagination in order to complete the project. Here are the scenarios. 

### Ungeneric

As more companies sign up to be Ungeneric customers, the company is facing the challenge that its own database servers can no longer handle the load. It is very difficult to add servers quickly for the needed capacity. Instead of managing a rapidly growing server farm, it seems sensible to move to some cloud platform. 

The existing codebase for the application is largely in Ruby. Philosophically the team is more oriented toward open source tools (e.g., Linux over Windows) and prefers to be platform agnostic. 

From a usage perspective, the product is not CPU or RAM intensive. The main requirement is that the web front end be responsive and that database retrieval and updating happen quickly. One important consideration is that a multinational company wants Ungeneric's product to be available for employees in its China and Europe offices. 

### Twisted Threads 

Twisted Threads currently uses a small cloud services provider that has not proved very robust. Uptime is fine during ordinary usage, but unreliable at peak times when inventory is rapidly cycled out, such as during the holidays or during a change of season. 

The service is proving expensive, particularly since the application requirements are quite small: 500MB of RAM and 2TB of database storage. The thinking among the team is that moving to a different, better known cloud platform would be advantageous.

The codebase is largely in C++. Prior to moving to the current cloud services provider, the company hosted its own servers using Windows.The inventory systems, POS infrastructure for brick-and-mortar stores, and back office systems are still Windows-based. The developers are comfortable in a Windows environment and lean toward Azure. However, the company founder feels that Amazon would be a good choice as there is also the possibility of hosting a storefront on Amazon Marketplace. 

This is a source of some tension as the developers feel they might lose their jobs if Twisted Threads no longer maintains its own online storefront but uses the services provided by Amazon. The founder has tried to reassure them that their jobs are safe. Her argument is that with a reliable infrastructure, developers can focus on new growth initiatives for the company rather than be in firefighting mode all the time.

### ChalkFull

There is a push at ChalkFull to add a new feature: a way for teachers to build lesson plans quickly. The idea is that teachers can share lesson plans they have previously used on a website. Other teachers from across the country can view and comment on the lesson plans, and also revise them for their own use. In addition, ChalkFull will host supplementary materials in the form of images, videos, quizzes, links to external web resources, etc. that can be incorporated into the lesson plan. The expectation is that this feature will be available as an add-on to the existing product within the next quarter, and then marketed as a separate, stand-alone product within six months. 

Rather than add to its existing server farm, ChalkFull intends to use a cloud provider to host this product. The analysis on what provider to use has just begun. ChalkFull's existing codebase is in Python (back end) and JavaScript (front end), so the chosen provider must handle these languages well. It's also important that the site feels responsive even when several users try to access the same set of resources. For example, large videos should play smoothly and uninterruptedly when the user needs. The expectation also is that usage will spike about three weeks before the start of each school term. During the school year, a smaller spike on weekends is expected as teachers prepare their lessons for the upcoming week.

## Analytical Section Requirements

* Pick any one of the three fictional scenarios described above. You are encouraged, but not required, to choose the same company that you did for P0.
* Pick any 2 public cloud providers from among Amazon Web Services, Google Cloud Platform, or Microsoft Azure. 
  * Evaluate the organizational knowledge about these cloud platforms
  * Evaluate your server and application technical requirements
  * Evaluate how each cloud platform can fill these needs
  * Make a recommendation about which cloud platform to use, based on the evaluation

## Consideration for Analytic Section

In your analysis, please take the following into account:

* Does the organization already use services from these cloud platforms or related companies? For instance, MS SQL server would count for MS Azure, and Google Apps would count for Google Cloud Platform.
* If so, how much weight should be given to this familiarity? Is such preexistent expertise more or less important than the ease of providing of additional services? 
* What are the server and application requirements? Please specify CPU speed, RAM and disk size, network bandwidth and in/out traffic usage. Are there any specific regional requirements?
What types of VM would best serve the application needs on each of the cloud platforms? If there are several profiles (e.g. normal usage vs periodical high load), please consider the best VMs for all profiles, along with approximate time distribution for each (e.g., normal usage 300 days a year; high usage 53 days a year; holiday season).
* Given the above profiles, calculate the cost of running the application on each of the cloud platforms for a year, using current prices. Add links to the pricing pages. Since prices change, also specify the date when you retrieved a given pricing page. 

Your recommendation, about one paragraph long, should follow this analysis. Which cloud service should the team pick for this particular application migration, and why?

## Technical Section Requirements

Create a Packer configuration (that is, a Packer file and scripts to be run) that would create an image that has the requirements for a working SonarQube server (Java JRE/JDK and either MySQL or Postgres database) but not the server itself. See version requirements ![here](http://docs.sonarqube.org/display/SONAR/Requirements).


