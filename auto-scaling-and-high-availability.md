# Auto Scaling and High Availability

Customers demand a lot these days, but they’re willing to reward the enterprises that deliver. Satisfying customers takes an IT infrastructure that is resilient enough to withstand outages and greatly reduce planned and unplanned downtime. Think of it as nonstop IT. It’s what the most successful businesses are beginning to master and it’s putting pressure on the entire industry to up its game.

Applications and processes that are critical to your business need around-the-clock monitoring and care. Excessive unscheduled downtime is not an option. Learn how to create a nonstop IT infrastructure with SUSE.

```

When downtime is not an option and your Recovery Time Objective (RTO) is measured in MINUTES, you need to take a serious look at a serious solution, ‘High Availability’

```

High availability refers to systems and solutions that are durable and which are likely to operate continuously, without failure for a long time. The term implies that a system has accommodations for failure in the form of redundant components and can recover from software or hardware failure automatically. The more transparent that failover is to users, the higher the availability of the system

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



### PAY ONLY FOR WHAT YOU NEED

AWS Auto Scaling can help you optimize your utilization and cost efficiencies when consuming AWS services so you only pay for the resources you actually need. When demand drops, AWS Auto Scaling will automatically remove any excess resource capacity so you avoid overspending. AWS Auto Scaling is free to use, and allows you to optimize the costs of your AWS environment.
