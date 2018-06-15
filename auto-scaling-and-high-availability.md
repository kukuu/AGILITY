# Auto Scaling and High Availability

Customers demand a lot these days—but they’re willing to reward the enterprises that deliver. Satisfying customers takes an IT infrastructure that is resilient enough to withstand outages and greatly reduce planned and unplanned downtime. Think of it as nonstop IT. It’s what the most successful businesses are beginning to master and it’s putting pressure on the entire industry to up its game.

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