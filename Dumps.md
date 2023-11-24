Links

- [Dumps 1](#dumps-1)
- [Dumps 2](#dumps-2)
- [Dumps 3](#dumps-3)


### Dumps 1

_Q1: A large manufacturing company would like to provide real-time feedback to machine operators regarding optimum machine speeds enabling less experienced operators to detect breaks earlier and maintain quality.Which service will allow the company to train and deploy a machine learning model that can detect machine issues early?_

**SageMaker**
> SageMaker helps you build, train, and deploy machine learning models quickly


Q2: A solutions architect wants to design an application architecture that reduces the risk of cascading failures between components. _Which design principles should be considered when planning the cloud architecture?_
(Choose 2)

- **Utilize loosely coupled components**
- **Design the architecture to reduce inter-dependencies**

> Loosely coupled components are connected but not dependent on each other. Loose coupling reduces the risk of cascading failures and can be achieved through asynchronous integration

> Architectures should be designed in a way that reduces inter-dependencies and the risk of cascading failures between components


Q3: A company that owns several warehouses (used to store and resell millions of like-new, open-box, and pre-owned items) would like to analyze images from their on-premises cameras to automatically detect if employees are wearing head covers (helmets) and other protective equipment. _Which service can be used to perform the image analysis?_

**Rekognition**

> The company can use Rekognition to identify objects like protective equipment in their images and detect if employees are wearing the required protective equipment


_Q4: In order to maintain HIPAA (Health Insurance Portability and Accountability Act) compliance, insurance providers and health plans must archive past patients' personal health information. The data will be accessed, at most, once or twice a year when requested by the Office for Civil Rights to ensure compliance. Which AWS service will provide the most cost-effective solution for storage and retrieval of these files?_

**S3 Glacier Deep Archive**

> S3 Glacier Deep Archive is used for long-term data archival that only needs to be accessed once or twice a year. It is often used to store data for regulatory compliance. If faster access times are needed, there is also S3 Glacier.

_Q5: You need to stream data in real time for a dashboard application_. Which AWS service would you use?

**AWS Kinesis**

> Kinesis allows you to analyze data and video streams in real time


_Q6: Where would you find the AWS Attestation of Compliance Documentation for PCI DSS?_

**AWS Artifact**

> AWS Artifact is your go-to, central resource for compliance-related information that matters to you. It provides on-demand access to AWS' security and compliance reports and select online agreements. AWS Support's site provides general information about compliance, but it does not hold the secure reports or certificates. AWS IAM is used to control security within your AWS Account. Amazon Macie is a data security classification service

Q7: In order to improve fault tolerance, you would like to begin using services that provide fault tolerance. _Which AWS services provide automatic replication across Availability Zones?_

- **DynamoDb**
- **S3**

_Q8: Under the AWS shared responsibility model, who is responsible for the configuration of infrastructure devices?_

**AWS is responsible for the configuration of infrastructure devices.**

> AWS maintains the configuration of its infrastructure devices. Don't forget AWS is responsible for its global infrastructure elements: Regions, edge locations, and Availability Zones



_Q9: Your organization is multi-national and uses multiple AWS Regions. Which AWS service can be used to route users to the nearest data center to reduce latency?_

**AWS Route 53**

> Route 53 is a DNS service that routes users to applications. Amazon Route 53 effectively connects user requests to infrastructure running in AWS (e.g., Amazon EC2 instances, Elastic Load Balancing load balancers, or Amazon S3 buckets) and can also be used to route users to infrastructure outside of AWS


_Q10: A company has underutilized servers in its on-premises data center. Unfortunately, they are still required to pay for idle resources. Which benefit of the cloud can help the company solve this problem?_

**Elasticity**

> With elasticity, the company doesn't have to plan ahead of time how much capacity they'll need - elasticity allows them to match the supply of resources with changing workload demands

_Q11: A customer set up an Amazon S3 bucket to accept downloads from their mobile application users. Due to data privacy requirements, the customer needs to automatically and continually scan S3 for the users' addresses. Which service can do this?_

**Macie**

> Macie uses machine learning to discover sensitive data stored on Amazon S3. Macie automatically detects a large and growing list of sensitive data types, including personally identifiable information (PII) such as names, addresses, and credit card numbers


_Q12: A financial company needs to migrate large amounts of data, at a petabyte scale, to AWS. Which AWS service can perform this type of migration?_

**AWS Snowball**

> Snowball is a petabyte-scale data transport solution

_Q13: Which of the following services helps you deliver content to your customers faster?_

**CloudFront**

> Amazon CloudFront is a content delivery network that speeds up the delivery of content to your users

_Q14: A DevOps engineer is planning for the deployment of an application that can't be impacted if an entire geographic location is affected by a disaster. How can the engineer deploy this application?_

**Deploy the application to multiple Regions**

> AWS logically groups its Regions into geographic locations. Each Region is spread out and fully independent and isolated from other Regions. If there's a flood, tsunami or earthquake in 1 Region, the other Regions will not be impacted. Because of this, it makes sense to deploy your application to multiple Regions



_Q15: When you upload an object to S3 storage, where will AWS keep it?_

In **multiple Availability Zones** within the Region you select

> Any object uploaded to S3 is automatically stored in multiple Availability Zones in the Region in which it was uploaded. This means that if any single AZ in a Region is experiencing issues, objects stored in S3 will still be available. Although objects in S3 can be made to be accessible globally, by default they are always stored in a redundant fashion in only the Region they were uploaded, ruling out the other answers

_Q16: You're hosting a web application on EC2. After a few days of production usage, you notice the traffic to the web application far exceeds what was expected. You've decided to move to a larger instance type. What AWS principle does this represent?_

**Vertical scaling**

> Vertical scaling is increasing the size and computing power of a single instance or node without increasing the number of nodes or instances.


_Q17: What is a geographical area of the world that is a collection of logically grouped data centers?_

**Region**

> A Region is a geographical area of the world that is a collection of data centers logically grouped into Availability Zones


_Q18: How can a customer on the Developer Support plan open a system impaired support case?_

Open a technical **support case via email**.

> Customers on the Developer Support plan can submit support cases for account and billing questions, service limit increases, and technical support cases via email only

_Q19: Which service allows users to record software configuration changes within servers running on-premises over time?_

**Config**

> Config allows you to assess, audit, and evaluate the configurations of your resources over time. Config works with EC2 instances, servers running on-premises, and servers and VMs in environments provided by other cloud providers

_Q20: You have just created a new bucket and uploaded a file into it. Will this be automatically viewable by anyone on the internet?_

No - **by default, buckets and their contents are private**

> By default, all data stored in S3 is not viewable by the public. If you want a bucket or object to be accessible by the public, you must explicitly make it so. NAT gateways and internet gateways are needed to allow communications between VPCs and the internet, but they are not required when it comes to S3.

_Q21: A startup is developing a new application. They don't know how to anticipate the usage or workload demands for the application. Which benefit of cloud computing will allow the startup to automatically adjust compute capacity based on demand?_

**Elasticity**

> With elasticity, the startup doesn't have to plan ahead of time how much capacity they'll need. Elasticity allows them to match the supply of resources with changing workload demands.



_Q22: A customer has an on-premises 5-gigabyte Oracle database that needs to be migrated to AWS and converted to Aurora. The customer requires minimal downtime to the database. Which service is the best option for migration and conversion?_

**Database Migration Service**

> DMS supports homogeneous migrations like Oracle to Oracle and heterogeneous migrations like Oracle to Aurora, with minimal downtime

_Q23: A solutions architect is designing a system to withstand the failure of one or more components. What type of system is able to withstand failure?_

**Highly available** 

> Highly available systems are designed to operate continuously without failure for a long time. These systems avoid loss of service by reducing or managing failures.

Q24: A customer would like to store secondary backup copies of on-premises data to the cloud. The customer is _not concerned about an extra level of protection by geographic redundancy_ but requires rapid access to the data when it is needed. _Which Amazon S3 storage class should be used as the lowest cost option with rapid access?_

**S3 One Zone-Infrequent Access**

> S3 One Zone-Infrequent Access is designed for customers who want a lower cost option for infrequently accessed data but do not require the multiple Availability Zone data resilience model of the S3 Standard or S3 Standard-Infrequent Access storage classes. S3 One Zone-Infrequent Access provides millisecond access when the data is needed

Q25: A company wants to provide access to an Amazon S3 bucket to all applications running on a Reserved Instance (RI) that's been assigned to a specific Availability Zone. _What's the best way to give S3 access to all applications running on the EC2 instance?_

Use an **instance profile to pass an IAM role with Amazon S3 permissions to the EC2 instance**

> The company will need to create a role that grants access to S3 and associate it with the instance



_Q26: A company is in the process of migrating its workloads to AWS, and they want to develop and implement security policies. What are some of the recommended best practices for Identity and Access Management (IAM) they can put in place to make sure their accounts are secure?_
(Choose 3)

- Enable **MFA for privileged users**
- **Create individual users instead of using root**
- **Do not share access keys**.


Question 27

_You need to visualize, understand, and identify trends for future charges, as well as manage your AWS costs and usage over time. Which AWS tool would you use?_

**AWS Cost Explorer**

> Cost Explorer allows you to visualize and forecast your costs and usage over time.

_Q28: For which of the below is S3 a suitable storage solution?_
(Choose 2)

**Pictures**, **Documents**


_Q29: AWS purchases computing resources in large quantities at lower costs and then passes volume discounts on to their customers. Which benefit of cloud computing does this demonstrate?_

**Lower pay-as-you-go prices due to massive economies of scale**

> Customers benefit from massive economies of scale and achieve lower variable costs than they can get on their own due to volume discounts

Question 30

Which of the following is an _AWS Well-Architected Framework design principle related to operational excellence?_

**Deploy smaller, reversible changes**


_Q31: AWS VPC is a component of which of the following overall service categories?_

**Networking and Content Delivery**

> Amazon Virtual Private Cloud (Amazon VPC) gives you full control over your virtual networking environment, including resource placement, connectivity, and security. VPC can be found under the Networking and Content Delivery category of services in the AWS Management Console


_Q32: An on-premises application requires a consistent, high-speed connection to the AWS Cloud environment that is better than an internet-based connection. Which AWS service can provide this connection?_

**Direct Connect**

> Direct Connect is a private (bypasses the public internet), dedicated physical network connection from your on-premises data center to AWS. Since the connection is private, it is extremely fast.



_Q33: Which of the following is used to secure Amazon S3 buckets?_

**Bucket access policy**

> A bucket access policy can be attached directly to an S3 bucket to limit access to specific users


_Q:34 A company is developing a new web application that has high availability requirements. How can the company increase availability when deploying the application?_
(Choose 2)

- Deploy the application to span across **multiple Availability Zones (AZs)**.
- Utilize a **multi-Region deployment** when deploying the application.

> Although deploying applications closer to users reduces latency, this alone doesn't ensure high availability


_Q35: You need to set a number range of EC2 instances to be made available to handle the load for your application. Which AWS service should you use?_

**AWS Auto Scaling**

> AWS Auto Scaling will ensure you have the optimal number of EC2 instances to handle your application's load, based on rules you specify. The other services mentioned can help distribute load amongst existing resources, but they do not have the ability by themselves to create new resources.

> Elastic Load Balancing automatically distributes your incoming application traffic across multiple EC2 instances

_Q36: A customer wants access to the full set of Trusted Advisor checks. What's the minimum support plan they need to have access to?_

**Business Support**

> Business Support is the minimum plan that provides access to the full set of Trusted Advisor checks

Question 37

A company is contemplating a move to the AWS Cloud. What benefits can be gained from such a move?

The company can focus on its business rather than managing a data center



_Q38: Which of the following are classified as migration services?_
(Choose 2)

- **AWS Snowball**
- **AWS Application Discovery Service**

> AWS Application Discovery Service helps you gather information about your on-premises environment and is considered a migration tool

> Snowball helps you migrate massive amounts of data into cloud, so it is considered a migration tool.

_Q39: A company is considering a serverless architecture_ and wants to _build and run applications without having to manage infrastructure_. _Which AWS services should the company consider using when building applications?_
(Choose 4)

**DynamoDB**, **Lambda**, **Fargate**, **S3**

Question 40

_Which is the most efficient AWS feature that allows a company to restrict IAM users from making changes to a common administrator IAM role created in all accounts in their organization?_

**Service control policies (SCPs)**


_Q41: A company is considering migrating its applications to AWS. Which costs should the company consider when comparing its on-premises total cost of ownership (TCO) to the TCO when running on AWS?_

- Software **license costs**
- **Data center cooling, power, and space requirements**
- **Hardware and infrastructure**




_Q42: Configuring user permissions so that users can access only the resources they need to do their job follows what principle?_

**Principle of least privilege**

> The principle of least privilege involves giving a user the minimum access required to get the job done

_Q43: A developer is building a new application and is given the option to deploy the application on-premises or to the AWS Cloud. What benefits does the AWS Cloud provide over an on-premises deployment?_

- Ability to **grow and shrink** computing capacity based on demand
- Ability to **focus on building the application** instead of managing servers
- Ability to **pay-as-you-go without upfront contracts** or long-term commitments


_Q44:A security administrator is setting up a new IAM user and has decided to grant the least privilege. What does the principle of least privilege mean?_

Granting the **minimum requiremen to perform a task** 

> The principle of least privilege means granting only the minimum requirements to perform a job or task

Question 45

_Which AWS service can help you optimize your AWS environment by giving recommendations to reduce cost, increase performance, and improve security?_

**AWS Trusted Advisor**

> Trusted Advisor provides real-time guidance to help you provision your resources following AWS best practices

_Q46: A company would like someone to help them coordinate access to AWS subject matter experts when they need help. Which support plan do they need to have?_

**Enterprise**

> Enterprise Support provides access to a Technical Account Manager (TAM) who helps coordinate access to subject matter experts among other things

_Q47: As an IT support center team member, you begin receiving calls from users about problems they're experiencing with your company's AWS-based point-of-sale system. You want to begin your investigation by checking with AWS for any service alerts they may be communicating. Which AWS tool will you give you the information you seek?_

**AWS Personal Health Dashboard**

> The AWS Personal Health Dashboard publishes alerts and remediation guidance when issues with AWS services arise. Notifications are also provided for scheduled events that may impact AWS customers



Q48: You have upgraded your AWS Support plan to the Business Support level. _What is true of the Business Support plan?_

**< 1 hour response time** support when your production system goes down.

> The Business level support plan provides 1 hour or less response time support for production-level failures

_Q49: How would you create and manage access keys for users that need to access AWS services from the AWS Command Line Interface (CLI)?_

**Identity and Access Management (IAM)**

> IAM allows you to create and manage access keys for an IAM user


Q50: A company is hosting a public-facing static website out of an S3 bucket. When reviewing website analytics and traffic, the company is surprised to learn the website is accessed by millions of users around the globe. The company wants to ensure all its users are seeing fast response times. _Which AWS service will help to deliver this website globally with low latency?_

**CloudFront**

> CloudFront is a CDN that delivers data and applications globally with low latency.

_Q51: What pillar of the Well-Architected Framework would include the use of information gathered through a workload process evaluation to drive adoption of new services or resources when they become available?_

**Performance Efficiency**

> This Performance Efficiency pillar focuses on the effective use of resources to meet demand. In this pillar, you would use the information gathered through the evaluation process to actively drive adoption of new services or resources. You would also define a process to improve workload performance, and you would need to stay up-to-date on new resources and services

_Q52: Which of the following allows you to make entire buckets (like 1 hosting an S3 website) public?_

**Bucket policies**

> Bucket policies allow you to control access to entire buckets, whereas access control lists let you control access to individual objects within an S3 bucket.

_Q53: A company has designed a hybrid architecture and needs to connect its on-premises database to an application running on an EC2 instance in the AWS cloud using a fast, private, and secure manner. Which method allows the company to securely connect on-premises to the cloud?_

**Direct Connect**

> Direct Connect is a private (bypasses the public internet), dedicated physical network connection from your on-premises data center to AWS. Since the connection is private, it is extremely fast


_Q54: Which AWS tool is specifically designed to help a company estimate their potential cloud bill for migrating workloads and calculate the overall total cost of ownership (TCO) based on their proposed workloads?_

The company can use the **AWS Pricing Calculator**
> The Pricing Calculator provides an estimate of AWS fees and charges. Since the company knows the workload details, the AWS Pricing Calculator can also help with calculating the total cost of ownership

Question 55

A large company is using multiple AWS accounts and would like to benefit from available volume discounts in AWS. _Which AWS feature will enable the company to get volume discounts?_

Use AWS Organizations and its **consolidated billing feature** to consolidate billing and payment for multiple AWS accounts

> Consolidated billing has the benefit of combining usage across all accounts in the organization to share the volume pricing discounts, Reserved Instance discounts, and Savings Plans. This can result in a lower charge for your project, department, or company than with individual standalone accounts

_Q56: The AWS Cloud spans multiple Regions, Availability Zones (AZs), edge locations, and more. How would you best describe an Availability Zone?_

**One or more discrete data centers with redundant power, networking, and connectivity in an AWS Region**

_Q57: A customer has created an Administrators group in IAM containing 5 users. What does the customer attach to the group to ensure all the users have the needed administrative access?_

**IAM policy**

> Policies can be attached to a group to ensure all users in the group have the same access. AWS even has a managed policy, Administrator Access, you can use.


Q58: Under the shared responsibility model for EC2, _who is responsible for patching the guest operating system?_

**The customer is responsible for patching the guest operating system**

_Q59: How can a customer with the Enterprise Support plan get help with billing and account questions?_
(Choose 2)

- Contact the **Support Concierge team**.
- Use the **AWS Support API to programmatically open a case with AWS Support.**

> The Concierge agent is the primary point of contact for billing or account inquiries

> Customers on the Enterprise Support plan have access to the AWS Support API to create, manage, and close support cases



_Q60: A company wants to ensure all AWS accounts in their environment conform to company-wide policies_. Which services can help?
(Choose 2)

- **Organizations**
- **Control Tower**
> Organizations allows you to centrally manage multiple AWS accounts under 1 umbrella. You can allocate resources and apply policies across accounts

> Control Tower helps you ensure your accounts conform to company-wide policies. Control Tower actually sits on top of Organizations.


 _Q61: A company is receiving automated alerts notifying them that their only production EC2 instance is continuously reaching 100% CPU utilization. When this happens, customers cannot make purchases and receive error messages stating they should try again later because all the company's servers are busy. As part of the solution, what could be used to add or replace EC2 instances of the same size automatically across AZs?_


**Horizontal scaling**

> Horizontal scaling (or scaling out) adds or replaces EC2 instances automatically across AZs, based on need and changing demand, and is used in the design of systems with high availability.



_Q62: A solutions architect is designing a new application for a customer. In designing the system, the architect recommends that content be cached to reduce latency to the end user. Which piece of the AWS global infrastructure allows for content to be cached and served from the nearest point to the user?_

**Edge location**

> An edge location uses cached copies of your content for fast delivery to users. Don't forget CloudFront speeds up delivery using edge locations.

_Q63: Your company would like to begin using Auto Scaling to add servers when CPU utilization reaches a certain threshold (e.g., 70%). Which service can you use to trigger actions when CPU utilization crosses the threshold?_

**CloudWatch Alarms**

> A CloudWatch alarm can be set up to monitor CPU utilization and trigger further action. Further action could be an Auto Scaling group adding another EC2 instance and/or using SNS to notify team members of the occurrence.

> Simple Notification Service can be used with CloudWatch to notify team members when a CloudWatch event or alarm is triggered, but SNS is not monitoring resource utilization


_Q64: A developer wants to be alerted when an EC2 running their application is approaching 100% CPU utilization_. Which service helps the developer do this in an automated way?

**CloudWatch**

> CloudWatch can monitor the state of your AWS resources and can notify you when an EC2 is approaching 100% utilization

Question 65

_In which of the following is CloudFront content cached?_

**Edge location**


## Dumps 2

_Q1: Select all the TRUE statements regarding the AWS Shared Responsibility Model._
(Choose 3)

- **Customers are responsible for security "in" the cloud**.
- **AWS manages the hardware and AWS Global Infrastructure**.
- AWS is responsible for security "of" the cloud

Question 2

_Which of the following tools provides a view of the performance and availability of your AWS services based on your requirements?_

**AWS Health Dashboard**

> Use the AWS Health Dashboard to learn about specific operational issues that affect your account. When you get an alert, it includes remediation details and specific guidance so that you can take action for events that affect your resources

_Q3: Which of the following can be used to author CloudFormation templates_?
(Choose 2)

**JSON**, **YAML**

_Q4:When considering common cloud computing models, which model is Amazon Elastic Compute Cloud (AWS EC2) an example of?_

**Infrastructure as a Service (IaaS)**

> IaaS includes the fundamental building blocks that can be rented from AWS. AWS manages the infrastructure and provides you a virtual machine that you can use however you'd like to meet your business requirements

Question 5

_Your Finance Department has instructed you to save costs wherever possible when using the AWS Cloud. You notice that using reserved EC2 instances on a 1-year contract will save money. What payment method will save the most money?_

All Upfront

_Q6: You have been tasked with creating identical, repeatable infrastructure for your customers. Which service will you use?_

**CloudFormation**

> CloudFormation provides the ability to provision a repeatedly deployable environment for your customers.


_Q7: Upon attempting to create an additional S3 bucket, you realize you have reached your S3 bucket limit in your AWS account. You anticipate creating even more S3 buckets in the future for your photos and documents. Which of the following is the best long-term solution?_

**Submit a service limit increase**

> The best long-term solution is to request a service limit increase at the AWS Support Center

_Q8: Which of the following is an AWS managed database service that is compatible with MySQL?_

**Aurora**

> Aurora is an AWS managed database service that is up to five times faster than a traditional MySQL database.

_Q9: Microsoft has announced a new patch for its operating system. For a platform-as-a-service solution, who would be responsible for applying the patch?_

**AWS**

> The platform-as-a-service model removes the need for organizations to manage the underlying infrastructure (usually hardware and operating systems) and allows you to focus on the deployment and management of your applications

Question 10

_Which benefit of cloud computing is demonstrated when you don't have to plan ahead of time how much capacity you will need to run your applications?_

**Elasticity**

Question 11

When AWS uses tape media to perform backups in their data centers, who would be responsible for their safe and secure disposal?

AWS



_Q12: What benefits can CloudFront bring to your e-commerce website?_
(Choose 3)

- Increased **application availability**
> You can improve resiliency and increase availability for specific scenarios by setting up CloudFront with origin failover.
- **Protection against network and application layer attacks via WAF**
> CloudFront provides protection with AWS WAF and AWS Shield.
- **Lower latency for customers of your e-commerce website**
> CloudFront provides the ability to cache both static and dynamic content around the world, ensuring quick response times for customers when retrieving cached website content.


_Q13: Which of the following acts like built-in firewalls per instance for your virtual servers?_

**Security groups**

> Security groups act like built-in firewalls for your virtual servers — the rules you create define what is allowed to talk to your instances and how. Although network access control lists can be used to block or deny traffic, these operate at the subnet level (covering all instances in the subnet with the same ruleset), not per instance as the question specifies. Route tables tell traffic where it should go next to reach its destination, and an Availability Zone is a collection of data centers — which isn't relevant in this question

_Q14: A user has created several IAM users in their account to perform administrative and general tasks. How can the user monitor and track the IP address of the users performing activities in their account?_

**CloudTrail**

> CloudTrail tracks user activity (along with the user's IP address) and API calls within your account

Question 15

_Which of the following are load balancer types offered by AWS?_
(Choose 3)

**Network**, **Classic**, **Application**

Question 16

_Which security concept confirms that users are who they say they are, by presenting an identity (username) and providing a verification (password)?_

**Authentication**


Q17: A huge department store sells products online and in-person. Most of their customers use credit cards instead of cash when making purchases. For security purposes, the credit card data must be encrypted at rest. _Which services allow the department store to generate and store the encryption key used to secure the credit card numbers?_
(Choose 2)

- **CloudHSM**

> CloudHSM is a hardware security module (HSM) used to generate and store encryption keys
- **Key Management Service (KMS)**
> KMS allows you to generate and store encryption keys.

> Macie uses machine learning to discover sensitive data stored on Amazon S3. Macie automatically detects a large and growing list of sensitive data types, including personally identifiable information (PII) such as names, addresses, and credit card numbers

Question 18

Deploying your EC2 instances across multiple AZs will help address which cloud concept?

High availability

_Q19: A developer deployed an application that consisted of 1 Lambda function, a DynamoDB table, and a firewall using Web Application Firewall (WAF) via the AWS Command Line Interface (CLI). When attempting to access the application's resources via the AWS Management Console, the developer cannot find the Lambda function or DynamoDB table. What could be the problem?_

**The developer is probably in a different Region from where the resources were initially deployed.**

> Resources that aren't global are typically deployed to a specific Region. Since Regions are isolated and resources aren't automatically replicated across them, the developer needs to switch to the correct Region in order to find the resources.



_Q20: Which type of Elastic Load Balancer is recommended for flexible application management and supports HTTP and HTTPS/2 traffic?_

**Application Load Balancer**

> Application Load Balancer is best suited for load balancing of HTTP and HTTPS (HTTPS/2) traffic and provides advanced request routing targeted at the delivery of modern application architectures, including microservices and containers. Operating at the individual request level (Layer 7), Application Load Balancer routes traffic to targets within Amazon Virtual Private Cloud (Amazon VPC) based on the content of the request.


_Q21: Your company is moving to the AWS Cloud and is reviewing the shared responsibility model. Which item is entirely the responsibility of AWS?_

**Physical and environmental controls**

> AWS is responsible for protecting the physical infrastructure and environmental controls that run all of the services offered in the AWS Cloud. This infrastructure is composed of the hardware, software, networking, and facilities that run AWS Cloud services

Question 22

_Which of the following best describes DynamoDB?_

**DynamoDB is a NoSQL database**

Question 23

_Which of the below is true about root accounts on AWS?_
(Choose 2)

- **The root user should not be used for day-to-day activities**.
- **The root user has full access to everything in the AWS account**.

Question 24

_A small software company is starting to work with the AWS Cloud. Which service will allow them to find, test, buy, and deploy software that runs on AWS?_

**AWS Marketplace**



Q25: You are managing the company's AWS account. The current support plan is Basic, but you would like to begin using _Infrastructure Event Management_. What support plan (that already normally includes Infrastructure Event Management) should you upgrade to?

**Upgrade to the Enterprise plan**

> AWS Infrastructure Event Management is a structured program available to Enterprise Support customers that helps you plan for large-scale events, such as product or application launches, infrastructure migrations, and marketing events. It is also available to Business Support customers, but they need to pay an additional fee to use this service and cannot use it normally as part of their plan

Q26: A popular company that sells products online just experienced a distributed denial-of-service (DDoS) attack that consumed all available bandwidth on their network and didn't allow legitimate requests to be processed. _Which AWS services can the company integrate and combine going forward to prevent future attacks?_
(Choose 4)

- **Web Application Firewall (WAF)**
- **CloudFront**, **Route 53**
> DDoS protection via Shield Advanced is supported on several services, including CloudFront, Route 53
- **AWS Shield**
> Shield is a managed Distributed Denial of Service (DDoS) protection service. Shield Standard provides free protection against common and frequently occurring attacks. Shield Advanced provides enhanced protections and 24/7 access to AWS experts for a fee

> GuardDuty is an intelligent threat detection system that uncovers unauthorized behavior.

_Q27: The CTO of a software company has requested an executive summary detailing the advantages of a potential move to the AWS Cloud. What can you say is an advantage of an RDS database over a traditional database?_

**AWS maintains the underlying OS and performs software patching on the database**

> RDS is a managed service that makes it easy to launch and manage relational databases. RDS does provide a lot of value, like automated backups and software patching, and frees you up to focus on your applications

_Q28: Which AWS service can provide a Desktop as a Service (DaaS) solution?_

**Amazon WorkSpaces**

> Amazon WorkSpaces is a managed, secure Desktop-as-a-Service (DaaS) solution. You can use Amazon WorkSpaces to provision either Windows or Linux desktops in just a few minutes and quickly scale to provide thousands of desktops to workers across the globe.



_Q29: A developer needs to provide version control for multiple Python source code files. Which service will provide source control for the files?_

**CodeCommit**

> CodeCommit is a source control system for private Git repositories

Q30: An independent developer needs help with _monitoring service limits to ensure they don't exceed free-tier usage on their account_. Which services will help them monitor service limits?
(Choose 2)

- **Trusted Advisor**
> Trusted Advisor has a service limit dashboard that helps you monitor service limits.
- **CloudWatch**
> CloudWatch Alarms can be used to determine the percentage of utilization versus the limit.

_Q31: A company has signed a 3-year contract with a school district to develop a Teacher Absence Management application. They anticipate consistent, daily development work throughout the duration of this project. Which type of EC2 instance would be best suited for this scenario?_

- **Standard Reserved Instances**
> Standard Reserved Instances are optimal for projects with predictable, consistent daily usage over an extended period, such as this 3-year contract. They offer significant cost savings, up to 72%, compared to On-Demand pricing. Given the long-term and steady nature of the development project, these instances ensure both capacity reservation and cost-effectiveness. In contrast, other instance types like On-Demand or Spot are better suited for short-term or unpredictable workloads



_Q32: A company has multiple AWS accounts across many departments. They are considering using Organizations to group all their accounts under 1 master payer account. What are the benefits of using Organizations?_
(Choose 3)

- They can **reduce costs by sharing resources across accounts**
- They can **easily add new accounts or create new accounts**
- They can **receive 1 bill for all their AWS accounts**

Question 33

You are reviewing the AWS Shared Responsibility model to present an overview to management on what your company is responsible for in AWS. Which option is a customer responsibility?

Customer data   



_Q34: Under the shared responsibility model, which of the following is an example of security of the cloud?_
(Choose 3)

- **Maintaining networking components**
> AWS maintains networking components: generators, uninterruptible power supply (UPS) systems, computer room air conditioning (CRAC) units, fire suppression systems, and more
- **Managing the AWS global infrastructure**
> AWS is responsible for the security of the cloud. AWS is responsible for its global infrastructure elements: Regions, edge locations, and Availability Zones.
- **Protecting the data center infrastructure**
> AWS is responsible for protecting the infrastructure that runs all of the services offered in the AWS Cloud. This infrastructure is composed of the hardware, software, networking, and facilities that run AWS Cloud services
Question 35

_Which storage service can provide very high durability storage for objects?_

**Amazon S3**
> S3 provides high durability storage of objects

Question 36

_Your company is considering migrating its data center to the cloud. Which of the following is an advantage of the AWS Cloud over an on-premises data center?_

Replace upfront capital expenses with low variable costs



Q37: A company is using CloudTrail to simplify operational analysis and troubleshooting. _When tracking user activity, which content fields does CloudTrail track when a user accesses the AWS Management Console?_
(Choose 2)

**Region**, **Username**

> CloudTrail tracks the AWS Region that the request was made to, such as us-east-1.

> CloudTrail allows you to track the username.


Question 38

Which statement below is one of the 6 advantages of cloud computing?

**Benefit from increased speed and agility**

_Q39: A company needs to use a load balancer that can serve traffic at the TCP and UDP layers. Additionally, it needs to handle millions of requests per second at very low latencies. Which load balancer should they use?_

**Network Load Balancer**

> Network Load Balancer is best suited for load balancing of Transmission Control Protocol (TCP), User Datagram Protocol (UDP), and Transport Layer Security (TLS) traffic where extreme performance is required. Operating at the connection level (Layer 4), Network Load Balancer routes traffic to targets within Amazon Virtual Private Cloud (Amazon VPC) and is capable of handling millions of requests per second while maintaining ultra-low latencies


_Q40: You need to allow IPv4 resources in a private subnet to connect to services outside your VPC, but you can't allow external services to initiate a connection with those private IPv4 resources. Which of the following must be present to enable this access?_

**NAT gateway**

> A NAT gateway is required to allow resources in a private subnet to access the internet

_Q41: You are a Systems Administrator who has just started adding IAM users to your company’s AWS account. However, you worry that the users will not create passwords strong enough to prevent unauthorized access. What is the most reliable way to ensure that users are using strong passwords?_

**Apply an IAM password policy to ensure users create appropriately strong passwords**.

> Use Identity and Access Management (IAM) to apply an IAM password policy. While awareness and training are critical to developing good security practices, the most reliable option is to use an IAM password policy, which won't allow users to use lower-strength passwords

_Q42: Broadly speaking, as a customer of AWS, you are responsible for:_

**Security IN the Cloud**


_Q43: You just had a Data Analyst join the company, and you have been tasked with creating a new IAM user accordingly. Although the user has received all the necessary credentials, she realized that she cannot perform any Amazon RDS actions on the Clients table. Which of the following are possible solutions to this issue?_
(Choose 2)

- **Create an identity-based policy**
> By default, an IAM user can’t access anything in the AWS account. So, the inability to perform the RDS actions on the Clients table is not a technical or password issue. To grant access, you would need to create an identity-based policy. However, if there is a group in the account with the permission policy that will grant such access, you can add the user to that group instead
- **Add the user to the group that has the necessary permission policy**


_Q44: You have a MySQL database that you want to migrate to the cloud, and you need it to be significantly faster there. You are looking for a speed increase up to 5 times the current performance. Which AWS offering could you use?_

**Amazon Aurora**

> Aurora is a relational database compatible with MySQL and PostgreSQL that was created by AWS

_Q45: A company is using Trusted Advisor to ensure they are following AWS best practices. What real-time guidance does Trusted Advisor provide?_
(Choose 3)

- **Open-access permissions for S3 buckets**
> Trusted Advisor checks Amazon S3 buckets for open-access permissions, which allow anyone to access the bucket's contents. It also checks for bucket policies that might override these permissions, giving unintended users access to the bucket.
- **Low utilization on EC2 instances**
> Trusted Advisor checks this for all customers
- **Exposed access keys**
> Trusted Advisor checks this for Enterprise and Business Support customers.

_Q46: Which of the following are focuses of the performance efficiency pillar of the Well-Architected Framework?_
(Choose 2)

- Use a **serverless architecture** first.
- Use **multi-region deployments**.

_Q47: What is the maximum number of objects you can store in S3 per AWS account?_

**Unlimited**

> You can store an essentially unlimited number of objects in S3 - either in a single bucket or across multiple in your account

_Q48: Which are focuses of the security pillar of the Well-Architected Framework?_
(Choose 2)

- **Track who did what and when**
- Assign **only the least privilege required**


_Q49: A small company has purchased a new system which they want to deploy in the AWS Cloud but does not have anyone with the required AWS skill set to perform the deployment. Which service can help with this?_

**AWS Partner Network (APN) Consulting Partners**

> APN Consulting Partners include professional services organizations like system integrators, strategic consultancies, agencies, managed service providers (MSPs), and value-added resellers. In this case, we would engage a Consulting Partner to help us deploy a new system to the AWS Cloud.


_Q50: Which of the below are TRUE when running a database in an EC2 instance?_
(Choose 3)

- The customer is responsible for managing access to the database
- The customer is responsible for updating the database software
- The customer is responsible for updating the guest operating system

Question 51

_Which is a core design principle for deploying resources in AWS?_

Deploy in multiple Availability Zones.

_Q52: A new web application is getting much more traffic than expected. You decide to add another EC2 instance to share the load. Which AWS concept best describes the act of changing the number of instances using the same instance size?_

**Horizontal scaling**

> Horizontal scaling is the act of changing the number of nodes in a computing system without changing the size of any individual node. So, with horizontal scaling, we would add instances



_Q53: Which of the following database migrations are classified as **heterogeneous**?_
(Choose 2)

- **Microsoft SQL Server to Amazon Aurora PostgreSQL**
- **Oracle to Amazon Aurora PostgreSQL**


_Q54: Your company is migrating to the AWS Cloud. For servers, your company has existing per-core licenses they would like to continue to use. Which EC2 purchasing option allows this? (Subject to your license terms)._

**Dedicated Host**

> Dedicated Hosts allow you to use your existing per-socket, per-core, or per-VM software licenses, subject to your license terms.

_Q55: You are trying out AWS on a trial basis and need to deploy a web application without having to configure servers. Which AWS service can you use?_

- **Elastic Beanstalk**

> Elastic Beanstalk allows you to deploy your web applications and web services to AWS


_Q56: Which of the following data archival services is extremely inexpensive but can have a multi-hour data-retrieval window?_

**Glacier**
> Glacier offers extremely inexpensive data archival, but requires a 3- to 5-hour data-retrieval window for standard retrievals - though this time can be reduced for a price

Question 57

A company is _rearchitecting its monolithic application using a microservices architecture_. Which design principle for cloud architecture should the company consider?

**Implement loose coupling**

> Loose coupling helps reduce the risk of cascading failures between components

Q58: A recent audit has dictated that a _company begin keeping a log of AWS Management Console actions and API calls. Which AWS service can help with this?_

**AWS CloudTrail**

> CloudTrail tracks user activity and API calls within your account

> AWS Inspector: Inspector works with EC2 instances to uncover and report vulnerabilities

Q59: Your company has decided to use Amazon WorkSpaces. _They can use Amazon WorkSpaces to provision either Windows or Linux desktops in just a few minutes. What type of solution is this?_

**DaaS**

> Amazon WorkSpaces provides a Desktop as a Service (DaaS) solution

_Q60: A company is considering moving their critical applications and databases to the cloud. They want to ensure their data never becomes corrupted or lost due to a system malfunction. A system that reliably stores data without loss is considered to be what?_

**Durable**

> A system that stores data without loss is a durable one. Durability is all about long-term data protection. This means your data will remain intact without corruption.


_Q61: A company would like to reduce operational overhead when operating AWS infrastructure_. Which service can help them do this?

**Managed Services**

> Managed Services helps you efficiently operate your AWS infrastructure and reduces operational risks and overhead

_Q62: A company is considering moving its data and applications to the cloud. What are some of the benefits of moving to the cloud?_
(Choose 2)

- Operate production workloads that are more highly available, fault tolerant, and scalable
- Provision exactly the right type and size of computing resources you need

_Q63: Which of the following allows you to restrict access to an entire S3 bucket?_

**Bucket policies**

> Bucket policies allow you to control access to entire buckets

Question 64

_You suspect that 1 of the AWS services your company is using has gone down. How can you check on the status of this service?_

**AWS Personal Health Dashboard**

> AWS Personal Health Dashboard provides alerts and guidance for AWS events that might affect your environment

Question 65

You have many database backups you need to store for an indefinite amount of time. If the backups are ever needed, they just need to be retrieved within 4 hours. What is the lowest-cost solution for this scenario?

S3 Glacier Flexible Retrieval (formerly S3 Glacier)


## Dumps 3


_Q1: Using Infrastructure as Code **(IaC)** is related to which cloud concept?_

**Automation**
> Infrastructure as Code is a key implementation of automation in cloud - using Infrastructure as Code allows you to quickly and easily deploy and manage your environment without reliance on humans to complete all the tasks.

Question 2

_A company has an application with user bases in both Canada and New Zealand. The company has deployed their application to servers currently provisioned in the Canada (Central) Region. Unfortunately, New Zealand users are experiencing high latency and slow download times. How can the **company reduce latency**?_

**Provision resources to the Australia (Sydney) Region**

> A multi-Region deployment solves the issue by deploying the application closest to the user base

Question 3

_When might **Auto Scaling** be used?_

When you require **scalable capacity to maintain service** levels in your environment



_Q4: Where is the best place to **store your root user access key** so your application can use it to make requests to AWS?_

**Nowhere— you should not use the root user access keys for this**

Question 5

_You have a web application that needs to run for a short period of time. It is all right if there are interruptions in the application. Which EC2 instance type would be best for this use case?_

**Spot Instance**

Question 6

_Which of the following statements about AWS Regions is true?_
(Choose 2)

- Regions are generally specific geographical areas
- Regions are made up of Availability Zones

Question 7

_What defines **long-term data protection**?_

**Durability**

Question 8

Which of the following are valid EC2 pricing options?
(Choose 2)

- On-Demand
- Reserved

Question 9

_Which of the following EC2 instance types will realize a savings over time in exchange for a contracted term-of-service?_

Reserved Instances

Question 10

_When talking about AWS security, what does "**authorization**" refer to?_

Evaluating what permissions a user has

Question 11

_A company has provisioned an EC2 instance as a web server. The web application on the server is running within a subnet within a VPC. For some reason, the **application is unable to access the internet**. Which component is missing?_

**Internet gateway**

_Q12: Your company is migrating its services to the AWS Cloud. The DevOps team has heard about Infrastructure as Code and wants to investigate this concept. Which AWS service would they investigate?_

**AWS CloudFormation**

> AWS CloudFormation is a service that helps you model and set up your Amazon Web Services resources so you can spend less time managing those resources and more time focusing on your applications that run in AWS

Question 13

_Which of the following are geographic areas that host 2 or more Availability Zones?_

Regions

_Q14: Which of the following is an **AWS global service?**_

**CloudFront**

> Amazon CloudFront is a fast content delivery network (CDN) service that securely delivers data, videos, applications, and APIs to customers globally with low latency and high transfer speeds, all within a developer-friendly environment.


_Q15: Which of the following is an **AWS global service**?_

**IAM**
> Identity and Access Management is a global service

Question 16

_A company is launching a new product and needs help with assessing its operational readiness and identifying and mitigating risks. Which feature of the **Enterprise Support plan provides** this?_

**Infrastructure Event Management**

> Infrastructure Event Management provides support for planning and running business-critical events

Question 17

_A customer has multiple IAM users that need the same access permissions. How can the customer provide the same access permissions to all the users quickly and efficiently?_

By **assigning users to an IAM group** that has the needed permissions

Question 18

_An organization needs to run a MySQL relational database on AWS. They plan to hire their own database administrators to manage their databases, including taking backups, using replication, and clustering. Which option provides the customer the control and flexibility needed?_

Install the MySQL database directly on an EC2 instance

Question 19

_Which of the following is AWS' **data warehousing** service?_

**Redshift**


_Q20: Which AWS service provides central governance and management across multiple AWS accounts?_

**AWS Organizations**

> AWS Organizations allows you to centrally manage multiple AWS accounts under one umbrella

Question 21

_Which AWS design principle can be a **valuable feature when deploying applications**?_

**Loose coupling**

Question 22

_Your company has decided to migrate entirely to the AWS Cloud. Which answers are a part of the 6 advantages of cloud computing?_
(Choose 2)

- Go global in minutes
- Stop spending money running and maintaining data centers

Question 23

_A colleague tells you about a service that uses machine learning to **discover and protect sensitive data stored in S3** buckets. Which AWS service does this?_

**Macie**

Question 24

_The Solutions Architect leading your project tells you the application your team is working on requires a managed **NoSQL database**. Which of the following AWS services best fits that description?_

**DynamoDB**

Question 25

_Your team needs to begin **monitoring** the applications running in your AWS account by collecting **metrics, logs, and events.** Which AWS service can you use?_

**Amazon CloudWatch**

Question 26

_A company is planning for a one-time sale of 75% off all products on its website. They expect to see a **short-term spike on** the sale day. Which EC2 instance type should the company use to meet its requirements and **maximize flexibility**?_

**On-Demand**

Question 27

_A college student wants to quickly launch a **WordPress website** but doesn't have a lot of cloud experience. Which service will help the student launch the website with a **low, predictable monthly fee**?_

**Lightsail**



_Q28: Which of the following are focuses of the operational excellence pillar of the Well-Architected Framework?_
(Choose 3)

- **Plan for and anticipate failure**
- **Script operations as code**
- **Deploy smaller reversible changes**

> This is a focus of the operational excellence pillar. This pillar focuses on creating applications that effectively support production workloads.


Question 29

_Which type of user is created when you **initially sign up** for an AWS account?_

**Root user**

Question 30

_The load on your application fluctuates by day of the week. Wednesdays have the most traffic, and Saturdays have the least traffic. Which AWS service allows you to **ensure** you have the **correct amount of compute capacity** while also optimizing on a cost basis?_

**Auto Scaling**

Question 31

_A company is considering the cloud deployment models when planning a new application. Which deployment model allows the company to **fully stop spending money running and maintaining data centers**?_

**Public cloud**

Question 32

_What AWS service protects against distributed denial of service **(DDoS) attacks** at the network and transport layers (layer 3 and 4) and the application layer (layer 7)?_

**AWS Shield Advanced**

Question 33

_You are concerned about access to your top-secret application by stolen passwords. What additional layer of security can you add for logging in to the AWS Management Console, in addition to user passwords?_

**Multi-factor authentication**

Question 34

_Your company utilizes DNS and wants to **migrate DNS and management** of DNS to the cloud. Which AWS service would you use?_

**Route 53**

Question 35

_A company with a popular website would like to **analyze website clickstreams in real time** to determine site usability. How can they obtain the data in real time for analysis?_

**Kinesis**

Question 36

A customer provisioned an on-demand EC2 instance using a Linux AMI. The instance ran for 10 hours, 3 minutes, and 7 seconds before the user terminated it. How much time will the customer be billed for?

10 hours, 3 minutes, and 7 seconds

Question 37

_Which statement is true regarding the AWS Global Infrastructure?_

- Each AWS Region consists of multiple, isolated, and physically separate AZs within a geographic area.



_Q38: Which service is used to manage the **encryption of EBS volumes** for Amazon EC2?_

**Key Management Service (KMS)**
> When you create an encrypted Amazon EBS volume, you're able to specify a KMS customer master key

Question 39

_What AWS service lets you provision a **logically isolated section** of the AWS Cloud?_

**Amazon Virtual Private Cloud**

Question 40

_Which of the following are steps you should take in **securing your AWS accoun**t?_
(Choose 3)

- Activate Multi-factor Authentication **(MFA)** on your root account
- Use **groups to delegate access** to IAM users
- Create **individual IAM users**

Question 41

_Under the shared responsibility model, for which of the following does **AWS NOT assume responsibility**?_

Customer data

Question 42

_You work for a financial company that has several mission-critical workloads running on AWS. Which AWS Support plan should you use if you want response times in under 15 minutes when issues occur?_

**Enterprise**

Question 43

_A company is configuring IAM for its new AWS account. There are **5 departments** with between 5 to 10 users in each department. How can they efficiently apply **access permissions** for each of these departments and simplify management of these users?_

**Create policies for each department** that define the permissions needed. **Create an IAM group** for each department and attach the policy to each group. Add each department's members to their respective IAM group

Question 44

_A developer has noticed several **SQL injection attacks** against a web application running on an EC2 spot instance. What is the best way to prevent this type of attack?_

**Web Application Firewall (WAF)**

Question 45

_Which credentials can you use to access the **AWS Management Console**?_

Your **username and password**

_Q46: You have 2 software systems that need to communicate, and you also need to **ensure messages are not lost between them**. Which AWS service can help meet these requirements?_

**SQS**

> Amazon SQS is a message queue service used by distributed applications to exchange messages through a polling model and can be used to decouple sending and receiving components. Amazon SQS also provides extremely high message durability, ensuring messages are not lost if your software systems fail.

Question 47

_A company with a business-critical application needs to ensure business continuity and that they will not be impacted by capacity restraints in a given Region. How can the company ensure this?_
(Choose 3)

- **Convertible Reserved Instance** (RI) with a capacity reservation    
> A Reserved Instance is a reservation of resources and capacity for either 1 or 3 years. A capacity reservation offers assurance that the customer will be given preference if there is ever a capacity constraint in a Region
- **On-demand capacity reservation**
> On-Demand Capacity Reservations enable you to reserve compute capacity for your Amazon EC2 instances for any duration.
- **Standard Reserved Instance (RI) with a capacity reservation**


_Q48: A purchasing department staff member is set up as an AWS user in the company’s Procurement AWS account. At each month-end, the staff member needs access to an application running on EC2 in the company’s Accounts Payable AWS account to reconcile reports. Which of the following provides the most secure and operationally efficient way to give the staff member access to the Accounts Payable application**?_

**Have the user request temporary security credentials for the application by assuming a role**

> The staff member should be given the ability to assume a role programmatically with the permissions necessary to run the Accounts Payable application

Question 49

_Your company has decided to migrate a SQL Server database to a newly created AWS account. Which service can be used to **migrate the database**?_

**Database Migration Service**

Question 50

_Why would you use **tags** in AWS?_

To **organize your resources**

Question 51

_Which of the following support services do **all accounts receive** as part of the AWS Support Basic tier?_

**Billing support**

Question 52

_Which of the following is correct regarding the number of Regions, Availability Zones, edge locations, and data centers?_

There are more Availability Zones than Regions

_Q53: A customer needs to identify vulnerabilities on their EC2 instances, such as unintended network access. Which services will provide a report of findings?_
(Choose 2)

- **Inspector**
- **Trusted Advisor**
> Inspector works with EC2 instances to uncover and report vulnerabilities.

> Trusted Advisor is a tool that provides real-time guidance to help you provision resources following AWS best practices. It will check security groups for rules that allow unrestricted access (0.0.0.0/0) to specific ports

Question 54

_What can we do in AWS to receive the benefits of volume pricing for your multiple AWS accounts?_

Use **consolidated billing** in AWS Organizations.

Question 55

_Which of the following are **characteristics of Regions**?_
(Choose 3)

- They are **grouped in geographic locations**.
- **They contain only the resources and services specifically deployed to them.**

> Regions are isolated, and resources that are uploaded are not automatically replicated across them.
- They are fully independent and isolated.



Question 56

_With which AWS service, **coupled with EC2**, can you implement elasticity by **adding and removing instances** as needed?_

**Auto Scaling**

_Q57: You would like to set up a loosely coupled architecture. Which service would allow you to send and receive messages and store them if they are not consumed immediately?_

**AWS SQS**

> SQS is a message queuing service that allows you to build loosely coupled systems

Question 58

_A customer has decided to go with a 1-year Standard Reserved Instance (RI) for EC2 since their application has steady state and predictable usage. Which pricing option should they choose to earn the **  **?_

**All upfront**

Question 59

_A company is trying to **visualize and forecast** its costs and usage over time. Which service can help them?_

**AWS Cost Explorer**


_Q60: When analyzing application performance, a developer realizes the queries to the database are taking a long time. What can the developer implement to **store common queries** and improve performance?_

**ElastiCache**

> ElastiCache helps you alleviate database load for data that is accessed often. ElastiCache is a great way to cache common queries.

Question 61

_When talking about AWS security, what does "authentication" refer to?_

Identifying who is accessing the system

Question 62

_Which of the following is a design principle of the Well-Architected Framework's **reliability pillar**?_

**Recover from failure automatically**


_Q63: A customer is managing multiple AWS accounts using AWS Organizations. What can the customer use to restrict the same permissions across all AWS accounts managed under AWS Organizations using minimal effort?_

**Service control policies**

> AWS Organizations provides central governance and management for multiple accounts. Organization service control policies (SCPs) allow you to create permissions guardrails that apply to all accounts within a given organization.

_Q64: You have an EC2 instance that contains a web application being put into operation. To prepare for the application going live for public use, you add a few **more instances in a distributed manner** in order to **handle an increase in load**. Which concept is used to measure a system's ability to grow to accommodate an increase in demand?_

**Scalability**

> Scalability means the systems can adapt to meet new levels of demand. There are both horizontal and vertical scaling in regards to compute resources. Horizontal scaling involves the adding of instances of the same size. Vertical scaling is typically a manual process where the size of the instance is changed

Question 65

_A customer has set up an Amazon **S3 bucket** and wants to **limit access** to specific users. What is the most efficient way to do so?_

**Bucket access policy**



















_Q1: A multi-national corporation wants to get expert professional advice on migrating to AWS and managing their applications on AWS Cloud. Which of the following entities would you recommend for this engagement?_

**APN Consulting Partner**

> _Note_: The AWS Partner Network (APN) is the global partner program for technology and consulting businesses that leverage Amazon Web Services to build solutions and services for customers. APN Consulting Partners are professional services firms that help customers of all types and sizes design, architect, build, migrate, and manage their workloads and applications on AWS, accelerating their migration to AWS cloud.


Incorrect options:

APN Technology Partner - APN Technology Partners provide hardware, connectivity services, or software solutions that are either hosted on or integrated with, the AWS Cloud. APN Technology Partners cannot help in migrating to AWS and managing applications on AWS Cloud.

_Q2: Which of the following is a hybrid storage service that allows on-premises applications to access data on AWS Cloud?_

**AWS Storage Gateway**

> _Note:_ AWS Storage Gateway is a hybrid cloud storage service that connects your existing on-premises environments with the AWS Cloud. Customers use Storage Gateway to simplify storage management and reduce costs for key hybrid cloud storage use cases.

_Q3: A financial services company wants to ensure that its AWS account activity meets the governance, compliance and auditing norms. As a Cloud Practitioner, which AWS service would you recommend for this use-case?_

**CloudTrail**

> _Note_: You can use CloudTrail to log, monitor and retain account activity related to actions across your AWS infrastructure. CloudTrail provides an event history of your AWS account activity, including actions taken through the AWS Management Console, AWS SDKs, command-line tools, and other AWS services.

_Q4: The DevOps team at an e-commerce company is trying to debug performance issues for its serverless application built using a microservices architecture. As a Cloud Practitioner, which AWS service would you recommend addressing this use-case?_

**AWS X-Ray**


> _Note:_ You can use AWS X-Ray to analyze and debug serverless and distributed applications such as those built using a microservices architecture. With X-Ray, you can understand how your application and its underlying services are performing to identify and troubleshoot the root cause of performance issues and errors.

_Q5: A silicon valley based healthcare startup stores anonymized patient health data on Amazon S3. The CTO further wants to ensure that any sensitive data on S3 is discovered and identified. As a Cloud Practitioner, which AWS service would you recommend addressing this use-case?_

**Amazon Macie**

> _Note:_ Amazon Macie is a fully managed data security and data privacy service that uses machine learning and pattern matching to discover and protect your sensitive data in AWS. Macie automatically provides an inventory of Amazon S3 buckets including a list of unencrypted buckets, publicly accessible buckets, and buckets shared with AWS accounts outside those you have defined in AWS Organizations. Then, Macie applies machine learning and pattern matching techniques to the buckets you select to identify and alert you to sensitive data, such as personally identifiable information (PII).

_Q6: A unicorn startup is building an analytics application with support for a speech-based interface. The application will accept speech-based input from users and then convey results via speech. As a Cloud Practitioner, which solution would you recommend for the given use-case?_

Use Amazon **Transcribe to convert speech to text** for downstream analysis. Then use Amazon **Polly to convey the text results via speech**

_Q7: A company uses reserved EC2 instances across multiple units with each unit having its own AWS account. However, some of the units under-utilize their reserved instances while other units need more reserved instances. As a Cloud Practitioner, which of the following would you recommend as the most cost-optimal solution?_

**Use AWS Organizations to manage AWS accounts of all units and then share the reserved EC2 instances amongst all units**

_Q8: A startup wants to provision an EC2 instance for the lowest possible cost for a long-term duration but needs to make sure that the instance would never be interrupted. As a Cloud Practitioner, which of the following options would you recommend?_

**Reserved Instance**

_Q9: Which of the following S3 storage classes takes the most time to retrieve data (also known as first byte latency)?_

**S3 Glacier Deep Archive**

_Q10: An intern at an IT company provisioned a Linux based On-demand EC2 instance with per-second billing but terminated it within 30 seconds as he wanted to provision another instance type. What is the duration for which the instance would be charged?_

**60 seconds**

> _Note:_  There is a one-minute minimum charge for Linux based EC2 instances, so this is the correct option.

_Q11: A data analytics company is running a proprietary batch analytics application on AWS and wants to use a storage service which would be accessed by hundreds of EC2 instances simultaneously to append data to existing files. As a Cloud Practitioner, which AWS service would you suggest for this use-case?_

**EFS**

> _Note:_ Amazon EFS is a file storage service for use with Amazon EC2. Amazon EFS provides a file system interface, file system access semantics, and concurrently-accessible storage for up to thousands of Amazon EC2 instances. Amazon EFS uses the Network File System protocol.

_Q12: Which AWS Route 53 routing policy would you use to route traffic to multiple resources and also choose how much traffic is routed to each resource?_

**Weighted routing policy**



> _Note_: Amazon Route 53 is a highly available and scalable cloud Domain Name System (DNS) web service. It is designed to give developers and businesses an extremely reliable and cost-effective way to route end users to Internet applications by translating names like www.example.com into the numeric IP addresses like 192.0.2.1 that computers use to connect to each other.
Weighted routing lets you associate multiple resources with a single domain name (example.com) or subdomain name (acme.example.com) and choose how much traffic is routed to each resource. This can be useful for a variety of purposes, including load balancing and testing new versions of software. To configure weighted routing, you create records that have the same name and type for each of your resources. You assign each record a relative weight that corresponds with how much traffic you want to send to each resource. Amazon Route 53 sends traffic to a resource based on the weight that you assign to the record as a proportion of the total weight for all records in the group.

_Q13: Which of the following AWS Support plans provides access to online training with self-paced labs?_

**Enterprise**

_Q14: Due to regulatory and compliance reasons, an organization is supposed to use a hardware device for any data encryption operations in the cloud. Which AWS service can be used to meet this compliance requirement?_

**AWS CloudHSM**

> _Note_: AWS CloudHSM is a cloud-based Hardware Security Module (HSM) that enables you to easily generate and use your encryption keys on the AWS Cloud. With CloudHSM, you can manage your encryption keys using FIPS 140-2 Level 3 validated HSMs. It is a fully-managed service that automates time-consuming administrative tasks for you, such as hardware provisioning, software patching, high-availability, and backups.

_Q15: Which AWS service can be used to review the compliance and governance-related documents on AWS?_


**Artifact**

> _Note_: AWS Artifact is your central resource for compliance-related information on AWS Cloud. It provides on-demand access to AWS’ security and compliance reports and select online agreements. Reports available in AWS Artifact include the Service Organization Control (SOC) reports, Payment Card Industry (PCI) reports, and certifications from accreditation bodies across geographies. Agreements available in AWS Artifact also include the Business Associate Addendum (BAA) and the Nondisclosure Agreement (NDA).

_Q16: A photo sharing web application wants to store thumbnails of user-uploaded images on Amazon S3. The thumbnails are rarely used but need to be immediately accessible from the web application. The thumbnails can be regenerated easily if they are lost. Which is the most cost-effective way to store these thumbnails on S3?_


**Use S3 One-Zone Infrequent Access (One-Zone IA) to store the thumbnails**

_Q17: What is the primary benefit of deploying an RDS database in a Multi-AZ configuration?_

**Multi-AZ enhances database availability**

_Q18: Which service gives a personalized view of the status of the AWS services that are part of your Cloud architecture so that you can quickly assess the impact on your business when AWS service(s) are experiencing issues?_

**AWS Personal Health Dashboard**

> _Note:_ AWS Personal Health Dashboard provides alerts and remediation guidance when AWS is experiencing events that may impact you. With Personal Health Dashboard, alerts are triggered by changes in the health of your AWS resources, giving you event visibility, and guidance to help quickly diagnose and resolve issues.

> _Exam Alert_: While the Service Health Dashboard displays the general status of AWS services, Personal Health Dashboard gives you a personalized view of the performance and availability of the AWS services underlying your AWS resources.

_Q19: An organization deploys its IT infrastructure in a combination of its on-premises data center along with AWS Cloud. How would you categorize this deployment model?_

**Hybrid deployment**

_Q20: Which policy describes prohibited uses of the web services offered by Amazon Web Services?_

**AWS Acceptable Use Policy**


> _Note_: The Acceptable Use Policy describes prohibited uses of the web services offered by Amazon Web Services, Inc. and its affiliates (the “Services”) and the website located at http://aws.amazon.com (the “AWS Site”). This policy is present at https://aws.amazon.com/aup/ and is updated on a need basis by AWS.

> AWS Trusted Advisor - AWS Trusted Advisor is an online tool that provides you real-time guidance to help you provision your resources following AWS best practices on cost optimization, security, fault tolerance, service limits, and performance improvement. Whether establishing new workflows, developing applications, or as part of ongoing improvement, recommendations provided by Trusted Advisor regularly help keep your solutions provisioned optimally. Trusted Advisor does not describe prohibited uses of the web services offered by Amazon Web Services.

_Q21: Which of the following AWS services are always free to use (Select two)?_

- Identity and Access Management (IAM)
- AWS Auto Scaling

_Q22: Which design principle of the AWS Well-Architected Framework can answer the question- "Who did what"?_

**Security**

> _Note:_ "Who did what" is nothing but traceability of action by any user on the system. It tells us which user performed what action on the system. Traceability is part of the Security design principle of AWS Cloud. So this is the correct option.
The Well-Architected Framework has been developed to help cloud architects build secure, high-performing, resilient, and efficient infrastructure for their applications. Based on five pillars — operational excellence, security, reliability, performance efficiency, and cost optimization — the Framework provides a consistent approach for customers and partners to evaluate architectures, and implement designs that will scale over time.


_Q23: Multi AZ (Availability Zone) deployment is an example of which of the following?_

**High Availability**

_Q24: Which of the following AWS services are part of the AWS Foundation services for the Reliability pillar of the Well-Architected Framework in AWS Cloud? (Select two)_

1. **AWS Trusted Advisor**
2. **AWS Service Quotas**

> _Note:_ The services that are part of foundations are: Amazon VPC, AWS Trusted Advisor, AWS Service Quotas (earlier known as AWS Service Limits).

> AWS Trusted Advisor is an online tool that provides you real-time guidance to help you provision your resources following AWS best practices on cost optimization, security, fault tolerance, service limits, and performance improvement. Whether establishing new workflows, developing applications, or as part of ongoing improvement, recommendations provided by Trusted Advisor regularly help keep your solutions provisioned optimally.

> Service Quotas enables you to view and manage your quotas for AWS services from a central location. Quotas, also referred to as limits in AWS, are the maximum values for the resources, actions, and items in your AWS account. Each AWS service defines its quotas and establishes default values for those quotas.

_Q25: Which AWS service helps you define your infrastructure as code?_

**AWS CloudFormation**

> _Note:_ AWS CloudFormation provides a common language to model and provision AWS and third-party application resources in your cloud environment. AWS CloudFormation allows you to use programming languages or a simple text file to model and provision, in an automated and secure manner, all the resources needed for your applications across all Regions and accounts. You can use AWS CloudFormation’s sample templates or create your templates to describe the AWS resources, and any associated dependencies or runtime parameters, required to run your application

_Q26: An IT company wants to run a log backup process every Monday at 2 AM. The usual runtime of the process is 5 minutes. As a Cloud Practitioner, which AWS services would you recommend to build a serverless solution for this use-case? (Select two)_

1. **CloudWatch**
2. **Lambda**

_Q27: Which AWS service can be used to automate code deployment to EC2 instances as well as on-premises instances?_

**AWS CodeDeploy**

> _Note:_ AWS CodeDeploy is a service that automates code deployments to any instance, including Amazon EC2 instances and instances running on-premises. AWS CodeDeploy makes it easier for you to rapidly release new features, helps you avoid downtime during deployment, and handles the complexity of updating your applications. You can use AWS CodeDeploy to automate deployments, eliminating the need for error-prone manual operations, and the service scales with your infrastructure so you can easily deploy to one instance or thousands.

_Q28: An IT company is on a cost-optimization spree and wants to identify all EC2 instances that are under-utilized. Which AWS services can be used to address this use-case? (Select two)_

1. **AWS Cost Explorer**
2. **AWS Trusted Advisor**

> _Note:_ AWS Trusted Advisor is an online tool that provides real-time guidance to help provision your resources following AWS best practices. Whether establishing new workflows, developing applications, or as part of ongoing improvement, recommendations provided by Trusted Advisor regularly help keep your solutions provisioned optimally. AWS Trusted Advisor analyzes your AWS environment and provides best practice recommendations in five categories: Cost Optimization, Performance, Security, Fault Tolerance, Service Limits.
AWS Trusted Advisor checks the Amazon Elastic Compute Cloud (Amazon EC2) instances that were running at any time during the last 14 days and alerts you if the daily CPU utilization was 10% or less and network I/O was 5 MB or less on 4 or more days

> _Note:_ AWS Cost Explorer has an easy-to-use interface that lets you visualize, understand, and manage your AWS costs and usage over time. AWS Cost Explorer includes a default report that helps you visualize the costs and usage associated with your top five cost-accruing AWS services, and gives you a detailed breakdown of all services in the table view. The reports let you adjust the time range to view historical data going back up to twelve months to gain an understanding of your cost trends. The rightsizing recommendations feature in Cost Explorer helps you identify cost-saving opportunities by downsizing or terminating EC2 instances. You can see all of your underutilized EC2 instances across member accounts in a single view to immediately identify how much you can save.

_Q29: Which pillar of the AWS Well-Architected Framework recommends maintaining infrastructure as code?_ 

**Operational Excellence**

> _Note:_ The AWS Well-Architected Framework helps you understand the pros and cons of decisions you make while building systems on AWS. By using the Framework you will learn architectural best practices for designing and operating reliable, secure, efficient, and cost-effective systems in the cloud. It provides a way for you to consistently measure your architectures against best practices and identify areas for improvement.
The AWS Well-Architected Framework is based on five pillars — Operational Excellence, Security, Reliability, Performance Efficiency, and Cost Optimization.
The Operational Excellence pillar includes the ability to run and monitor systems to deliver business value and to continually improve supporting processes and procedures. In the cloud, you can apply the same engineering discipline that you use for application code to your entire environment. You can define your entire workload (applications, infrastructure) as code and update it with code. You can implement your operations procedures as code and automate their execution by triggering them in response to events.

_Q30: A startup runs its proprietary application on docker containers. As a Cloud Practitioner, which AWS service would you recommend so that the startup can run containers and still have access to the underlying servers?_

**Amazon Elastic Container Service (Amazon ECS)**

> _Note:_ Amazon Elastic Container Service (Amazon ECS) - Amazon Elastic Container Service (Amazon ECS) is a highly scalable, fast, container management service that makes it easy to run, stop, and manage Docker containers on a cluster. This is not a fully managed service and you can manage the underlying servers yourself.

_Q31: What is the primary benefit of deploying an RDS database in a Read Replica configuration?_

**Read Replica improves database scalability**

_Q32: An IT company has a hybrid cloud architecture and it wants to centralize the server logs for its EC2 instances and on-premises servers. Which of the following is the MOST effective for this use-case?_

**Use CloudWatch Logs for both the EC2 instance and the on-premises servers**

> _Note:_ You can use Amazon CloudWatch Logs to monitor, store, and access your log files from Amazon Elastic Compute Cloud (Amazon EC2) instances, AWS CloudTrail, Route 53, and other sources such as on-premises servers.
CloudWatch Logs enables you to centralize the logs from all of your systems, applications, and AWS services that you use, in a single, highly scalable service. You can then easily view them, search them for specific error codes or patterns, filter them based on specific fields, or archive them securely for future analysis.

_Q33: Which of the following AWS services offer block-level storage? (Select two)_

1. **EBS**
2. **Instance Store**

> _Note:_ EBS - Amazon Elastic Block Store (EBS) is an easy to use, high-performance block storage service designed for use with Amazon Elastic Compute Cloud (EC2) for both throughput and transaction-intensive workloads at any scale. A broad range of workloads, such as relational and non-relational databases, enterprise applications, containerized applications, big data analytics engines, file systems, and media workflows are widely deployed on Amazon EBS.

> Instance Store - An instance store provides temporary block-level storage for your EC2 instance. This storage is located on disks that are physically attached to the host computer. Instance store is ideal for the temporary storage of information that changes frequently, such as buffers, caches, scratch data, and other temporary content, or for data that is replicated across a fleet of instances, such as a load-balanced pool of web servers. Instance storage is temporary, data is lost if instance experiences failure or is terminated. EC2 instance store cannot be used for file sharing between instances.

_Q34: An AWS user is trying to launch an EC2 instance in a given region. What is the region-specific constraint that the Amazon Machine Image (AMI) must meet so that it can be used for this EC2 instance?_

**You must use an AMI from the same region as that of the EC2 instance. The region of the AMI has no bearing on the performance of the EC2 instance**

> _Note:_ An Amazon Machine Image (AMI) provides the information required to launch an instance. You must specify an AMI when you launch an instance. You can launch multiple instances from a single AMI when you need multiple instances with the same configuration.

> The AMI must be in the same region as that of the EC2 instance to be launched. If the AMI exists in a different region, you can copy that AMI to the region where you want to launch the EC2 instance. The region of AMI has no bearing on the performance of the EC2 instance.

_Q35: A medical device company is looking for a durable and cost-effective way of storing their historic data. Due to compliance requirements, the data must be stored for 10 years. Which AWS Storage solution will you suggest?_

**S3 Glacier Deep Archive**

> S3 Glacier Deep Archive is Amazon S3’s lowest-cost storage class and supports long-term retention and digital preservation for data that may be accessed once or twice in a year. It is designed for customers — particularly those in highly-regulated industries, such as the Financial Services, Healthcare, and Public Sectors — that retain data sets for 7-10 years or longer to meet regulatory compliance requirements. S3 Glacier Deep Archive can also be used for backup and disaster recovery use cases. It has a retrieval time (first byte latency) of 12 to 48 hours.

_Q36: A financial services enterprise plans to enable Multi-Factor Authentication (MFA) for its employees. For ease of travel, they prefer not to use any physical devices to implement MFA. Which of the below options is best suited for this use case?_

**Virtual MFA device**

> A software app that runs on a phone or other device and emulates a physical device. The device generates a six-digit numeric code based upon a time-synchronized one-time password algorithm. The user must type a valid code from the device on a second webpage during sign-in. Each virtual MFA device assigned to a user must be unique. A user cannot type a code from another user's virtual MFA device to authenticate.

_Q37: A cyber-security agency uses AWS Cloud and wants to carry out security assessments on their own AWS infrastructure without any prior approval from AWS. Which of the following describes/facilitates this practice?_

**Penetration Testing**

> AWS customers can carry out security assessments or penetration tests against their AWS infrastructure without prior approval for few common AWS services. Customers are not permitted to conduct any security assessments of AWS infrastructure, or the AWS services themselves

_Q38: Which of the following are correct statements regarding the AWS Shared Responsibility Model? (Select two)_

1. **AWS is responsible for Security "of" the Cloud**
2. **For abstracted services like Amazon S3, AWS operates the infrastructure layer, the operating system, and platforms**

_Q39: Data encryption is automatically enabled for which of the following AWS services? (Select two)?_ 

1. **Amazon S3 Glacier**
2. **AWS Storage Gateway**

> Amazon S3 Glacier - Amazon S3 Glacier (S3 Glacier), is a storage service optimized for infrequently used data, or "cold data. Data at rest stored in S3 Glacier is automatically server-side encrypted using 256-bit Advanced Encryption Standard (AES-256) with keys maintained by AWS.

> AWS Storage Gateway - AWS Storage Gateway is a hybrid cloud storage service that gives you on-premises access to virtually unlimited cloud storage. All data transferred between the gateway and AWS storage is encrypted using SSL (for all three types of gateways - File, Volume and Tape Gateways).

_Q40: AWS Marketplace facilitates which of the following use-cases? (Select two)_

1. **Sell Software as a Service (SaaS) solutions to AWS customers**
2. **AWS customer can buy software that has been bundled into customized AMIs by the AWS Marketplace sellers**

_Q41: A financial services company wants to migrate from its on-premises data center to AWS Cloud. As a Cloud Practitioner, which AWS service would you recommend so that the company can compare the cost of running their IT infrastructure on-premises vs AWS Cloud?_

**AWS Total Cost of Ownership (TCO) Calculator**

> TCO calculator helps to compare the cost of your applications in an on-premises or traditional hosting environment to AWS. AWS helps reduce Total Cost of Ownership (TCO) by reducing the need to invest in large capital expenditures and providing a pay-as-you-go model that empowers to invest in the capacity you need and use it only when the business requires it. Once you describe your on-premises or hosting environment configuration, it produces a detailed cost comparison with AWS. TCO calculator can be used from https://awstcocalculator.com/.

_Q42: Which AWS service can help you analyze your infrastructure to identify unattached or underutilized EBS volumes?_

**AWS Trusted Advisor**

> AWS Trusted Advisor is an online tool that provides real-time guidance to help provision your resources following AWS best practices. Whether establishing new workflows, developing applications, or as part of ongoing improvement, recommendations provided by Trusted Advisor regularly help keep your solutions provisioned optimally. AWS Trusted Advisor analyzes your AWS environment and provides best practice recommendations in five categories: Cost Optimization, Performance, Security, Fault Tolerance, Service Limits.

> AWS Trusted Advisor can check Amazon Elastic Block Store (Amazon EBS) volume configurations and warns when volumes appear to be underused. Charges begin when a volume is created. If a volume remains unattached or has very low write activity (excluding boot volumes) for a period of time, the volume is probably not being used

_Q43: Which AWS service will you use to provision the same AWS infrastructure across multiple AWS accounts and regions?_

**AWS CloudFormation**

> AWS CloudFormation allows you to use programming languages or a simple text file to model and provision, in an automated and secure manner, all the resources needed for your applications across all Regions and accounts. A stack is a collection of AWS resources that you can manage as a single unit. In other words, you can create, update, or delete a collection of resources by creating, updating, or deleting stacks.

> AWS CloudFormation StackSets extends the functionality of stacks by enabling you to create, update, or delete stacks across multiple accounts and regions with a single operation. Using an administrator account, you define and manage an AWS CloudFormation template, and use the template as the basis for provisioning stacks into selected target accounts across specified regions.

_Q44: An organization maintains a separate Virtual Private Cloud (VPC) for each of its business units. Two units need to privately share data. Which is the most optimal way of privately sharing data between the two VPCs?_

**VPC Peering**

> A VPC peering connection is a networking connection between two VPCs that enables you to route traffic between them privately. Instances in either VPC can communicate with each other as if they are within the same network. You can create a VPC peering connection between your VPCs, with a VPC in another AWS account, or with a VPC in a different AWS Region

_Q45: Which benefit of Cloud Computing allows AWS to offer lower pay-as-you-go prices as usage from hundreds of thousands of customers is aggregated in the cloud?_

**Massive economies of scale**

> Cloud computing is the on-demand delivery of IT resources over the Internet with pay-as-you-go pricing. Instead of buying, owning, and maintaining physical data centers and servers, you can access technology services, such as computing power, storage, and databases, on an as-needed basis.
By using cloud computing, you can achieve a lower variable cost than you can get on your own. Because usage from hundreds of thousands of customers is aggregated in the cloud, providers such as AWS can achieve higher economies of scale, which translates into lower pay-as-you-go prices

_46: Which of the following are the serverless computing services offered by AWS (Select two)_

1. **AWS Lambda**
2. **AWS Fargate**

_Q47: Which of the following AWS services can be used to forecast your AWS account usage and costs?_

**AWS Cost Explorer**

> AWS Cost Explorer has an easy-to-use interface that lets you visualize, understand, and manage your AWS costs and usage over time. AWS Cost Explorer includes a default report that helps you visualize the costs and usage associated with your top five cost-accruing AWS services, and gives you a detailed breakdown of all services in the table view. The reports let you adjust the time range to view historical data going back up to twelve months to gain an understanding of your cost trends. AWS Cost Explorer also supports forecasting to get a better idea of what your costs and usage may look like in the future so that you can plan

_Q48: Which of the following is a container service of AWS?_

**AWS Fargate**

> AWS Fargate is a serverless compute engine for containers that works with both Amazon Elastic Container Service (ECS) and Amazon Elastic Kubernetes Service (EKS). Fargate makes it easy for you to focus on building your applications. Fargate removes the need to provision and manage servers, lets you specify and pay for resources per application, and improves security through application isolation by design.

_Q49: Which of the following AWS authentication mechanisms supports a Multi-Factor Authentication (MFA) device that you can plug into a USB port on your computer?_

**U2F security key**

> Universal 2nd Factor (U2F) Security Key is a device that you can plug into a USB port on your computer. U2F is an open authentication standard hosted by the FIDO Alliance. When you enable a U2F security key, you sign in by entering your credentials and then tapping the device instead of manually entering a code

1. **Volume discounts for Amazon EC2 and Amazon S3 aggregated across the member AWS accounts**
2. **Share the reserved EC2 instances amongst the member AWS accounts**

_Q50: Which AWS service would you choose for a data processing project to store unstructured data?_

**Amazon DynamoDB**

> Amazon DynamoDB is a key-value and document database that delivers single-digit millisecond performance at any scale. It's a fully managed, multi-Region, multi-master, durable database with built-in security, backup and restore, and in-memory caching for internet-scale applications. DynamoDB offers flexible schema and can easily handle unstructured data.

_Q51: Which entity ensures that your application on Amazon EC2 always has the right amount of capacity to handle the current traffic demand?_

**Auto Scaling**

> Auto Scaling helps you ensure that you have the correct number of Amazon EC2 instances available to handle the load for your application. You create collections of EC2 instances, called Auto Scaling groups. You can specify the minimum number of instances in each Auto Scaling group, and Amazon EC2 Auto Scaling ensures that your group never goes below this size.

_Q52: Which of the following statements is the MOST accurate when describing AWS Elastic Beanstalk?_

**It is a Platform as a Service (PaaS) which allows you to deploy and scale web applications and services**

> AWS Elastic Beanstalk makes it even easier for developers to quickly deploy and manage applications in the AWS Cloud. Developers simply upload their application, and Elastic Beanstalk automatically handles the deployment details of capacity provisioning, load balancing, auto-scaling, and application health monitoring.

_54: Which of the following options are the benefits of using AWS Elastic Load Balancing (ELB)? (Select TWO)_

1. **High availability**
2. **Fault tolerance**

> Elastic Load Balancing (ELB) automatically distributes incoming application traffic across multiple targets, such as Amazon EC2 instances, containers, and IP addresses. It can handle the varying load of your application traffic in a single Availability Zone or across multiple Availability Zones.

> Elastic Load Balancing offers three types of load balancers that all feature the high availability, automatic scaling, and robust security necessary to make your applications fault-tolerant: Application Load Balancer (best suited for HTTP and HTTPS traffic), Network Load Balancer (best suited for TCP traffic), and Classic Load Balancer.

_Q55: Which AWS service can be used to subscribe to an RSS feed to be notified of the status of all AWS service interruptions?_

**AWS Service Health Dashboard**

> AWS Service Health Dashboard publishes most up-to-the-minute information on the status and availability of all AWS services in tabular form for all Regions that AWS is present in. You can check on this page https://status.aws.amazon.com/ to get current status information.

> AWS Service Health Dashboard offers the possibility to subscribe to an RSS feed to be notified of interruptions to each service

_56: A developer would like to automate operations on his on-premises environment using Chef and Puppet. Which AWS service can help with this task?_

**AWS OpsWorks**

> AWS OpsWorks is a configuration management service that provides managed instances of Chef and Puppet. Chef and Puppet are automation platforms that allow you to use code to automate the configurations of your servers. OpsWorks lets you use Chef and Puppet to automate how servers are configured, deployed, and managed across your Amazon EC2 instances or on-premises compute environments.

_Q57: Which of the following are the best practices when using AWS Organizations? (Select TWO)_

1. **Create accounts per department**
2. **Restrict account privileges using Service Control Policies (SCP)**

> AWS Organizations helps you centrally govern your environment as you grow and scale your workloads on AWS. Whether you are a growing startup or a large enterprise, Organizations helps you to centrally manage billing; control access, compliance, and security; and share resources across your AWS accounts.

> Using AWS Organizations, you can automate account creation, create groups of accounts to reflect your business needs, and apply policies for these groups for governance. You can also simplify billing by setting up a single payment method for all of your AWS accounts. Through integrations with other AWS services, you can use Organizations to define central configurations and resource sharing across accounts in your organization. AWS Organizations is available to all AWS customers at no additional charge.

> You should create accounts per department based on regulatory restrictions (using SCP) for better resource isolation, and to have separate per-account service limits.

> AWS Organizations allows you to restrict what services and actions are allowed in your accounts. You can use Service Control Policies (SCPs) to apply permission guardrails on AWS Identity and Access Management (IAM) users and roles

_Q58: A Cloud Practitioner would like to get operational insights of its resources to quickly identify any issues that might impact applications using those resources. Which AWS service can help with this task?_

**AWS Systems Manager**

> AWS Systems Manager allows you to centralize operational data from multiple AWS services and automate tasks across your AWS resources. You can create logical groups of resources such as applications, different layers of an application stack, or production versus development environments.

> With Systems Manager, you can select a resource group and view its recent API activity, resource configuration changes, related notifications, operational alerts, software inventory, and patch compliance status. You can also take action on each resource group depending on your operational needs. Systems Manager provides a central place to view and manage your AWS resources, so you can have complete visibility and control over your operations.


_Q59: Which of the following options are features of Amazon Inspector?_

1. **Automate security assessments**
2. **Analyze against unintended network accessibility**
3. **Inspect running operating systems (OS) against known vulnerabilities**

_Q60: A Cloud Practitioner would like to deploy identical resources across all regions and accounts using templates while estimating costs. Which AWS service can assist with this task?_

**AWS CloudFormation**

_Q60: A corporation would like to have a central user portal to log in to third-party business applications as well as accounts managed under AWS Organizations. As a Cloud Practitioner, which AWS service would you use for this task?_

**AWS Single Sign-On (SSO)**

> AWS SSO is an AWS service that enables you to makes it easy to centrally manage access to multiple AWS accounts and business applications and provide users with single sign-on access to all their assigned accounts and applications from one place.

> With AWS SSO, you can easily manage SSO access and user permissions to all of your accounts in AWS Organizations centrally. AWS SSO allows you to create and manage user identities in AWS SSO’s identity store, or easily connect to your existing identity source including Microsoft Active Directory, Azure Active Directory (Azure AD), and Okta Universal Directory.

> You can use AWS SSO to quickly and easily assign and manage your employees’ access to multiple AWS accounts, SAML-enabled cloud applications (such as Salesforce, Office 365, and Box), and custom-built in-house applications, all from a central place.

_Q62: A company would like to separate cost for AWS services by the department for cost allocation. Which of the following is the simplest way to achieve this task?_

**Create tags for each department**

> You can assign metadata to your AWS resources in the form of tags. Each tag is a label consisting of a user-defined key and value. Tags can help you manage, identify, organize, search for, and filter resources. You can create tags to categorize resources by purpose, owner, environment, or other criteria.

> Typically, you use business tags such as cost center/business unit, customer, or project to associate AWS costs with traditional cost-allocation dimensions. But a cost allocation report can include any tag. This lets you associate costs with technical or security dimensions, such as specific applications, environments, or compliance programs.

_Q63: Which of the following are advantages of using the AWS Cloud? (Select TWO)_

1. **Increase speed and agility**
2. **Stop guessing about capacity**

_Q64: A company would like to optimize Amazon EC2 costs. Which of the following actions can help with this task? (Select TWO)_

1. Set up Auto Scaling groups to align the number of instances with demand
2. Purchase EC2 Reserved instances

_Q65: A start-up would like to quickly deploy a popular technology on AWS. As a Cloud Practitioner, which AWS tool would you use for this task?_

**AWS Quick Starts references**

> Quick Starts are built by AWS solutions architects and partners to help you deploy popular technologies on AWS, based on AWS best practices for security and high availability. These accelerators reduce hundreds of manual procedures into just a few steps, so you can build your production environment quickly and start using it immediately.

> Each Quick Start includes AWS CloudFormation templates that automate the deployment and a guide that discusses the architecture and provides step-by-step deployment instructions