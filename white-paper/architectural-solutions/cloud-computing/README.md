
# Cloud Computing Platforms & Service Models

Cloud Computing is a broad term that describes a broad range of services. Since the Cloud is a broad collection of services, organizations can choose where, when, and how they use Cloud Computing. Such services are, Software as a Service (SaaS), Platform as a Service (PaaS) and Infrastructure as a Service (IaaS).

Cloud computing is a model for enabling convenient, on-demand network access to a shared pool of configurable computing resources (e.g., networks, servers, storage, applications, and services) that can be rapidly provisioned and released with minimal management effort or service provider interaction. By using these services there is the potential to reduce IT support costs by outsourcing hardware and software maintenance and support to the providers.

Characteristics associated with Cloud Computing services include:

```

i. On-demand self-service. The ability for an end user to sign up and receive services without the long delays that have characterized traditional IT normally using thin client like the Browser.

ii. Broad network access. Ability to access the service via standard platforms (desktop, laptop, mobile etc)

iii. Resource pooling. Resources are pooled across multiple customers.

iv. Rapid elasticity. Capability can scale to cope with demand peaks.

v. Measured Service. Billing is metered and delivered as a utility service

```

### Models

#### SaaS (Software as a Service) applications are designed for end-users, delivered over the web.

SaaS is a software distribution model in which applications are hosted by a vendor 
or service provider and made available to customers over a network, typically the Internet.

With Saas model you are provided with access to application softwares often 
referred to as on-demand softwares. 
You don't have to worry about the installation, setup and running of the application. 
Service provider will do that for you. You just have to pay and use it through some client.

Example: Google Apps, Microsoft Office 365.

#### PaaS
PaaS (Platform as a Service) is the set of tools and services designed to make coding and deploying those applications quick and efficient over the Internet.

The model is a category of cloud computing services that provides a platform allowing 
customers to develop, run, and manage web applications without the complexity of building and
maintaining the infrastructure typically associated with developing and launching 
an app - via the browser.

Examples: AWS Elastic Beanstalk, Windows Azure, Heroku, Force.com, Google App Engine, 
and Apache Stratos.
IaaS (Infrastructure as a Service), is the hardware and software that powers it all – servers, storage, networks, operating system.


#### IaaS

IaaS provides you the computing infrastructure, physical or (quite often) virtual machines and 
other resources like virtual-machine disk image library, block and file-based storage, firewalls,
load balancers, IP addresses, virtual local area networks etc. 

Examples: Amazon EC2, Windows Azure, Rackspace, Google Compute Engine.
Additional points to note:

AWS(Amazon web services) is a complete suite which involves a whole bunch of useful web services. 
Most popular are EC2 and S3 and they belong to IaaS service model.

Although Hadoop is based on previous works by Google(GFS and MapReduce), it is not from Google. 
It is an Apache project.It is just a distributed computing platform and does not fall into 
any of these service models

Windows Azure is both a PaaS and IaaS.

## Scalability

Performance
Hadoop MapReduce (Hadoop Map/Reduce) is a software framework for distributed processing of 
large data sets on compute clusters of commodity hardware. It is a sub-project of the 
Apache Hadoop project. The framework takes care of scheduling tasks, 
monitoring them and re-executing any failed tasks. 

Choose a particular platform based on your requirements and needs. For example, if you want to 
have a Hadoop cluster on which you would run MapReduce jobs, you will find EC2 a perfect fit, 
which is IaaS. On the other hand if you have some application, written in some language, 
and you want to deploy it over the cloud,  you would choose something like Heroku, 
which is an example of PaaS.



## Microservices




Loose coupling::individual deployment:: repeatable deployment can only be achieved by repeatble context ==> containerisation
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

4.   Use Containerisation



## The TWELVE-FACTOR App

The twelve-factor app is a methodology for building software-as-a-service apps that:
```
i. Use declarative formats for setup automation, to minimize time and cost for new developers joining the project

ii. Have a clean contract with the underlying operating system, offering maximum portability between execution environments

iii. Are suitable for deployment on modern cloud platforms, obviating the need for servers and systems administration

iv. Minimize divergence between development and production, enabling continuous deployment for maximum agility

v. Scales up without significant changes to tooling, architecture, or development practices.
The twelve-factor methodology can be applied to apps written in any programming language, and which use any combination of backing services (database, queue, memory cache, etc).

- https://12factor.net

```

## Architectures

1. End to end integration - https://github.com/kukuu/AGILITY/blob/master/test-pyramid-coverage.jpg

2. AWS

	i. Architecting for High Availability & Multi-Availability Zones - https://github.com/kukuu/AGILITY/tree/master/AWS-AS 

	ii. Back end - https://github.com/kukuu/AGILITY/blob/master/aws-backend-app-pipeline.png

	iii. Front end - https://github.com/kukuu/AGILITY/blob/master/aws-web-app-pipeline.png 


3. Docker - https://github.com/kukuu/AGILITY/tree/master/docker 

4. Kubernetes - https://github.com/kukuu/AGILITY/tree/master/kubernetes 

5. CI Pipeline - https://github.com/kukuu/AGILITY/blob/master/CI-CDL-CDPL-pipeline.jpg 

6. Microservices - https://github.com/kukuu/AGILITY/blob/master/MICRO-SERVICES-oriented%20Architecture.png 

7. SOA - https://github.com/kukuu/AGILITY/blob/master/SOA-1.png 

8. Test Pyramid (Coverage) - https://github.com/kukuu/AGILITY/blob/master/test-pyramid-coverage.jpg


## Resources

1. Microservices vs SOA Architectures

https://github.com/kukuu/AGILITY/blob/master/white-paper/architectural-solutions/difference-between-monolithic-and-microservices-architecture-1.png

2. AWS Auto scaling - https://aws.amazon.com/autoscaling/

3. Continuous Integration, Continuous Delivery and Continuous Deployment and the Vector Pipeline

i. https://github.com/kukuu/AGILITY/blob/master/white-paper/architectural-solutions/continuous-integration-with-team-city.png

ii. https://github.com/kukuu/AGILITY/blob/master/white-paper/architectural-solutions/CI-CDL-CDPL-pipeline.jpg

4. Elastic Load Ballancers (ALP, Classic and Network - https://docs.aws.amazon.com/elasticloadbalancing/latest/application/introduction.html 

5. Cloud Native

i. Container Solutions - https://container-solutions.com/what-is-cloud-native/ 

ii. Security Strategies - https://www.twistlock.com/2017/10/02/security-cloud-native-environments/?ads_cmpid=1071572634&ads_adid=54488335919&ads_matchtype=b&ads_network=g&ads_creative=269316971720&utm_term=&ads_targetid=dsa-446131505180&utm_campaign=&utm_source=adwords&utm_medium=ppc&ttv=2&gclid=EAIaIQobChMIld3mtZqF3QIVqrXtCh16MwdBEAAYAyAAEgLSO_D_BwE 

6.Agility -  https://github.com/kukuu/AGILITY 

7. Unit Test - https://github.com/kukuu/AGILITY/blob/master/unit-test/notes.rtf 

8. Architectural Solutions - https://github.com/kukuu/AGILITY/tree/master/white-paper/architectural-solutions

9. ... https://github.com/kukuu/worldlabs/blob/master/resources.md





