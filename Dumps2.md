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




