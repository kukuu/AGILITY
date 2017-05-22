

# Benefits of AGILE

#### 1. Revenue

The iterative nature of agile development means features are delivered incrementally, enabling some benefits to be realised early as the product continues to develop.


#### 2. Speed-to-market

Research suggests about 80% of all market leaders were first to market. As well as the higher revenue from incremental delivery, agile development philosophy also supports the notion of early and regular releases, and ‘perpetual beta’.


#### 3. Quality

A key principle of agile development is that testing is integrated throughout the cycle, enabling regular inspection of the working product as it develops. This allows the product owner to make adjustments if necessary and gives the product team early sight of any quality issues.


#### 4. Visibility

Agile development principles encourage active user involvement throughout the product’s development and a very cooperative collaborative approach. This provides excellent visibility  for key stakeholders, both of the project’s progress and of the product itself, which in turn helps to ensure that expectations are effectively managed.


#### 5. Risk Management

Small incremental releases made visible to the product owner and product team through its development help to identify any issues early and make it easier to respond to change. The clear visibility in agile development helps to ensure that any necessary decisions can be taken at the earliest possible opportunity, while there’s still time to make a material difference to the outcome.


#### 6. Flexibility / Agility

In traditional development projects, we write a big spec up-front and then tell business owners how expensive it is to change anything, particularly as the project goes on. In fear of scope creep and a never-ending project, we resist changes and put people through a change control committee to keep them to the essential minimum. Agile development principles are different. In agile development, change is accepted. In fact, it’s expected. Because the one thing that’s certain in life is change. Instead the timescale is fixed and requirements emerge and evolve as the product is developed. Of course for this to work, it’s imperative to have an actively involved  stakeholder who understands this concept and makes the necessary trade-off decisions, trading existing scope for new.


#### 7. Cost Control

The above approach of fixed timescales and evolving requirements enables a fixed budget. The scope of the product and its features are variable, rather than the cost.


#### 8. Business Engagement/Customer Satisfaction
 
The active involvement of a user representative and/or product owner, the high visibility  of the product and progress, and the flexibility to change when change is needed, create much better business engagement and customer satisfaction. This is an important benefit that can create much more positive and enduring working relationships.


#### 9. Right Product

Above all other points, the ability for agile development requirements to emerge and evolve, and the ability to embrace change (with the appropriate trade-offs), the team build the right product. It’s all too common in more traditional projects to deliver a “successful” project in IT terms and find that the product is not what was expected, needed or hoped for. In agile development, the emphasis is absolutely on building the right product.


#### 10. More Enjoyable!

The active involvement, cooperation and collaboration make agile development teams a much more enjoyable place for most people. Instead of big specs, we discuss requirements in workshops. Instead of lengthy status reports, we collaborate around a task-board discussing progress. Instead of long project plans and change management committees, we discuss what’s right for the product and project and the team is empowered to make decisions. In my experience this makes it a much more rewarding approach for everyone. In turn this helps to create highly motivated, high performance teams that are highly co-operative.


# Continuous Delivery

 CD is the ability to get changes of all types—including new features, configuration changes, bug fixes and experiments—into production, or into the hands of users, safely and quickly in a sustainable way.

The ultimate goal of continuous delivery is to minimise the iteration time of the code-test-deliver-measure experimentation cycle. Increasing deliverable throughput in this way is the key to not only more feature work being delivered but higher quality code as well. This might seem counter-intuitive at first but code is fixed and polished through that same cycle and less time spent on deployment is more time spent on designing quality code.

The high-level requirements FOR CD are:

	1.	Software must be easily testable, which means it must be loosely coupled.

	2.	Delivery must—under normal circumstances—require minimal human interaction.

	3.	Delivery—from commit to production—must be fast. Preferably under 10 minutes.

	4.	Rolling back a deployed feature if it is found to be broken or unwanted must be trivial.

The most optimum path to achieve these goals is to use  microservices architecture


# Micro-services

Microservices enforce loose coupling, plus it’s easier to develop fast and reliable deployment pipelines if they only have to handle small packages.

However, note microservices introduced a new problem: if adding a feature was often going to require adding a new, independently deployed and hosted service then that process had to be fast and not require any specialist knowledge. 

Demanding that every single developer in the company learn the intricacies of maintaining Puppet configuration for all their services would have been impractical and more than a little cruel.

Resolution:

	1.	Set up feature teams  that can possibly set up a new service in under four hours. What this means
		is Developing services should not   require knowledge of the infrastructure and changing 
		infrastructure should not require detailed knowledge of the services running on it. 
		If we need to change the hostname or port a service runs on it should require no changes
		to the service itself.

	2.	All project configuration—from build process to health monitoring—must be contained within the 
		project repository. Anything else introduces hidden dependencies for deployment that threaten
		to break the pipeline and require specialist knowledge to debug.

	3.	The above configuration should be declarative and not require adding dependencies to the project.

	4.  Use Containerisation


# Containerisation

Source code of any  program cannot fully describe the function of that program without the context it will be compiled and run in. Most unexpected behaviour during deployment comes from build environments being different than expected. To make deployment repeatable, we need to make a program’s context repeatable. That’s where Docker comes in.

Docker essentially allows you to specify a “source code” for a program’s context that can then be “compiled” to an image and run as a container. This means that once we have tested an image we can have high confidence that it will perform equally well in every environment it is deployed to.

Additionally, Docker allows you to specify deploy configurations made up of multiple containers all linked in a private network and DNS that allows services that depend strongly on each other to be deployed and scaled together. 

To be fully context-agnostic, deployment should be able to happen to any host on the network on whatever port the host happens to have free. This presents a challenge: how do services link up when their network locations are fluid? You need a reverse proxy (like nginx) and a way to keep its configuration up to date in a changing service landscape.
You will need a  Consul to store and  manage service states.


#### What a deployment looks like:

	1.	Build Docker image.

	2.	Test that image in isolation.

	3.	Push that image to the in-house image registry.

	4.	Pull all images you need to deploy linked.

	5.	Deploy them to a test environment.

	6.	Run automated tests against the container system.

	7.	Upload service configuration to Consul API (if changed).

	8.	Deploy the containers to all hosts, tagged with the offline colour.

	9.	Wait until they are all responding and passing automated checks.

	10.	Flip environment alias to point at the offline colour.

	11.	The new build is now online.


#### Ultimate development/production workflow. How to get changes from your local machine into production:

	1.	Preferred development workflow involves the use of project management tracking tools like JIRA,
		Confluence. Developing practices like TDD, Unit Testing, XP, BDD. 
		The use source control like GIT/svn and continuous integration tools like Jenkins and Hudson

	2.   Typical development workflow will follow software development lifecyle:

		a. Requirement gathering

		b. Participation in system and interface design with Architects and UX Team

		c. Lead SPRINT Planning (Define SPRINT goals)

		d. Refining backlog with Product Owners and Team

		e. Create tickets and associate estimations and  resources with team

		f. Leading code reviews

		g. Ensuring Testing Framework is in place to check deliverables and requirement are met.

		h. Owning the code base and release cycles

		i. Working with Platform team to mange deployment and release management

		j. Managing bug fixes, and making sure regression tests are fully fulfilled

		k. Supporting aftercare (Hypercare)

		l. Refining and improving product and platform


	3	How to ensure that the quality of your code is high, and meets the standards of the project:

		1. Having best practices in place and supporting continuos delivery. 

		2. Using Automated Testing

		3. Having  a code review process in place. 

		4. Reducing manual testing times and spending more time on improving code quality

		5. Follow and support development and usability standards proclaimed by W3C

		6. Breaking features into smaller modules and having  test framework and documentation in 
		   place to support.

		7. Ensuring incremental releases. As this will allow to mange volume of flaws

		8. Have a micro-service architecture in place that ensures features are shipped with their 
		   context and configuration management services. 

		9. No configurations will sit outside the features that are developed. They will be contained 
		   in the same repository. This will be to avoid platform configuration changes that can potentially result 
		   in code and applications breaking. Use Docker, Puppet and Vagrant to support the application build

		10. Have documentation and dashboard available and easily accessible to the development team and stakeholders

		11. Ensure there is consistent and constant communication in the team with actions and setup agenda.


	4.	Improving and managing  complicated API random calls to disparate systems:

		The API data flow to the the UI environment may initially consist of making several API calls to a variable
		number of  different data sources from the backend. May include  Machine Learning servers, ElasticSearch indexes, 
		H-BASE and CORE  source. Making these numbers of API calls to such disparate  systems is  expensive and increases 
		latency and expected response times. 

		Such an architecture can be re-vamped by  bulding a gatewawy to allow all the data systems to manage and push into
		a central gateway poll, using for example Apache's ActiveMQ as middleware, from where the UI backend will make a 
		single call to the gateway pipeline. The gateway serves to save data and replicate across multiple services with
		stored changes.  It also allowed multiple  end points to subscribe to the service that it provides.


	5.   Ensuring that websites and apps built are performant for your target audience, and address performance issues:

		a. Have as part of the infrastructure devices that are commonly used by the customers to  access and use the 
		   product during  development. This will allow you to  capture some bottlenecks that could be obvious and 
		   inherent during development

		b. Research into  customer needs. This is fed into requirement gathering, analysed and turned into specification.

		c. Have automated debugging tools available and incorporated in the code building phase. Use Dev and debugging 
		   Tools built into browser. 
		   Use integrated test frameworks like BrowserStack, Selenium and  BDD (Behavior Driven Design) to handle user 
		   stories and acceptance criteria.

		d. Have a usability testing phases whiles the product is being built. Done to gather customer feedback

		e. Ensure a beta  release of the application will be in place and create a segmentation for a cross section 
		   of customers to evaluate.

		   Normally segmentation is done with loyalty uses. These are reliable customers who use the application very often,
		   so it is important to seek their opinion

		f. Engage positive feedback, workshops with customer services and platform/release management/DevOps to review customer 
		   concerns with view to refining product features,

		g. Use Analytics tools to build statistics and pattern of customer behaviour i.e - Omniture/Google Analytics
