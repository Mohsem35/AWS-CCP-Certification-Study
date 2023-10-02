## AWS-Learning for AWS Certified Cloud Practitioner Exam

4 exam domains

- **`Cloud Concepts`** (24% of scored content)
- **`Security and Compliance`** (30% of scored content)
- **`Cloud Technology and Services`** (34% of scored content)
- **`Billing, Pricing, and Support`** (12% of scored content)

#### chapter 1
### Foundations of Cloud Computing

Q: What is cloud computing, exactly?
Cloud computing is the **delivery of computing services** over the internet.

_Service Category_ | _Names_
------------- | -------------
_Compute_  | _EC2_, _Lambda_
Networking | VPC, Direct Connect
Storage  | S3, EBS
Analytics | Ethena, Redshift
Development | Cloud9, CodeCommit
Security | IAM, Macie
Databases | RDS, DynamoDB

 
> **_NOTE:_** Read the _overview of amazon web services whitepaper_, and review it again the day before exam.

[Overview of Amazon Web Services](https://docs.aws.amazon.com/pdfs/whitepapers/latest/aws-overview/aws-overview.pdf)





**`Virtualization`** is at the **`heart`** of _cloud computing_. Virtualization lets you _divide hardware resources_ on a single physical server into **`smaller units`** called _Virtual Machines_



**`Usage`** : Your usage is placed on a meter. You pay only when you access it and only for what you use.

1. **`On Demand`**: No long-term commitments or upfront payments
2. **`Pay as You Go`**: Pay by the hour or the second for only what you use



#### There are 6 advantages to cloud computing

1. **`Go global in minutes`**: Deploy your apps around the world at the click of a button.

2. **`Stop spending money running and maintaining data centers`**: You can focus on building your applications instead of managing hardware.

3. **`Benefit from massive economies of scale`**: Volume discounts are passed on to you, which provides lower pay-as-you-go prices.

4. **`Increase speed and agility`**: The provided services allow youto innovate more quickly and deliver your applications faster.

5. **`Stop guessing capacity`**: Your capacity is matched exactly to your demand.

6. **`Trade capital expense for variable expense`**: You pay for what you use instead of making huge upfront investments


#### Cloud computing terminology

- **`High Availability`**:  Highly available systems are designed to _operate continuously without failure for a long time_. These systems avoid loss of service by reducing or managing failures.

- **`Elasticity`**: With elasticity, you _don't have to plan ahead of time how much capacity you need_. You can provision only what you need, and then _grow and shrink based on demand_.

- **`Agility`**: The cloud gives you increased agility. All the services you have access to help you _innovate faster, giving you speed to market_.

- **`Durability`**: Durability is all about long-term data protection. This means your _data will remain intact without corruption_.



For more terminology: [AWS Terminology Cheat Sheet](https://www.pluralsight.com/resources/blog/cloud/your-aws-terminology-cheat-sheet)


**CapEx vs. OpEx**


_Capital Expenditure(CapEx)_: Capital expenditures are _upfront purchases toward fixed assetse_ like quipment, property, computers and softwares.
_Operating Expenditure(OpEx)_: Operating expenses are _funds used to run day-to-day operations_ like research and development, employee salaries, rent, marketing.


> **_NOTE:_**  Understand the _6 advantages_ and _cloud terminology_


#### Cloud Computing Models

There are 3 common cloud computing models

1. **`Infrastructure as a Service(IaaS)`**

- _Building Blocks_: Fundamental building blocks that can be rented like _EC2_
- _Web Hosting_: Monthly subscription to have a hosting company serve your website

2. **`Software as a Service(SaaS)`**

- _Complete Application_: Using a complete application, on demand, that  someone _offers to users_. Example: _Amazon SageMaker (cloud machine learning platform)_
- _Email Provider_: Your personal email that you access through a web browser is SaaS

3. **`Platform as a Service(PaaS)`**

- _Used by Developers_: Develop software using web-based tools without worrying about the underlying infrastructure. Example:  _Cloud9_

- _Storefront Website_: Tools provided to build a storefront application that runs on another company’s server


#### Cloud Deployment Models

There are 3 common cloud deployment models

1. Private Cloud
2. Public Cloud
3. **`Hybrid(Private + Public)Cloud`**: Companies keep **`Highly sensitive data`** stored in their own private cloud but web application runs on AWS infrastructure. AWS provides tools so they talk to each other using a service provided by AWS called **`direct connect`** 


> **_NOTE:_** Know the _computing models_ and _delpoyment models_

#### Region

**`Region`**: A Region is a  _physical location_. AWS logically _groups its Regions_ into **`geographic`** locations


Region Characteristics:


- A Region is a **`collection of AZs`**
- You should set up resources in Regions _closest to your users_
- A Region is **`global`** and has _2 or more AZs_
- Fully **`Independent`** and **`Isolated`**
- **`Physicall seperated`** and they _use different power grids_
- _Connected among themselves_ through **`low-latency`** links
- **`Fault tolerant`** means one AZ goes out of service, the _other should not be impacted_
- Allows for high availability


#### Availability Zones

**`Availability Zones`**: Availability Zones (AZs) consist of one or more physically separated **`data centers`**, each with _redundant power, networking, and connectivity, housed in separate facilities_.

1. An AZ is a **`collection of data centers`**
2. An AZ contains the _servers you are renting_, and where you deploy your applications
3. An AZ is _associated with a single Region_
4. **`Multi-AZ deployments`** provide high availability. Systems that are highly available are dependable enough to **`operate continuously without failure`**


#### Edge Locations

**`Edge Locations`**: Edge locations **`cache content`** for **`fast delivery`** to your users

- Edge locations **`reduce latency`**
- Content delivery network(**`CDN`**) and cache content by **`Amazon CloudFront`**
- An edge location is like **`mini data center`**, but it _doesn't run our main infrastructure_ like EC2 instances.
- Edge locations ensure low latency by placing content **`closer to users`**. There are _more edge locations than Regions and AZs_





#### The AWS Management Console


The AWS Management Console is **`GUI`** and allows you to access your AWS account and manage applications running in your account from a **`web browser`**

Good For: 
- If you’re just _getting started with the cloud_.
- If you serve in a _non-technical role: business analyst, project manager, and many more_. 
- If you serve in a _technical role: software engineer, web developer, solutions architect, and many more_.


#### Root User

Root user is **`automatically`** created when you **`initially sign up`** for your account
- _Protect Root user_ with multi-factor authentication (**`MFA`**)
- There are _certain things that only the root user can do_
- One thing that will _already be provisioned in our AWS account_ will be a **`default VPC`**

#### AWS Command Line Interface (CLI)


The AWS Command Line Interface (CLI) allows you to _access your AWS account_ through a **`terminal`** or **`command`** window.

- The CLI is mainly used by **`developers`**
- AWS CLI are sending commands which **`trigger APIs`** _through your terminal_

> **_NOTE:_** Sometimes new features are available via the CLI before the console

**`Programmatic Access`**: Programmatic access provides _access to your AWS resources_ through an application or a _tool like the CLI_

AWS services can be accessed by 3 ways

1. _CLI_: from a terminal session of our laptop
2. _Application Code_: services can be accessed from application code using SDKs and programmatic calls
3. _Software Development Kits (SDKs)_: from popular programming languages like Java, Python, C# and many more 

