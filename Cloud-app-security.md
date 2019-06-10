# Cloud app security 


## How not to fail

Unfortunately these days, the burden of creating secure technology solutions—using the right approaches, models, and technology—belongs to developers.



The movement to DevOps and CloudOps places the responsibility of writing and testing secure cloud applications back on developers. While you have operational SMEs in the loop, including security admins, most are not well versed in cloud-oriented security approaches. That means developers assume responsibility for security by default. That's a big responsibility.


Newer security models such as identity and access management (IAM) need to be coded right into applications. That means software engineers need to understand the functions of IAM, as well as how the organization's security model and enabling technology should be layered into the application.


The use of APIs, including public and private cloud services within applications, means developers must come up with the approaches and enabling technology needed to secure these services. API managers, and API security technology, are the law of the land these days, and it's up to software engineers to take charge.

If developers are responsible for dealing with cloud application security, then what do you need to understand before you can be an effective cloud application developer? You need to focus on higher-level, more valuable concepts, such as encryption at rest, encryption in flight, encryption in use and IAM.



## Encryption 

## What developers need to know 

To define cloud application security requirements with regard to your data, you need to focus in three areas:

1. Encryption in flight, or the need to secure data as it flows from system to system. In some instances, this is where data is most vulnerable.

2. Encryption at rest, or data as it sits in a storage sub-system. This includes data that exists in raw storage, or in a database.

3. Encryption in use, or data that an application accesses and manipulates. Data services let you access data in use through layers of abstraction. 

Whether the data is in use or not, the same security requirements always exist.

## Managing Performance - as latency mounts

1. Developers often have a knee-jerk response and encrypt everything everywhere. While that sounds like the safest route, there are trade-offs you should consider first. For instance, if you implement encryption in flight, you'll have to 
encrypt and decrypt data before you place it on the network for remote consumption, and before any of your applications can consume it. That requires processing time and imposes a performance penalty that, in the cloud, can add up to a major cost. 

Make sure you have clear requirements for encryption in flight and that the level of risk and potential loss, calculated, is worth the cost of using encryption in flight.

2. Encryption at rest is the most practical to apply, because you're ensuring that the data can't be read as it sits on a cloud-based storage system. This is an especially important best practice because you don't really know where or how your data is physically stored in the cloud. But if your data is encrypted, it shouldn't matter. 

That said, as a developer you still must deal with the extra resources and latency associated with encrypting the data. Again, do your risk/benefit analysis before moving forward with encryption at rest.

##. Enforcing IAM

As with encryption, you need to focus on IAM as a business driver as well as a security technology. Software engineers who deploy IAM must focus on the core business processes, as well as the details of the security process. 

The good news is that if you develop mature IAM capabilities, you can reduce identity management costs and become more agile in supporting new business initiatives at the same time. IAM functions will need to be embedded in more than half of all existing applications you migrate to the pubic cloud, as well as in almost 90 percent of new applications you build for the cloud.

What's more, the use of IAM within cloud application deployments will back-fill into the enterprise, as organizations modernize security approaches and technologies to align with the use of the public cloud. In many instances, IAM will be offered as a service back into the enterprise. In this way, the movement to cloud applications that are IAM-enabled will end up increasing the quality of existing enterprise security systems. 

As a result, cloud applications will be more secure than traditional on-premises enterprise applications, and developers who learn how to build IAM capabilities into cloud applications will likely layer those applications back into those traditional on-premises systems. That's absolutely required if you want to maintain a consistent level of security across the enterprise, for both cloud and on-premises environments.

Before selecting and deploying IAM for cloud-based platforms, developers must first consider their core requirements. Every problem domain is different, and so is the security solution. But in every case you'll need services in these four areas:

### Features of IAM


1. Identity management services

Identity management services refers to identity life-cycle management, access provisioning, centralized role management, and workflow design and implementation. The idea is to provide core identity management services that let you define core identities for all resources and actors; provide access to those resources; offer a centralized, enterprise-wide mechanism to store and read those identities; and manage how you can operationally leverage each.

The service offers user account provisioning, user account control, as well as group membership, IT compliance, access rights, and file server permissions management abilities.

2. Access management services

Access management services refers to single sign-on services, federation services, role-based access, and access to the platform. This works in conjunction with identity management services by using identity information to grant access based upon authorization.


3. Identity governance services

Identity governance services refers to role engineering, compliance, and identity assurance. This service places policies around how you manage identities, including the roles each has, how you link identities with compliance policies, and other aspects of managing identities when you need to put governance controls in place.

4. Multi-factor Authentication services

This refers to out-of-band authentication, and managed authentication services. The important point here is that you, as the developer, need to understand the core components of the IAM system you select, based on the requirements you've identified. The path to selecting the right solution involves listing your core IAM requirements, and matching up the solution components provided by each IAM technology provider.

IAM products all take a different approach. While some products focus on cloud computing, others are designed for more traditional enterprise approaches.

The trick is to pick an IAM technology that can meet most of your requirements. Unfortunately, many enterprises that deploy cloud-based platforms use two or even three different IAM products. For example, they might choose one to manage identity and another to manage single sign-on.

## Follow these best practices


1. Integrate cloud-based identity management solutions with enterprise security from the outset. Security should be holistic, and those charged with building security applications should do so using consistent application security approaches. It doesn't matter if you're in the cloud or not.

2. Focus on the design and architecture of your security solution first; select the technology second. While your solution will be more complex, the architecture should endure through many technology changes.

3. Build security testing into your DevOps automation. This means validating that your applications are properly secured and up to the specifications you've outlined and scripted. The automation of these tests and checks is critical to the consistent deployment of secure, cloud-based applications - Use SNYK as an example.

4. Consider performance in your design. While most IAM systems don't slow things down, in some situations they will; encryption can certainly cause latency. These kinds of issues are harder to fix after deployment. In addition, they tend to create issues with your security systems because users, annoyed by the performance issues, quickly figure out ways around your carefully constructed security mechanisms.

5. Know your industry's security regulations and compliance requirements. Once you have them, these can be managed by the identity governance system within IAM, and you can use these requirements to determine the type of encryption you need as well. It's tough to retrofit your compliance polices after implementation, so make sure you fully understand the requirements up front.

6. When it comes to implementing cloud application security, it's all on you. If something goes awry, you can't point to a committee of system admins and enterprise architects, as was the case when you built traditional enterprise applications, where just a user ID and a password were all you needed to worry about. 


### Guide to Software Test Automation Tools 

1. QMetry Automation Studio(QAS) is a leading software automation tool built on Eclipse IDE and leading open source frameworks, Selenium and Appium. QMetry Automation Studio brings structure, efficiency, and reusability to automation efforts.

2. TestComplete.


3. Robot Framework.

4. Ranorex.

5. SoapUI.

6. Katalon Studio.

7. HPE Unified Functional Testing


