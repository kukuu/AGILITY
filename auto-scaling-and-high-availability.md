

# Architecting for High Availability, Auto Scaling and  & Multi-availability Zones

Amazon Web Services (AWS) provides a platform that is ideally suited for building highly available systems, enabling you to build reliable, affordable, fault-tolerant systems that operate with minimal amount of human interaction.


Customers demand a lot these days, but they’re willing to reward the enterprises that deliver. Satisfying customers takes an IT infrastructure that is resilient enough to withstand outages and greatly reduce planned and unplanned downtime. Think of it as non-stop IT. It’s what the most successful businesses are beginning to master and it’s putting pressure on the entire industry to up its game.
 
 ## KPIs for High Availability
 
These KPIs provide the basis for building a credible scaleable development infrastructure. Achieving them requires the adoption of Lean Engineering Practices including, but not limited to:
 
 AREST
 
 ```
Automation - Deployment should happen automatically. Creating and publishing packages are for 
the dark ages!

Reproducible - Production environment should be the same as the development environment. 
Issues in production should be easy to reproduce in development. 

Elastic - Easy to scale up or down services based upon demand.

Smooth - Zero downtime while scaling or upgrading the service. Process of re-instating a failed
build should be trivial.

Traceable - Logging & monitoring should be in place to watch for issues
```

Applications and processes that are critical to your business need around-the-clock monitoring and care. Excessive unscheduled downtime is not an option. 

```

When downtime is not an option and your Recovery Time Objective (RTO) is measured in MINUTES,
you need to take a serious look at a serious solution, ‘High Availability’

```

High availability refers to systems and solutions that are durable and which are likely to operate continuously, without failure for a long time. The term implies that a system has accommodations for failure in the form of redundant components and can recover from software or hardware failure automatically. The more transparent that failover is to users, the higher the availability of the system

### 5 Best Design Architectural Practices 

```
1. Design for failure. Avoid single points of failure, and have remedy strategies in place:
```

i. https://github.com/kukuu/AGILITY/blob/master/AWS-AS/1-designing-4-failure/1-dff.png

ii.https://github.com/kukuu/AGILITY/blob/master/AWS-AS/1-designing-4-failure/2-dff.png

iii. https://github.com/kukuu/AGILITY/blob/master/AWS-AS/1-designing-4-failure/3-dff.png

iv. https://github.com/kukuu/AGILITY/blob/master/AWS-AS/1-designing-4-failure/4-dff.png

v. https://github.com/kukuu/AGILITY/blob/master/AWS-AS/1-designing-4-failure/5-dff.png

vi. https://github.com/kukuu/AGILITY/blob/master/AWS-AS/1-designing-4-failure/6-dff.png

```
2. Have Multiple Availability Zones
```
i. https://github.com/kukuu/AGILITY/blob/master/AWS-AS/2-architecting-4-multiple-availability-zones/1-az.png 

ii. https://github.com/kukuu/AGILITY/blob/master/AWS-AS/2-architecting-4-multiple-availability-zones/2-az.png

iii. https://github.com/kukuu/AGILITY/blob/master/AWS-AS/2-architecting-4-multiple-availability-zones/3-az.png

iv. https://github.com/kukuu/AGILITY/blob/master/AWS-AS/2-architecting-4-multiple-availability-zones/4-az.png

 v. https://github.com/kukuu/AGILITY/blob/master/AWS-AS/2-architecting-4-multiple-availability-zones/5-az.png

```
3. Scaling

```
```
4. Self Healing 

```

```
5. Loose coupling

```



## Using a Load Balancer With an Auto Scaling Group

You can automatically increase the size of your Auto Scaling group when demand goes up and decrease it when demand goes down. As the Auto Scaling group adds and removes EC2 instances, you must ensure that the traffic for your application is distributed across all of your EC2 instances. 

The Elastic Load Balancing service automatically routes incoming web traffic across such a dynamically changing number of EC2 instances. Your load balancer acts as a single point of contact for all incoming traffic to the instances in your Auto Scaling group. 

To use a load balancer with your Auto Scaling group, create the load balancer and then attach it to the group.

## Steps to take

```

1. Attaching a Load Balancer to Your Auto Scaling Group

2. Use ELB Health Checks with Auto Scaling

3. Expanding Your Scaled and Load-Balanced Application to an Additional Availability Zone

```

## AWS Auto Scaling 

AWS AS monitors your applications and automatically adjusts capacity to maintain steady, predictable performance at the lowest possible cost. Using AWS Auto Scaling, it’s easy to setup application scaling for multiple resources across multiple services in minutes.

The service provides a simple, powerful user interface that lets you build scaling plans for resources including Amazon EC2 instances and Spot Fleets, Amazon ECS tasks, Amazon DynamoDB tables and indexes, and Amazon Aurora Replicas. AWS Auto Scaling makes scaling simple with recommendations that allow you to optimize performance, costs, or balance between them. 

If you’re already using Amazon EC2 Auto Scaling to dynamically scale your Amazon EC2 instances, you can now combine it with AWS Auto Scaling to scale additional resources for other AWS services. With AWS Auto Scaling, your applications always have the right resources at the right time.

It’s easy to get started with AWS Auto Scaling using the AWS Management Console, Command Line Interface (CLI), or SDK. AWS Auto Scaling is available at no additional charge. You pay only for the AWS resources needed to run your applications and Amazon CloudWatch monitoring fees.

### Benefits

Two main factors that comes into play with AWS AS are Flexibily and Cost.

#### SETUP SCALING QUICKLY

AWS Auto Scaling lets you set target utilization levels for multiple resources in a single, intuitive interface. You can quickly see the average utilization of all of your scalable resources without having to navigate to other consoles. For example, if your application uses Amazon EC2 and Amazon DynamoDB, you can use AWS Auto Scaling to manage resource provisioning for all of the EC2 Auto Scaling groups and database tables in your application.


#### MAKE SMART SCALING DECISIONS

AWS Auto Scaling lets you build scaling plans that automate how groups of different resources respond to changes in demand. You can optimize availability, costs, or a balance of both. AWS Auto Scaling automatically creates all of the scaling policies and sets targets for you based on your preference. AWS Auto Scaling monitors your application and automatically adds or removes capacity from your resource groups in real-time as demands change.


#### AUTOMATICALLY MAINTAIN PERFORMANCE

Using AWS Auto Scaling, you maintain optimal application performance and availability, even when workloads are periodic, unpredictable, or continuously changing. AWS Auto Scaling continually monitors your applications to make sure that they are operating at your desired performance levels. When demand spikes, AWS Auto Scaling automatically increases the capacity of constrained resources so you maintain a high quality of service.



#### PAY ONLY FOR WHAT YOU NEED

AWS Auto Scaling can help you optimize your utilization and cost efficiencies when consuming AWS services so you only pay for the resources you actually need. When demand drops, AWS Auto Scaling will automatically remove any excess resource capacity so you avoid overspending. AWS Auto Scaling is free to use, and allows you to optimize the costs of your AWS environment.

## Terraform

It is a command line tool for building, changing, and versioning infrastructure safely and efficiently. Terraform can manage existing and popular service providers as well as custom in-house solutions. Configuration files describe to Terraform the components needed to run a single application or your entire datacenter.

 Terraform is an “infrastructure as code” tool similar to AWS. Terraform's code is written in HashiCorp's proprietary language called HashiCorp Configuration Language (HCL). HCL is a structured configuration language that is intended to be both machine friendly and human readable.

  It is an open source tool that codifies APIs into declarative configuration files that can be shared amongst team members, treated as code, edited, reviewed, and versioned.

  https://linoxide.com/devops/install-terraform-provision-aws-ec2-instance/


## VPCs and Subnets

A virtual private cloud (VPC) is a virtual network dedicated to your AWS account. It is logically isolated from other virtual networks in the AWS Cloud. You can launch your AWS resources, such as Amazon EC2 instances, into your VPC.

Benefit of VPC is that it helps in aspects of cloud computing like privacy, security and preventing loss of proprietary data. Lets take a look at some of the basics of a VPC. Subnets: A subnet can be thought of as dividing a large network into smaller networks.


## CIDR

Classless inter-domain routing (CIDR) is a set of Internet protocol (IP) standards that is used to create unique identifiers for networks and individual devices. The IP addresses allow particular information packets to be sent to specific computers.

https://specialties.bayt.com/en/specialties/q/270484/what-is-cidr-and-why-it-is-important-in-today-s-scenario/

