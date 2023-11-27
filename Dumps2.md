_Q1: You need to set up a data warehouse on AWS for financial/actuary data. Which AWS service will you use?_

**Redshift**

> Redshift is a scalable data warehouse solution

_Q2: Which of the following best describes EBS?_

**A virtual hard disk in the cloud**

> An EBS volume is best described as a virtual hard disk in the cloud - storage that, for all intents and purposes, appears to be directly attached to your instance. These are used by the virtual server instances in the cloud, which are known as EC2 instances.

_Q3: When you access your personal email through a web browser using an application like Gmail, which cloud computing model are you using?_

**Software as a Service (SaaS)**

> SaaS allows you to use a complete application on demand. When you access your personal email through a web browser, you're using SaaS

_Q4: Which of the following are AWS compute services?_
(Choose 2)

EC2, Lambda

_Q5: How can a customer meet corporate, contractual, and regulatory compliance requirements for data security by using dedicated hardware in the cloud?_

**CloudHSM**

> CloudHSM allows customers to meet compliance requirements for data security by using dedicated hardware

_Q6: A development team has created a large amount of CloudFormation templates in the JSON format. Which AWS database would be best suited for storing these documents?_

**Amazon DocumentDB**

> Amazon DocumentDB (with MongoDB compatibility) is a fast, scalable, highly available, and fully managed document database service that supports MongoDB workloads. As a document database, Amazon DocumentDB makes it easy to store, query, and index JSON data

Question 7

_Which of the following are focuses of the cost optimization pillar of the Well-Architected Framework?_
(Choose 3)

1. **Implement cloud financial management**
2. **Measure overall efficiency**
3. **Utilize consumption-based pricing**

_Q8: Which of the following are compute services?_

**Elastic Beanstalk**, **Lambda**, **EC2**

_Q9: A solutions architect is designing a new web application to be highly available. There are regulatory requirements that require multiple EC2 instances to be provisioned in the same geographic location. Where should the EC2 instances be placed?_

**Multiple Availability Zones**


_Q10: You have a project that will require 90 hours of computing time. There is no deadline, and the work can be stopped and restarted without adverse effect. Which of the following computing options offers the most cost-effective solution?_

**Spot Instances**

> Spot Instances are usually the most cost-effective solution for workloads that can be interrupted. On-Demand and Reserved Instances are both more expensive in this use case, and Custom Instances do not exist.

_Q11: When you pay a subscription fee to a hosting company to serve your website on an instance you manage, which cloud computing model are you using?_

**Infrastructure as a Service (IaaS)**

> IaaS offers building blocks that can be rented. When you pay a web hosting fee, you're using IaaS



_Q12: An IAM user with administrative access is attempting to close the AWS account. After troubleshooting, the admin user uncovers they need to sign in with root user credentials in order to perform this task. What other tasks require root user credentials?_
(Choose 3)

**Changing the email address associated with the account**
> This task can only be performed when you sign in as the root user of an account. AWS Documentation: Tasks that require root user credentials.

**Configuring an Amazon S3 bucket to enable MFA (multi-factor authentication)**

> This task can only be performed when you sign in as the root user of an account. This task was presented in the additional reading, "Tasks that require root user credentials," provided with the lesson. AWS Documentation: Tasks that require root user credentials.

**Activate IAM access to the Billing and Cost Management console**
> This task can only be performed when you sign in as the root user of an account. This task was presented in the additional reading, "Tasks that require root user credentials", provided with the lesson. AWS Documentation: Tasks that require root user credentials.

_Q13: Which of the following scenarios are examples of scaling an IT architecture vertically?_
(Choose 2)

1. **Resizing an EC2 instance type from a1.medium to a1.xlarge for more CPU and memory power**
2. **Resizing an RDS instance type from db.r5.large to db.r5.2xlarge**

_Q14: You need to run your code, but you don’t want to worry about provisioning or managing servers. Which of the following AWS services would you choose?_

Lambda


_Q15: A small startup is configuring its AWS Cloud environment. Which AWS service will allow grouping these users together and applying permissions to them as a group?_

**AWS IAM**

_Q16: A gaming company is using the AWS Developer Tools suite to develop, build, and deploy their applications. Which AWS service can be used to trace user requests from end to end through the application?_

**AWS X-Ray**

> AWS X-Ray provides an end-to-end view of requests as they travel through your application, and shows a map of your application’s underlying components. You can use X-Ray to analyze from simple three-tier applications to complex microservices applications consisting of thousands of services

_Q17: Which of the below is correct when looking at Regions, Availability Zones, edge locations, and data centers?_
(Choose 2)

1. Regions contain Availability Zones
2. Availability Zones contain data centers



_Q18: For which services is DDoS protection via AWS Shield Advanced supported?_
(Choose 3)

- **Elastic Load Balancing**
- **CloudFront**
- **Route 53**



_Q19: Which pillar of the Well-Architected Framework encourages performing operations as code (for example, encouraging the use of services such as CloudFormation) as one of its design principles?_

**Operational excellence**

> Operational excellence focuses on creating applications that effectively support production workloads. Scripting operations as code is part of this pillar, which includes the use of CloudFormation



_Q20: Which AWS service is specifically designed to assist you in processing large datasets?_

**EMR**

> EMR is a service that makes it easy to process large amounts of data efficiently.

_Q21: Which of the following best describes a system that will remain operational even in the event of a component failure?_

**Fault tolerant**

> A fault-tolerant system will remain operational even in the event of a component failure. Reliability Pillar - AWS Well-Architected Framework



_Q22: A developer has developed a 3-tier web application that will be deployed directly on Amazon EC2. The developer is considering deploying the application to more than one Availability Zone. What advantages does this deployment approach offer?_
(Choose 3)

- **Increase in responsiveness when load balancing is used**
- **Enhances resiliency, allowing the application to recover from failure due to load**
- **Improves the availability of the application**



_Q23: Which of the following statements is true of AWS Regions?_
(Choose 2)

- They are independent geographical areas
- They are composed of Availability Zones



_Q24: Which types of deployments offer high availability?_
(Choose 2)

1. Multi-AZ deployments
2. Multi-Region deployments

_Q:25 A person new to the cloud is learning about the services that offer compute power. Which AWS services offer computing resources in the cloud?_
(Choose 3)

1. **AWS Lambda**
2. **Amazon Elastic Compute Cloud (EC2)**
3. **AWS Elastic Beanstalk**

> Lambda is a serverless compute service that lets you run code without managing servers.

> EC2 allows you to rent and manage virtual servers in the cloud.

> Elastic Beanstalk allows you to deploy your web applications and web services to AWS. Although we covered Elastic Beanstalk in the "Deployment and Infrastructure Management Services" lesson, it is a compute service.



_Q26: Several EC2 instances in a public subnet need internet access. Which will you configure as 1 step in granting internet access?_

**Internet gateway**

> An internet gateway allows public traffic to the internet from a VPC

> The NAT gateway resides in a public subnet, but it helps to provide internet access to instances in private subnets

Question 27

_A company is considering migrating to the cloud. How does moving to the cloud reduce upfront costs?_

**By replacing large capital expenditures with lower variable costs spread over time**

> The cloud allows you to trade capital expenses for variable expenses

Question 28

_You have decided to use the AWS Cost and Usage Report to track your EC2 Reserved Instance costs. Which AWS service can be used to store AWS Cost and Usage report files?_

**An S3 bucket you own**

> You can use Cost and Usage Reports to publish your AWS billing reports to an S3 bucket you own. AWS updates the report in your bucket once a day in comma-separated value (CSV) format. You can view the reports using spreadsheet software or access them from an application using the Amazon S3 API

_Q29: You have been tasked to create an S3 bucket for storing templates. A team member has forwarded you the templates, which are used for creating multiple different AWS resources such as S3 buckets, EC2 instances, and VPCs. Which service uses these templates to create AWS resources?_

**CloudFormation**

> CloudFormation allows you to provision AWS resources using Infrastructure as Code (IaC) and reusable templates

_Q30: Which of the below are you responsible for managing when storing data in S3?_
(Choose 2)

- **Who has access to data you stored on the S3 service**
- **Who has access to the S3 service**



_Q31: Which of the following statements are true regarding AWS Reserved Instances?_
(Choose 3)

1. **Reserved Instances usually have contract terms of one or three years. The longer the term, the higher the savings**

> Reserved Instances usually have contract terms of one or three years. Standard RIs provide the biggest discount for a designated instance type over a long-term contract. Convertible RIs provide a smaller discount but let you change the instance type

2. **Reserved Instances are available in all up-front, partial up-front, or no upfront payments.**

> Reserved Instances are available in all up-front (AURI), partial up-front (PURI), or no upfront payments (NURI). The more you pay up-front, the higher the savings

3. **Reserved Instances act as a discount on new or existing On-Demand Instances.**

> Reserved Instances act as a discount on new or existing On-Demand Instances. The discount is applied when you launch an instance with the required specifications.


_Q:32 Which of the following is NOT part of the AWS Global infrastructure?_

**Security groups**

_Q33: You have infrequently accessed data in S3 buckets that you want to transfer to Glacier. What can you use in AWS to do this?_

**S3 Lifecycle policy**

> You can add rules in an S3 Lifecycle configuration to tell Amazon S3 to transition objects to another Amazon S3 storage class. For example: When you know objects are infrequently accessed, you might transition them to the S3 Standard-IA storage class. You might want to archive objects that you don't need to access in real time to the S3 Glacier storage class.

_Q34: You need a "virtual hard disk" for your EC2 instance. Which of the following should you choose?_

**EBS**

> EBS volumes are "virtual hard disks" for your EC2 instance

_Q35: When you access tools provided to build a storefront application that runs on another company’s server, which cloud computing model are you using?_

**Platform as a Service (PaaS)**

> PaaS is often used by developers to develop software using web-based tools

_Q36: Scientists would like to analyze terabytes of scientific data from a rover that landed on Mars. Which service will help them find trends and understand the vast amount of data using Hadoop?_

**Elastic MapReduce (EMR)**

> EMR helps you process large amounts of data using big data frameworks like Hadoop

_Q37: You need a paid AWS Support plan for your production workloads but want to keep costs to a minimum. Which of the following plans should you choose?_

**Business**

> The Business Support plan is specifically designed for production workloads in AWS


_Q38: You would like to give an application running on one of your EC2 instances access to an S3 bucket. What is the best way to implement this?_

**Assign the instance an IAM role**

> The recommended method to assign permissions to apps running in EC2 is to use IAM roles.

_Q39: A software company is looking for a tool to automate their release process from end to end. Which AWS service can provide this continuous delivery functionality?_

**CodePipeline**

> CodePipeline automates the software release process

_Q40: Which of the following AWS services allows you to run complex analytic queries against petabytes of structured data, use sophisticated query optimization, has columnar storage on high-performance local disks, and has massively parallel query execution?_

**Redshift**

> Redshift allows you to run complex analytic queries against petabytes of structured data, using sophisticated query optimization, columnar storage on high-performance local disks, and massively parallel query execution.

_Q41: A company is looking to lower its total cost of ownership (TCO) by moving the file system used for its business-critical, Linux-based applications to a managed file system in the cloud. Which service meets their needs?_

**Elastic File System (EFS)**

> EFS is a fully managed file system that provides elastic file storage for a broad range of Linux-based applications

_Q42: What is the recommended way to give your applications running in EC2 permission to other AWS resources?_

**Create an IAM role with appropriate permissions and assign it to the instance.**

> You should use IAM roles wherever possible to enable applications running on EC2 instances to access other AWS resources. This is the most secure method to do so

_Q43: A company ingests data to S3 using Kinesis. What is the easiest way for the company to run ad hoc SQL queries against the data in S3 without the need to manage servers?_

**Use Athena**

> Athena allows the company to query data in S3 using standard SQL.

_Q44: Which of the following AWS Support levels offers 24x7 support via phone or chat?_

**Business**

> The Business and Enterprise support plans, the two most expensive plans, offer 24 X 7 support via phone or chat

_Q45: Which of the following is a shared control of the AWS shared responsibility model?_

**Patch management**

> Shared controls are elements of the shared responsibility model where both AWS and the customer have shared responsibilities within their own contexts. Patch management is a shared control, since AWS is responsible for patching and fixing flaws within the infrastructure, including managed services like RDS, but customers are responsible for patching their guest OS and applications. https://aws.amazon.com/compliance/shared-responsibility-model/


_Q46: Which of the following are support levels offered by AWS?_
(Choose 3)

**Developer**, **Basic**, **Business**


_Q47: A company wants to build a customer identity graph to provide a single unified view of customers and prospects by linking identifiers like website browsing history, preferences, and more. Which database product allows the customer to store and navigate billions of interconnected relationships?_

**Neptune**

> Neptune is a fully managed graph database that supports highly connected datasets.

_Q48: You are an AWS Enterprise customer with questions about billing and your overall AWS account. Which of the following AWS Support personnel should you contact?_

**AWS Concierge**

> For AWS Enterprise customers, the AWS Concierge is a resource dedicated to answering billing and account questions



_Q49: A company would like to call AWS support to open cases when issues arise. What's the minimum support plan they need to subscribe to in order to have telephone access?_

**Business Support**

_Q50: You are gathering information to present to management on a potential move to the AWS Cloud. Can you identify advantages of cloud computing?_
(Choose 2)

1. **Increase speed and agility**
2. **Trade capital expense for variable expense**

_Q51: Which AWS service allows the deployment of resources in code templates, otherwise known as Infrastructure as Code?_

CloudFormation

_Q52: Which of the following are criteria affecting your billing for RDS?_
(Choose 3)

- **Running duration of the RDS instances**
- **Additional storage**
- **Internet data transfer**

_Q53: As an AWS account administrator, you are in charge of creating AWS accounts and securing those accounts. What steps can you take?_
(Choose 2)

- **Add IP restrictions for all accounts**
- **Create multi-factor authentication for the root account**



_Q54: You need to purchase Reserved Instances for a 3-year project. But a company initiative may change all the company compute operating systems from Windows to Linux midway through this project. What type of Reserved Instance should you purchase?_

**Convertible**

> These can be exchanged during the term for another Convertible Reserved Instance with new attributes, including instance family, instance type, platform, scope, or tenancy

_Q55: You are setting up an S3 bucket to host a public website. You have uploaded the files for your website to S3, but when clicking on the object URL of the file to verify it can be seen, you receive the message, "access denied". You have tried making the file public but the option is not available. What configuration has been missed?_

**Removing "Block Public Access" from the bucket.**

> To enable the option for selecting an object to be public you first need to disable the Block Public Access setting on the S3 bucket. This setting is in place to prevent accidental configuration of the S3 bucket and objects being visible from anywhere on the internet



_Q56: You need to track your AWS costs on a detailed level. Which tool will allow you to do this?_

**Cost Allocation Tags**

> A tag is a label that you or AWS assign to an AWS resource. Each tag consists of a key and a value. Tagged resources can appear on the Cost Explorer or on a cost allocation report

_Q57: What does a developer need in order to log in to an EC2 instance via SSH from their local machine?_
(Choose 2)

1. **Private key**
2. **SSH client**


_Q58: There are several options for interacting with and accessing resources in your AWS account. Which of the following are ways to interact with AWS services?_
(Choose 3)

1. **AWS Command Line Interface (CLI)**
2. **AWS Management Console**
3. **Software Development Kit (SDK)**



_Q59: Which of the following are programmatic access types enabling users to interact with AWS services?_
(Choose 3)

1. **AWS SDKs**
2. **AWS CLI**
3. **API calls**

_Q60: In the AWS Global Infrastructure, what are edge locations responsible for?_

**Hosting a content delivery network called CloudFront**

_Q61: A development team wants to gain full observability into the health of their applications and instances in order to provide the best service level to users of their applications. Which services can help them monitor the health of their applications and instances?_
(Choose 3)

**Elastic Load Balancing**

> Load balancers monitor the health of EC2 instances and route the traffic to only instances that are in a healthy state.

**Elastic Beanstalk**

> Elastic Beanstalk monitors application health via a health dashboard.

**Route 53**

> Route 53 can be used to configure DNS health checks to route traffic to healthy endpoints or to monitor the health of your applications


_Q62: You are currently running an application in a production environment, but you want to ensure that it is free of vulnerabilities. Which of the following AWS services would you need to use?_

**Amazon Inspector**

> You will need to turn to Amazon Inspector for security assessment. Not only does it identify vulnerabilities in your application, it will also spot deviations from security best practices. AWS Shield and WAF protect the application from attacks that exploit vulnerabilities, rather than identify them. Trusted Advisor only provides recommendations on how to improve security


_Q63: You are storing sensitive employee information in an S3 bucket. What can you use to give bucket access only to authorized personnel?_

**Bucket policy**

> S3 bucket policies allow you to grant permissions to your S3 resources

_Q64: A company wants to deploy applications entirely on a serverless platform. Which AWS service can they use to build their applications without worrying about managing servers?_

**AWS Lambda**


_Q65: According to the Shared Responsibility Model, which of the following is AWS responsible for?_
(Choose 2)

1. Elastic Cloud Compute **(EC2) infrastructure**
2. Amazon **Virtual Private Cloud infrastructure**




## Dump 5

Question 1

A company has developed a new web application that uses Amazon RDS MySQL as the backend database. The company wants to ensure the application is highly available. Which feature of RDS can ensure high availability?

**Using Multi-AZ deployment**

> RDS provides high availability and failover support for databases when using Multi-AZ deployments.


Question 2

VMware Cloud on AWS allows companies to migrate and extend their on-premises VMware vSphere-based environments to AWS Cloud using Amazon EC2. Which of the following choices accurately classifies this deployment model?

**Hybrid**

> Hybrid deployments connect infrastructure and applications between cloud-based resources and existing resources that are not located in the cloud. VMware Cloud on AWS is an example of a hybrid deployment, since it involves the on-premises environments of VMware and the cloud-based services of AWS.

Question 3

Which of the following are advantages of cloud computing?
(Choose 3)

- You can stop guessing capacity.
- You can increase speed and agility
- You can go global in minutes

Question 4

Which services can host a MariaDB database?
(Choose 2)

**EC2, RDS**

> RDS supports several popular database engines: Amazon Aurora, PostgreSQL, MySQL, MariaDB, Oracle Database, and SQL Server.

Question 5

After configuring your VPC and all of the resources within it, you want to add an extra layer of security at the **subnet level**. Which will you use to add this security?

**Network ACL**

> A network access control list (NACL) is an optional layer of security for your VPC that ensures the proper traffic is allowed into the subnet

Question 6

Which of the following is correct regarding the number of Regions, Availability Zones, edge locations, and data centers?

**There are more edge locations than Availability Zones**

Question 7

What is the most efficient intelligent threat detection service that can be used to analyze malicious or unauthorized activity and continuously monitor CloudTrail event logs, Amazon VPC Flow Logs, and DNS logs?

**Amazon GuardDuty**
> GuardDuty is an intelligent threat detection system that uncovers malicious or unauthorized activity.

Question 8

You are creating a few IAM policies. This is the first time you have worked with IAM policies. Which tool can you use to test IAM policies?

**IAM policy simulator**

> The IAM policy simulator allows you to test and troubleshoot identity-based policies, IAM permissions boundaries, service control policies (SCPs), and resource-based policies

Question 9

Which factors are required to sign in to the AWS Management Console using multi-factor authentication (MFA)?

**Username and password + authentication code**

Question 10

You need to use an AWS service to assess software vulnerabilities and unintended network exposure of your Amazon EC2 instances. Which of the following services should you use?

**Amazon Inspector**

> Amazon Inspector is an automated vulnerability management service that continually scans Amazon Elastic Compute Cloud (EC2) and container workloads for software vulnerabilities and unintended network exposure.

Question 11

Which of the following services are available **24x7 for all AWS Support plans**?
(Choose 3)
- **Customer service**
- **Storage costs**
- **Data transfer costs**


Question 12

Which of the following is AWS responsible for in the Shared Responsibility Model?
(Choose 3)
- Availability Zones
- Edge locations
- Regions

Question 13

AWS Trusted Advisor provides checks and recommended actions. Which of the following is not one of those checks?

**Checks to determine if an administrative user is used instead of the root account**

> This is not a check provided in Trusted Advisor.


Question 14

A new application needs temporary access to resources in AWS. How can this best be achieved?

**Create an IAM role and have the application assume the role.**

> Roles define access permissions and are temporarily assumed by an IAM user or service.

Question 15

Which of the following can be used as a web-based interface to access and manage the AWS cloud?

**AWS Management Console**

Question 16

A company would like to understand its total cost of ownership (TCO) when all workloads are moved to the cloud. Which should the company consider in their AWS TCO?
(Choose 3)

Question 17

You want to define a secure private network in an AWS account where you launch your resources. What do you need to configure?

**Virtual private cloud (VPC)**

Question 18

Which of the following are storage services?
(Choose 2)

**S3, AWS Elastic File System**

Question 19

Which cloud computing model offers fundamental building blocks that can be rented?

**Infrastructure as a Service (IaaS)**
> IaaS offers building blocks that can be rented. EC2 is an example of IaaS

Question 20

Which AWS service allows you to run code without having to worry about provisioning any underlying resources (such as virtual machines, databases, etc.)?

**Lambda**

> Lambda is the AWS Function as a Service (FaaS) offering that lets you run code without provisioning or managing servers

Question 21

Which of the following support plans features a < 4-hour response time in the event of an impaired production system?

**Business**

Question 22

A fantasy sports company needs to run an application for the length of a football season (5 months). They will run the application on an EC2 instance and there can be no interruption. Which purchasing option best suits this use case?

**On-Demand**

Question 23

Which of the following are common use cases for S3?
(Choose 2)

- Static web hosting
- Storing application assets

Question 24

A healthcare company has nightly batch jobs that can afford to be interrupted. Which EC2 pricing model can meet this need and provide great savings by using a supply-and-demand model?

**Spot Instances**

Question 25

A customer would like the ability to send HTML formatted emails from their application for marketing campaigns. Which service should the customer consider using?

**Simple Email Service (SES)**

Question 26

You have a short-term computing task to complete. It is essential that this task run uninterrupted from start to finish. Which is the best EC2 option for this task?

**On-Demand Instance**


Question 27

What are the 3 cloud computing models?
(Choose 3)

- Infrastructure as a Service (IaaS)
- Software as a Service (SaaS)
- Platform as a Service (PaaS)

Question 28

Which of the following statements are true about who can use IAM roles?
(Choose 3)

- A web service offered by AWS.
- An IAM user in the same AWS account as the role.
- An IAM user in a different AWS account than the role.


Question 29

Which of the following AWS services gives you a personalized view of the performance and availability of the AWS services underlying your AWS resources, alerting you and providing remediation guidance when AWS is experiencing events that may affect you?

**AWS Personal Health Dashboard**

> AWS Personal Health Dashboard gives you a personalized view of the performance and availability of the AWS services underlying your AWS resources.

Question 30

If you have a new application and you are not sure about future demand, which of the below characteristics of cloud make cloud an ideal place to host it?
(Choose 3)

**Scalability**

> No upfront payment and pay as you go mean that you do not need an initial outlay of capital for resources to build in cloud. Rather, you only need to pay for what you use going forward. These combined with the ability to consume more resources when needed (scalability) mean that cloud is a great way to host applications that have dynamic requirements

**No upfront payment**

**Pay as you go**


Question 31

A healthcare agency needs to store certain patient information for up to 10 years. To save cost, they want to archive this data to cheaper storage. The data needs to be retrieved within 12 hours. Which is the cheapest option?

**Glacier Deep Archive**

Question 32

Which of the following allows you to access AWS services from popular programming languages like Java, Python, and C#?

**Software development kits**

Question 33

Which of the following AWS services is a fast, fully managed data warehouse that makes it simple and cost-effective to analyze all your data using standard SQL and your existing business intelligence tools.

**Redshift**

Question 34

Which of the following is AWS' event-driven, serverless compute service?

**Lambda**

> Lambda is AWS' event-driven, serverless compute service that allows you to run code without having to deploy or manage any of the underlying resources such as EC2 instances.

Question 35

Which of the following are advantages of cloud computing?
(Choose 3)

- Elasticity
- Agility
- Variable expense

Question 36

A telecommunications company has hired you as a consultant to develop a business case for moving its IT applications and infrastructure to AWS. The company's leadership understands the agility value of the cloud, but the finance group is not interested in shifting capital expense to operating expense due to the company's tax structure. What will you include in the business case to attempt to satisfy everyone at the company?

**Suggest that the company make Reserved Instance purchases and capitalize them.**

Question 37

How does AWS Shield Standard help protect your environment?

**By blocking DDOS attacks**

Question 38

Which of the following are characteristics of Availability Zones?
(Choose 3)

- Contain redundant connectivity
- Contain redundant networking
- Contain physically separated data centers

Question 39

A customer has a complex multi-resource application environment containing multiple EC2 instances, load balancers, S3 buckets, and more. They'd like to provision these resources in an automated and repeatable manner from environment to environment using Infrastructure as Code (IaC). Which service achieves this?

**CloudFormation**

Question 40

In Identity and Access Management (IAM), which term applies to a person or application that uses the AWS account root user, an IAM user, or an IAM role to sign in and make requests to AWS?

**Principal**

> A principal is a person or application that uses the AWS account root user, an IAM user, or an IAM role to sign in and make requests to AWS

Question 41

An EC2 instance in your VPC needs which of the following for the internet gateway to route its traffic to the internet?

**Public IP address**

> An EC2 instance in your VPC needs a public IP address for the internet gateway to route its traffic to the internet

Question 42

What type of long-term credentials for IAM users can be used to sign programmatic requests to the AWS CLI or AWS API (directly or using the AWS SDK)?

**Access keys**

> Access keys are long-term credentials for an IAM user or the AWS account root user. You can use access keys to sign programmatic requests to the AWS CLI or AWS API (directly or using the AWS SDK). Access keys consist of two parts: an access key ID (for example, AKIAIOSFODNN7EXAMPLE) and a secret access key (for example, wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY). Like a user name and password, you must use both the access key ID and secret access key together to authenticate your requests.

Question 43

You have a read-heavy application workload resulting in I/O-intensive Amazon RDS database queries. Which service is most suitable to improve performance?

**ElastiCache**

> You can use ElastiCache to store the results of often-used queries, and this will allow quicker retrieval of this data

Question 44

How does S3 Transfer Acceleration help you get your data into S3 quicker?

**By using AWS' network of edge locations to upload to a location closest to you before taking the most optimal path within AWS' network**

Question 45

Which of the following are valid ways for an IAM user to manage AWS resources?
(Choose 3)

- AWS Management Console access
- **Programmatic access via the command line**
- Using the AWS SDK

Question 46

You need to store key-value pairs of users and their high scores for a gaming application. Which is the fastest and cheapest storage option for this type of data?

**DynamoDB**

Question 47

Which of the following AWS Support pricing plans provides a Technical Account Manager (TAM) for proactive guidance on your AWS account?

**Enterprise**

Question 48

Which of the following can you host on S3?

**Static websites**

Question 49

Which of the following statements are true about the Amazon EC2 service?
(Choose 3)

- It supplies various configurations of CPU, memory, storage, and network capacity. You can use a preconfigured template called an Amazon Machine Image (AMI) to launch your instance.
- It provides scalable computing capacity in the AWS cloud.
- It provides virtual computing environments

Question 50

A company would like to automate the configuration of its servers and deploy code to servers in the cloud and on-premises. Which service meets the requirement?

**OpsWorks**

Question 51

What can you do using AWS Budgets?

**Track costs associated with your account and choose to be alerted when expenditures exceed your fixed target amount**

Question 52

What is the time that passes between a user request and the resulting response called?

**Latency**

> Latency is the time that passes between a user request and the resulting response

Question 53

When would you use the EC2 On-Demand pricing model?
(Choose 2)

- **No upfront payments required**
- **Unpredictable workloads that cannot be interrupted**

Question 54

Broadly speaking, AWS is responsible for:

**Security OF the Cloud**

Question 55

A company would like to implement a hybrid storage model where they connect on-premises data storage to storage in the AWS Cloud in order to move their backups to the cloud. What is the best and most efficient way to achieve this?

**Storage Gateway**

> Storage Gateway is a hybrid storage service that allows you to connect on-premises and cloud data.


Question 56

Which of the below statements are correct in relation to security responsibilities in AWS?
(Choose 2)

- As an AWS customer, you are responsible for the security IN the Cloud
- AWS is responsible for the security OF the Cloud.


Question 57

A company runs workloads in the cloud with unknown and dynamic user demand. Which usage features make the cloud cost effective for this type of workload?
(Choose 2)

- Pay-as-you-go
- On-demand

Question 58

The AWS global infrastructure includes Regions, Availability Zones, and edge locations. Which best describes the relationship between the infrastructure components?
(Choose 2)

- There are more edge locations than Regions
- There are more Availability Zones than Regions

Question 59

Which of the following best describes an AWS Region?

**A specific geographic location designed to provide high availability to a certain area**

Question 60

You want to streamline access management for your AWS administrators by assigning them permissions based on their job role. Which AWS features would you use to define and manage permissions for a set of users based on their roles?
(Choose 2)

**Use IAM groups**

> Using IAM groups lets you create a list of pre-defined permissions that any user made a part of that group will be granted. Roles are primarily used to grant AWS resources permissions to other AWS resources and generally are not for end-users

**Use IAM policies**
> You manage permissions for IAM users, groups, and roles by creating a policy document in JSON format and attaching it

Question 61

Your design team has recommended the need to distribute incoming traffic across multiple EC2 instances and also across multiple Availability Zones. Which AWS service can accomplish this?

**Elastic Load Balancing**

> Elastic Load Balancing automatically distributes incoming application traffic across multiple targets, such as Amazon EC2 instances

Question 62

How can new AWS users easily search for and find services in their AWS accounts?

**AWS Management Console**

Question 63

Which of the below are you responsible for when running an RDS database on AWS?

**Controlling access to the database**

Question 64

Which security service provides enhanced protections and 24/7 access to AWS experts for a fee when issues arise?

**AWS Shield Advanced**

> AWS Shield Advanced provides enhanced protections and 24/7 access to AWS experts for a fee

Question 65

If you want access to all AWS Trusted Advisor checks, which of the AWS Support plans will provide that?
(Choose 2)

**Enterprise**, **Business**

## Dump 6

Question 1

Who are the main users of the AWS Command Line Interface (CLI)?

**Developers**

Question 2

Which of the following statements are true of Amazon Redshift?
(Choose 2)

- **It is designed for storing petabytes of data.**
- **It is a data warehouse service.**

Question 3

You are leading a pilot program to try the AWS Cloud for 1 of your applications. You have been instructed to provide an estimate of your AWS bill. Which service will allow you to do this by manually entering your planned resources by service?

Question 4

You have been tasked with going into the AWS company account and getting information on saving money, improving system performance and reliability, and closing security gaps. Which tool can you use to get this information?

Question 5

Which benefit of cloud computing allows you to avoid planning ahead of time for how much capacity you need?

**Elasticity**

Question 6

Which of the following AWS services controls authentication and authorization within an AWS account?

Question 7

Which of the following provides the least expensive Amazon S3 storage?

Question 8

Which defines one or more discrete data centers with redundant power, networking, and connectivity?

**Availability Zone**

Question 9

Which of the following best describes Availability Zones (AZs)?

**Distinct locations from within an AWS Region that are engineered to be isolated from failures**


Question 10

An auditor is conducting an audit of your IT operations for compliance. The auditor requests visibility to logs of event history across your AWS-based employee expense system infrastructure. Which AWS service will record and provide you the information you need?

**AWS CloudTrail**

Question 11

You have used On-Demand Instances for a month but have met unexpected costs with this choice. Which EC2 option provides up to 90% discount on On-Demand Instances while taking advantage of AWS unused EC2 capacity?

Question 12

Users need to access AWS resources from the Command Line Interface. Which IAM option can be used for authentication?

Question 13

Which of the following statements is true of AWS CloudTrail?
(Choose 3)

- **Log files are encrypted**
- **With CloudTrail, you can create a trail that either applies to one Region or to all Regions**
- **CloudTrail delivers log files within 15 minutes of account activity.**


Question 14

You are using your corporate directory to grant your users access to AWS services. What is this called?

**Federated access**

Question 15

You need to set up a virtual firewall for your EC2 instance. Which would you use?

Question 16

Which term refers to the Identity and Access Management (IAM) **resource objects** that AWS uses for authentication?

**Entities**

Question 17

ElastiCache is an example of what type of AWS service?

Question 18

Which of the following services does the AWS Shield Standard plan provide?
(Choose 2)

- **Network flow monitoring**
- **Assistance with protection from common DDoS attacks**


Question 19

Trusted Advisor is classified as what type of AWS service?

- **Management & Governance**

Question 20

Which of the following engines are classified as relational databases on AWS?
(Choose 3)

Question 21

Which of the following enables you to interact with AWS services using only textual commands?

Question 22

Which component of the AWS Global Infrastructure caches content for fast delivery to users?

**Edge locations**

Question 23

Which following statement is true of newly created security groups with their default rules?

Question 24

Which of the following AWS Support levels offers the assistance of a Technical Account Manager?

Question 25

Which of the following AWS services enables you to continuously monitor and record configuration changes of your resources?

Question 26

Which of the following best describes the ability to scale computing resources out or in easily, while only paying for the resources used?

**Elasticity**

> Elasticity describes the ability to scale computing resources out or in easily, while only paying for the resources used.

Question 27

Your Development team uses 4 On-Demand EC2 instances. Your QA team has 5 Reserved Instances, only 3 of which are being used. Assuming all AWS accounts are under a single AWS Organization, how will the Development team's instances be billed?

**The Dev team will be billed for 2 instances at On-Demand prices and 2 instances at the Reserved Instance price.**

Question 28

Which of the following falls under the AWS compute services category?
(Choose 2)

Question 29

You are working with IAM and need to attach policies to users, groups, and roles. Which of the following will you be attaching these policies to?

**Identities**

Question 30

Which of the following statements are true of Amazon Aurora?
(Choose 2)

- **You can use the AWS Management Console, AWS CLI commands, and API operations to handle routine database tasks.**
- **It is compatible with the MySQL and PostgreSQL database engines**.

Question 31

Which of the following support plans features access to Enhanced Technical Support via email only during business hours?

Question 32

In order to comply with regulatory mandates, some of your data needs to be retained in perpetuity. Which of the following AWS storage classes offers low-cost, long-term data archival?

Question 33

Your application needs fully managed storage for objects. Which of the following options should you choose?

Question 34

You have recently started using AWS and now need to launch a large number of instances in your VPC. You learn that this number exceeds the service limits for instances in a VPC. What can you do?

**Contact AWS and request a service limit increase**

Question 35

You've been tasked with assessing your AWS infrastructure in terms of cost optimization. Which of the following AWS services would help with this task?

Question 36

AWS uses the shared responsibility model. For security, which of the following are the responsibilities of AWS?
(Choose 3)

Question 37

Which of the following does Amazon ensure will happen when paying for AWS on an as-needed basis?
(Choose 3)

- Redirecting focus to innovation and invention
- **Reducing procurement complexity**
- Enabling the full elasticity of business operations

Question 38

Which of the following are characteristics of Availability Zones (AZs)?
(Choose 3)

- Fault tolerant
- Physically separated
- Connected through low-latency links

Question 39

Which benefit of cloud computing helps you innovate faster and gives you speed to market?

**Agility**

Question 40

A company has a large number of S3 buckets and needs to manage and automate tasks on these buckets at one time. Which AWS feature can do this?

Question 41

Which of the following AWS services fall under the Migration and Transfer category?
(Choose 2)

Question 42

Your company has entered into a 3-year contract with a government agency. Your best option for EC2 is Reserved Instances. Which AWS feature would you use to track your Reserved Instance usage?

Question 43

The AWS Global Infrastructure comprises Regions, Availability Zones, and edge locations, and there is a different number of each infrastructure element. Select the option that shows the correct order from greatest to least.

Number of Edge Locations > Number of Availability Zones > Number of Regions

Question 44

Which of the following does AWS use to notify you by email when you exceed **85% of your Free Tier limits for each service**?

**AWS Budgets**

Question 45

Enabling Amazon GuardDuty automatically grants the service permission to analyze continuous metadata streams from which of the following data sources?
(Choose 3)

Question 46

When would you use the Reserved Instance pricing model?
(Choose 2)

Question 47

Which of the following is AWS' managed DDoS protection service?

Question 48

A company on the Business Support plan currently runs all their applications in a single Region. They have made the decision to expand to multiple Regions. What is the process to start deploying their applications to the new Regions?

**Just start deploying the applications to the new Regions**

Question 49

Which of the following is true of AWS Lambda?
(Choose 3)

Question 50

Which of the following statements are true of the AWS Free Tier?
(Choose 2)

Question 51

Upon which of these measurements is AWS Lambda pricing based?
(Choose 3)

- **Number of requests**
- **Data transfer**
- **Duration and memory**


Question 52

In AWS, you can stop or terminate instances when not in use. Which of the following concepts describes this capability?

Elasticity

Question 53

Which of the below are you responsible for when running an EC2 instance on AWS?
(Choose 2)

Question 54

Your company hosts gaming applications online and would like to deliver these apps to a worldwide audience. Which AWS service would enable delivery to users worldwide and greatly improve response times?

Question 55

Which of the following is an AWS managed distributed denial-of-service (DDoS) protection service?

Question 56

Which of the following falls under AWS compute services category?
(Choose 3)

- **Amazon Elastic Compute Cloud (EC2)**
- **Amazon Lightsail**
- **Amazon Elastic Beanstalk**

Question 57

According to the AWS Shared Responsibility Model, which of the following is the customer responsible for?
(Choose 3)

Question 58

Which of the following compute services is ideal if you need to run a simple website or a simple e-commerce application?

Question 59

VPC, CloudFront, and Route 53 are examples of what type of AWS service?

Question 60

Which deployment types offers the advantages of cloud computing?
(Choose 2)

- Public cloud
- Hybrid cloud

Question 61

Which of the following are examples of programmatic access?
(Choose 3)
- Command Line Interface (CLI)
- Application code
- Software Development Kits (SDKs)

Question 62

Which of the following are characteristics of cloud computing?
(Choose 3)

- Services are delivered via the internet.
- Pay-as-you-go pricing
- On-demand delivery

Question 63

How are permissions assigned to an IAM group?
(Choose 2)

- **Roles**
- **Policies**

Question 64

Which of the following describes a subnet accurately?

Question 65

When architecting a solution on AWS, it is important to know if you are designing for zero downtime even if a component fails or if you are designing for reliable performance and minimal (but non-zero) downtime. Which of the following terms best describes the latter solution?

**High availability**