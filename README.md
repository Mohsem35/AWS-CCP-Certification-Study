Demonstrate: EC2, Lambda. S3, Rekognition, DynamoDB Table Using CloudFormation, Cloudwatch, IAM


Agendas

1. [Foundations of Cloud Computing](#foundations-of-cloud-computing)
2. [Technology](#technology)
3. [Security and Compliance](#security-and-compliance)
4. [Pricing, Billing and Governance](#pricing-billing-and-governance)


## AWS-Learning for AWS Certified Cloud Practitioner Exam

4 exam domains

- **`Cloud Concepts`** (24% of scored content)
- **`Security and Compliance`** (30% of scored content)
- **`Cloud Technology and Services`** (34% of scored content)
- **`Billing, Pricing, and Support`** (12% of scored content)

#### chapter 1
### Foundations of Cloud Computing 

### 24%

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





**Virtualization** is at the **heart** of cloud computing. Virtualization lets you divide hardware resources on a single physical server into **smaller units** called Virtual Machines



**`Usage`** : Your usage is placed on a meter. You pay only when you access it and only for what you use.

1. **`On Demand`**: No long-term commitments or upfront payments
2. **`Pay as You Go`**: Pay by the hour or the second for only what you use



#### There are 6 advantages to cloud computing

1. **Go global in minutes**: Deploy your apps around the world at the click of a button.

2. **Stop spending money running and maintaining data centers**: You can focus on building your applications instead of managing hardware.

3. **Benefit from massive economies of scale**: **Volume discounts are passed on to you**, which provides lower **pay-as-you-go** prices.

4. **Increase speed and agility**: The provided services allow you to **innovate** more quickly and **deliver your applications faster**.

5. **Stop guessing capacity**: Your capacity is matched exactly to your demand.

6. **Trade capital expense for variable expense**: You **pay for what you use** instead of making huge upfront investments


#### Cloud computing terminology

- **`High Availability`**:  Highly available systems are designed to **operate continuously without failure for a long time**. These systems avoid loss of service by reducing or managing failures.

- **`Elasticity`**: With elasticity, you don't have to plan ahead of time how much capacity you need_. You can provision only what you need, and then **grow and shrink based on demand**.

- **`Agility`**: The cloud gives you increased agility. All the services you have access to help you **innovate faster, giving you speed to market**.

- **`Durability`**: Durability is all about **long-term data protection**. This means your **data will remain intact without corruption**.



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


#### Data Center

A single data center contains multiple servers

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


#### Questions  

Which of the following is a best practice for securing access to your AWS account?
- Multi-Factor Authentication (MFA)

Which of the following are benefits provided by cloud computing?
- It offers easy access to servers, storage, and other services over the internet.
- It allows on-demand spinning up of needed resources (such as virtual machines).

Which of the following is a geographic area containing multiple Availability Zones (AZs)?
- Region

AWS defines a hybrid cloud as a combination of public and private clouds.

- True

What does the concept of durability mean in a cloud computing environment?
- Durability offers long-term data protection.

Which of the following contains 1 or more physically separated data centers?
- Availability Zone

Which type of expense includes upfront purchases toward fixed assets?
- Capital expenditures (CapEx)

Which of the following actions can be performed using the AWS Console?
- Access your AWS account
- Search for services
- Manage applications

Which type of expense includes funds used to run day-to-day operations? 
- Operating expenses (OpEx)


#### chapter 2
### Technology 

#### (33%)

![amazon_ec2](https://github.com/Mohsem35/AWS-Learning/assets/58659448/69d04611-d71a-41e5-bbe4-88323bf20ff4)


#### Elastic Compute Cloud (EC2)

- Elastic compute power simply means that it can grow and shrink
- EC2 is a **`foundational piece`** of AWS's Cloud Computing platform 
- EC2 allows you to **`rent and manage virtual servers`** in the cloud


**`Servers`** are the _physical compute hardware_ **`running in a data center`**.

**`EC2 instances`** are the _virtual servers_ running on these physical servers.

Instances are **`not`** considered **`serverless`**

##### Let's take a closer look of EC2

1. You're able to provision an EC2 instance at the click of a button
2. You can use a preconfigured **`template`** called an **`Amazon Machine Image (AMI)`** to launch your instance.
3. You can deploy your applications directly to EC2 instances.
4. You receive 750 compute hours per month on the Free Tier plan.


##### Use Cases

EC2 in the Real World

1. **`Deploy a database`**: Deploying a database to EC2 gives you _full control over the database_

1. **`Deploy a web application`**: Deploy to **`multiple AZs`** to make the web application highly available

##### Connectivity

Methods to Access an EC2 Instance


- [x] _AWS Management Console_

You're able to configure and manage your instances **`via web browser`**

- [x] _Secure Shell (SSH)_

SSH allows you to establish a **`secure connection`** to your instance **`from your local laptop`** 

- [x] _EC2 Instance Connect (EIC)_

EIC allows you to use **`IAM policies`** to control SSH access to your instances, **`removing the need to manage SSH keys`**

- [x] _AWS Systems Manager_

Systems Manager allows you to manage your EC2 instances **`via a web browser or the AWS CLI`**.

<img width="850" alt="Screenshot 2023-10-10 at 12 26 20 AM" src="https://github.com/Mohsem35/AWS-Learning/assets/58659448/684a2491-5cd2-47f6-a4ae-11887e32befc">


#### EC2 Pricing Options

##### 1. On-Demand
A fixed price in which you are billed **`down to the second`** based on the instance type. There is no contract, and you **`pay only for what you use`**.

Use On-Demand instances when:
1. You care about _low cost without any upfront payment or long-term commitment_.
2. Your applications have _unpredictable workloads that can't be interrupted_.
3. Your _applications are under development_.
4. Your workloads will _not run longer than a year_.

Fun facts:

You can **`reserve capacity`** using On-Demand Capacity Reservations. The EC2 capacity is held for you whether or not you run the instance.


##### 2. Spot (Cheapest Option)
Spot instances let you take advantage of **`unused`** EC2 capacity. Your request is fulfilled **`only`** if capacity is available.

Use Spot instances when:
1. You are **`not concerned`** about the _start or stop time of your application_
2. Your workloads can be **`interrupted`**.
3. Your _application is only feasible at very low compute prices_


Fun facts:

You can save up to **`90% off`** On-Demand prices. You pay the spot price that's in effect at the beginning of each hour.


##### 3. Reserved Instances (RIs)
RIs allow you to **`commit`** to a _specific instance type_ in a **`particular Region for 1 or 3 years`**.

Use Reserved Instances when:

1. Your application has **`steady state usage`**, and you can commit to 1 or 3 years.
2. You can pay money **`upfront`** in order to receive a discount on On-Demand prices.
3. Your application requires a **`capacity reservation`**


Fun facts:
- You can save up to 75% off On-Demand prices.
- You are **`required to sign a contract`**.
- You can **`reserve capacity`** in an **`Availability Zone`** _for any duration_   
- You can pay **`All Upfront`**, Partial Upfront, or No Upfront. All Upfront for the max term earns the highest discount.
- Provides convertible types at **`54%`** discount.



##### 4. Dedicated Hosts

Dedicated Hosts allow you to pay for a physical server that is **`fully dedicated to running your instances`**.

Use Dedicated Hosts when:
1. You want to **`bring your own`** _server-bound software_ **`license`** from vendors like Microsoft or Oracle.
2. You have regulatory or corporate compliance requirements around tenancy model.


Fun facts:

- You can save up to 70% off On-Demand prices.
- You bring your existing **`per-socket`**, **`per-core`**, or **`per-VM`** software licenses.
- There is no multi-tenancy, meaning the **`server is not shared with other customers`**.
- A Dedicated Host is a physical server, whereas a Dedicated Instance runs on the host.



##### 5. Savings Plan
Savings Plan allows you to commit to compute usage (**`measured per hour`**) _for 1 or 3 years_.

Use Savings Plans when:
1. _You want to lower your bill across multiple compute services_.
2. You want the **`flexibility to change`** compute services, instance types, operating sytems, or Regions.

Fun facts:

- You can save up to 72% off On-Demand prices.
- You are not making a commitment to a Dedicated Host, **`just compute usage`**
- Savings **`can be shared across various compute services`** like EC2, Fargate, and Lambda.
- This does **`not`** provide a capacity reservation.

#### Features


EC2 instances offer 

1. **`load balancing`** and
2. **`Auto Scaling`**

#### Elastic Load Balancer

![AWS-Elastic-Load-Balancing-AWS-ELB](https://github.com/Mohsem35/AWS-Learning/assets/58659448/4e9a843b-5243-4c0a-890d-cf7a41f474b0)


**_Elastic Load Balancing_** automatically distributes your **`incoming application traffic`** across multiple EC2 instances

<img width="387" alt="Screenshot 2023-10-10 at 5 42 21 PM" src="https://github.com/Mohsem35/AWS-Learning/assets/58659448/a3e03089-161c-4eea-83e6-5672b2220308">

Four types of load balancers are available
1. Classis
2. Application
3. Gateway
4. Network


![download](https://github.com/Mohsem35/AWS-Learning/assets/58659448/72d61e38-f1f2-4ce7-92fa-89a1ecd38bf7)

#### EC2 Auto Scaling

![1_9ke2MJPI9vy034alPKJk7A](https://github.com/Mohsem35/AWS-Learning/assets/58659448/7933549a-a99b-4d4c-abca-db538738a7e9)

**_EC2 Auto Scaling_** adds or replaces EC2 instances automatically across AZs, **`based on need and changing demand`**

<img width="349" alt="Screenshot 2023-10-10 at 5 51 47 PM" src="https://github.com/Mohsem35/AWS-Learning/assets/58659448/3ad0ebce-5043-4730-8d4e-e47a69a0f318">

Auto Scaling reduces the impact of system failures and improves the availability of your applications.

> **_Note_** : Do not confuse horizontal scaling with vertical scaling (or scaling up), which upgrades an EC2 instance by adding more power (CPU, RAM) to an existing server.

- `EC2 pricing options`: Understand On-Demand, Spot, Reserved Instances, Dedicated Hosts, and Savings Plans.
- `Know the types of load balancers`: Classic, Application, Gateway, and Network
- `Understand real-world usage`: Deploying a database or a web application
- `Horizontal scaling vs. vertical scaling`: Horizontal scaling (or scaling out) adds or replaces instances, while vertical scaling (or scaling up) upgrades an existing instance.
- `Understand the benefits of Auto Scaling`: Remember Auto Scaling improves the availability of your applications, and don't confuse it with load balancing.
- `Understand how to connect to an EC2 instance from your local machine`: A key pair is needed to access an EC2 instance from your local machine.




![download png 20-44-42-831](https://github.com/Mohsem35/AWS-Learning/assets/58659448/24f4939f-0761-4a02-8eb0-6e7dde49fa4d)

#### AWS Lambda



Lambda allows **`developers`** to _focus on core business logic_ for the apps they are developing _instead of worrying about managing servers_

AWS Lambda is a **`serverless compute service`** that lets you **`run code without managing servers`**

- _You author application code_, called **`functions`**, using many popular languages
- Scales automatically
- **`Serverless`** means you _don’t worry about managing servers like with EC2_


##### Use Cases

Lambda is a **`building block`** for many serverless applications. Serverless simply means _AWS manages the servers for you_ and you **`cannot access`** them. You can pretend they don't exist.


1. **`Real-time file processing`**

<img width="400" alt="Screenshot 2023-10-10 at 8 10 24 PM" src="https://github.com/Mohsem35/AWS-Learning/assets/58659448/96c7d03e-5c9f-41d3-8fd8-bad3fa09dd53">


2. **`Sending email notifications`**

<img width="400" alt="Screenshot 2023-10-10 at 8 14 13 PM" src="https://github.com/Mohsem35/AWS-Learning/assets/58659448/7fe2999d-20f6-4234-9d5f-029207213013">


3. **`Backend business logic`**

<img width="400" alt="Screenshot 2023-10-10 at 8 14 23 PM" src="https://github.com/Mohsem35/AWS-Learning/assets/58659448/13c72d5b-7390-467c-a3ef-1e0de5f2ecca">


##### Features


1. **`Supports popular programming languages`** like Java, Go, PowerShell, Node.js, C#, Python, and Ruby.
2. You **`author code`** using your favorite development environment or via the console.
3. Lambda can _execute your code_ in _response to events_
4. Lambda **`functions`** have a **`15-minute timeout`**


##### Pricing Model

You are charged based on the **`duration`** and **`number of requests`**


1. **`Compute time`**: Pay only for compute time used - there is **`no charge if your code is not running`**

2. **`Request count`**: A request is counted each time it starts execution. _Test invokes in the console count as well_

3. **`Always free`**: The free usage tier includes **`1 million free requests each month`**


>**_Note_**: Things to Remember When Studying for the Exam


- Your responsibility: You are only responsible for your application code. AWS manages servers, coding environment, and language support.
- Always free: Even after the free-usage tier expires, you'll have access to 1 million free Lambda calls each month.



#### AWS Fargate

Fargate is a **`serverless`** compute engine for **`containers`**


- Fargate allows you to _manage containers, like Docker_.
- _Scales automatically_
- Serverless means you don’t worry about provisioning, configuring, or scaling servers.
- Fargate _works with Amazon Elastic Container Service_, **`ECS`**




#### Amazon Lightsail

Lightsail allows you to **`quickly launch(preconfigured applications) all the resources`** you need for **`small projects`**

- _Deploy preconfigured applications_, like **`WordPress websites`**, at the click of a button
- Simple screens for _people with no cloud experience_
- Includes a **`virtual machine`**, **`SSD-based storage`**, **`data transfer`**, **`DNS management`**, and a **`static IP`**
- Provides a low, predictable monthly fee, as low as $3.50



#### AWS Outposts

AWS তে outpost লিখা দেখলেই বুঝতে হবে, সেখানে internal data center থাকবে 

Outposts allows you to **`run cloud services`** in your **`internal data center`**

- Supports workloads that need to **`remain on-premises`** due to _latency or data sovereignty needs_

> **_Note_**: data sovereignty is also considered data residency.
You may have _legal, regulatory, or contractual requirements that require you to keep your data in a particular location_,and Outposts can assist you with that.

- AWS **`delivers and installs servers`** in your _internal data center_
- Have access to the cloud services and APIs to develop **`apps on-premises`**
- Used for a **`hybrid`** experience



#### AWS Batch

Batch allows you to process large **`workloads in smaller chunks`** (or batches).

- Runs hundreds and thousands of smaller **`batch processing`** jobs
- **`Dynamically`** provisions instances **`based on volume`**


![0_8qgeGxrtC7ynPl8I](https://github.com/Mohsem35/AWS-Learning/assets/58659448/a8b6806b-3c80-4075-b1d2-d8616f00bb5e)



#### AWS Amazon Simple Storage Service (S3)

Companies today need to _collect_, _store_, and _analyze_ the data they've accumulated over the years on a massive scale. Storage services in the cloud provide a place for companies to store data.

S3 is an **`object storage service`** for the cloud that is highly available

- **`Objects`** (or files) are stored in **`buckets`** (or directories). _Instead of files and directories, we have objects and buckets_
- Essentially **`unlimited storage`** that can hold millions of objects per bucket.
- Objects can be **`public`** or **`private`**
- You can **`upload`** objects via the _console_, the _CLI_, or _programmatically from within code using SDKs_. 


##### Facts


You can set **`security`** at the `bucket` or `individual` object level using _access control lists(ACLs)_, _bucket policies_, or _access point policies_


You can **`enable versioning`** to create _multiple versions of your file_ in order to protect against _accidental deletion_ and to use a previous version.


You can use **`S3 access logs`** to track the access to your buckets and objects. So that you can see the _root cause of issues_ or _track down any suspicious activity_

S3 is a **`regional service`**, but **`bucket names must be globally unique`**


##### Data Accessibility



1. **Durability**: Will my data be there tomorrow? means you can _expect your data to be there_. Durability is important so your **`objects are never lost or compromised`**

    Amazon S3 Standard is designed for _99.999999999%_ (**`11 9’s`**) of durability

2. **Availability**: How quickly can I access my data? _can I have it right now?_. Availability is important so you can **`access your data quickly`** when you need it.

    Amazon S3 Standard is designed for _99.99%_ availability

##### Q: How can AWS offer 11 nines of durability and 99.99%?

- data stored on an S3 buscket inside a region is **`replicated across multiple servers`**. so it gives HA and durability on a regional level. _for cross region replication, we have to set up of our own_

##### S3 Storage Classes

Amazon S3 offers several storage classes designed for different use cases.


1. **`S3 Standard`**
    - General-purpose storage 
    - Data stored across multiple Availability Zones
    - Low latency and high throughput

Recommended for: Frequently accessed data 

Durability of 99.999999999% & Availability of 99.99%


2. **`S3 Intelligent-Tiering`**
    - **`Automatically moves`** your data to the **`most cost-effective storage class`**
    - **`Automatic cost savings`**
    - _Machine learning behind the scene_
    - _No retrieval fees_
    - Data stored across multiple Availability Zones

Recommended for: **`Data`** with **`unknown or changing access pattern`**

Durability of 99.999999999% & Availability of 99.9% 


3. **`S3 Standard-Infrequent Access Recommended for (IA)`**
    - _Data accessed less frequently_ but requires rapid access
    - Data stored across multiple Availability Zones
    - Cheaper than S3 Standard


Recommended for: **`Long-lived data`**, **`Infrequently accessed`**, Millisecond access when needed
Availability of 99.9%

Durability of 99.999999999% & Availability of 99.9% 


4. **`S3 One Zone-Infrequent(IA)`**
    - Like S3 Standard-IA but **`data stored in a single Availability Zone`**
    - Costs 20% less than S3 Standard-IA
    - Data stored in this storage class can be lost

Durability of 99.999999999% & Availability of **`99.5%`**

Recommended for: **`Re-creatable data`**, Infrequently accessed with millisecond access, **`Availability and durability not essential`**


5. **`S3 Glacier`**

    - _Long-term data storage and archival for lower costs_
    - Data retrieval takes longer
    - 3 retrieval options: **`1-5 minutes`**, **`3-5 hours`**, or **`5-12 hours`**
    - Data stored across multiple Availability Zones

Recommended for: **`Long-term backups`**, Cheaper storage options

Durability of 99.999999999% and **`no Availability`**


6. **`S3 Glacier Deep Archive`**

    - Like S3 Glacier but longer access times
    - 2 retrieval options: **`12 hours`** or **`48 hours`**
    - **`Cheapest of all S3 options`**
    - Data stored across multiple Availability Zones

Recommended for: _Long-term data archival_ accessed **`once or twice a year`**, Retaining data for **`regulatory compliance requirements`**

Durability of 99.999999999% & **`no Availability`**


7. **`S3 Outposts`**

    - Provides object storage on- premises
    - A single storage class
    - Store data across multiple devices and servers

Recommended for: **`Data that needs to be kept local`**, Demanding **`application performance needs`**

**`no Durability & Availability`**


##### S3 in the Real World


1. _Static websites_: Deploy static websites to S3 and use _CloudFront_ for global distribution.

2. _Data archive_: Archive data using _Amazon Glacier_ as a storage option for Amazon S3.

3. _Analytics systems_: Store data in Amazon S3 for use with analytics services like _Redshift_ and _Athena_

4. _Mobile applications_: Mobile application users can _upload files_ to an Amazon S3 bucket.


Things to Remember
> **_Note_**: S3 is a _regional service but has a global namespace_, S3 offers unlimited storage with many storage classes. Understand the use cases for each storage class.


#### Additional Storage Services


#### > EC2  Storage

<img width="800" alt="Screenshot 2023-10-15 at 12 26 14 PM" src="https://github.com/Mohsem35/AWS-Learning/assets/58659448/51a7c98e-7231-4363-80ad-20c7b649249b">



All EC2 instances must have a **`root drive`**. this could be an _EBS_ volume or an _instance store drives(physical machine)_

#### Amazon Elastic Block Store (EBS)

EBS is a **`storage device`** (called a **`volume`**) that _can be attached to (or removed from_) your instance


- Data **`persists`** when the instance is not running
- Tied to **`one`** Availability Zone
- Can only be attached to **`one instance`** in the same Availability Zone


Recommended for: Quickly accessible data, **`Running a database on an instance`**, Long-term data storagex


You can also _attach multiple EBS volumes to a single EC2 instance_. You can think of these as **`hard drives`** that you've installed on the EC2 instance. The important **`distinction`** between EBS drives and instance store drives is that EBS drives are **`persistent`**. You can stop or terminate the instance, or even detach an EBS drive and attach it to a different EC2 instance. They have lower latency, but that data does not persist if an EC2 instance is stopped or terminated.




#### EC2 Instance Store

An **`instance store`** is local storage that is physically attached to the host computer and _cannot be removed_

- Storage on disks **`physically attached to an instance`**
- **`Faster`** with higher I/O speeds
- Storage is **`temporary`** since **`data loss`** occurs when the EC2 instance is **`stopped`**

Recommended for: Temporary storage needs, _Data replicated across multiple instances_

#### Amazon Elastic File System (EFS)

EFS is a **`serverless network file system`** for sharing files.

- Only supports the **`Linux`** file system
- More **`expensive`** than EBS
- Accessible across **`different Availability Zones`** in the same Region

like **`dropbox`** or **`google drive`**


Recommended for: Main directories for **`business-critical apps`**, Lift-and-shift existing enterprise apps


#### > Storage Gateway


#### Storage Gateway

Storage Gateway is a **`hybrid`** storage service.

- Connect **`on-premises`** and **`cloud`** data 
- Supports a hybrid model


So if you have a Site-to-Site **`VPN`** or a direct connection to the AWS Cloud, you can use Storage Gateway to hybridize your data storage. You can think of this sort of as a file directory, where some of the files are hosted locally, and some of them are hosted in the cloud.

Recommended for: **`Moving backups to the cloud`**, Reducing costs for hybrid cloud storage, _Low latency access to data_

#### > AWS Backup

#### AWS Backup

AWS Backup helps you manage **`data backups across multiple AWS services`**

- Integrates with resources like **`EC2`**, **`EBS`**, **`EFS`**, and more
- Create a backup plan that includes **`frequency`** and **`retention`**



#### Amazon CloudFront


##### What is a content delivery network (CDN)?


Well, the **`internet`** is all about **`delivering content`**, like websites and images and apps, and there are so many requests for massive amounts of data, like high-definition videos, large downloads, and more. Wouldn't it be nice if there were a **`service`** that ensured **`fast download times`**? Well, that's where a content delivery network comes into play.

A CDN is a mechanism to **`deliver content quickly`** and efficiently based on **`geographic location`**. Low latency is good!


**`Amazon CloudFront is a CDN`** that delivers data and applications globally with low latency.

- Makes content available **`globally`** or restricts it based on location
- **`Speeds up`** delivery of  static and dynamic web content
- Uses **`edge locations`** to **`cache`** content
- Even if your app is in a single Region, it can still be **`delivered globally`** because of CloudFront

> _Note_: Did you know that if the content is already in the edge location, CloudFront delivers it immediately? If not, CloudFront retrieves the files from the origin.


- **`CloudFront distribution cache`** is just the name given to a **`collection of edge locations`** and remember, an 
- edge location is like a **`mini data center`** where files are cached.

<img width="800" alt="Screenshot 2023-10-15 at 1 40 35 PM" src="https://github.com/Mohsem35/AWS-Learning/assets/58659448/c0947378-734f-487b-a411-ed90df358566">



##### Use cases

1. **`S3 static websites`**: CloudFront is often used with S3 to deploy content globally.

2. **`Prevent attacks`**: CloudFront can stop certain web attacks, like _DDoS_. 
3. **`IP addresses blocking`**: Geo-restriction prevents users in certain countries from accessing content.




#### Amazon Global Accelerator

Global Accelerator  **`sends your users`** through the **`AWS global network`** when _accessing your content, speeding up delivery_

- _Improves latency and availability_ of **`single-Region applications`**
- Sends traffic through the AWS global network infrastructure
- **`60%`** performance boost
- **`Automatically re-routes traffic`** to healthy available **`regional endpoints`**




#### Amazon S3 Transfer Acceleration

S3 Transfer Acceleration improves content **`uploads and downloads to and from S3 buckets`**

- **`Fast transfer`** of files over **`long distances`**
- **`Uses`** CloudFront’s globally distributed **`edge locations`**
- Customers around the world can upload to a **`central bucket`**


> Note: Things to Remember  

CloudFront: Don't forget CloudFront allows for global distribution of content. Don't forget CloudFront has security features like  _DDoS protection and geo-restriction_

Global Accelerator: Remember Global Accelerator provides _low latency_.

S3 Transfer Acceleration: Remember S3 Transfer Acceleration provides fast transfer of files over long distances.


#### Amazon Virtual Private Cloud (VPC)

<img width="600" alt="1687361452587" src="https://github.com/Mohsem35/AWS-Learning/assets/58659448/22bda7cc-5127-4a6a-9bbf-00fdcc527f27">


VPC is a foundational service that allows you to create a **`secure private network`** in the AWS cloud where you launch your resources.

- **`Private`** virtual network
- **`Launch`** resources like EC2 instances inside the VPC
- Isolate and **`protect resources`**
- A VPC **`spans Availability Zones`** in a Region

![Screenshot from 2023-10-17 19-15-35](https://github.com/Mohsem35/AWS-Learning/assets/58659448/96d53108-312d-4ee0-ae01-88c9257c8a54)

- You're able to set up a private virtual network, and you specify various things like the **`IP address range`**, **`subnets`**, **`security groups,`** and you configure **`route tables`**.


![Screenshot from 2023-10-17 19-18-04](https://github.com/Mohsem35/AWS-Learning/assets/58659448/bc11a2fe-b59e-4aca-8bf8-66c4e990083c)


First, we have a **`NACL (or network access control list)`**. This ensures the **`proper traffic`** is allowed into the **`subnet`** and you can use it to block traffic to a particular instance.

**`Router & Route Table`**: Defines where network traffic is routed

**`Internet Gateway`**: allows public traffic to the internet from a VPC

![Screenshot from 2023-10-17 19-22-50](https://github.com/Mohsem35/AWS-Learning/assets/58659448/6ccb378c-c100-441f-a107-0d004bcefddb)


Now _behind the scenes, the wizard is doing a lot for you_  . It's creating a VPC with a range of IP addresses, it's **`attaching an internet gateway to the VPC`**, creating a **`subnet`** creating a **`custom route table`**, and associating it with the subnet, and that basically allows the traffic to flow between the subnet and the internet gateway.

> **_Note_**: Things to Remember When
Don't forget an _internet gateway allows traffic to the public internet_ and _peering connects 2 VPCs together_

Learnings from LAB
create a VPC(only) -> create public subnet -> Enable auto-assign public IPv4 address for subnet ->  create internet gateway and attach to VPC -> create new route table to direct traffic in public subnet

### Networking Services: Additional Networking Services

Q: What Is DNS?

DNS stands for **`Domain Name System`** and directs internet traffic by connecting domain names with web servers.

![Amazon-Route-53](https://github.com/Mohsem35/AWS-Learning/assets/58659448/4ee3bbb9-6dad-41a5-aa8d-bc8a2ec35ce8)

#### Amazon Route 53

- Domain name registration
- Performs **`health checks`** on AWS resources
- Supports **`hybrid`** cloud architectures



#### AWS Direct Connect

![1682955125806](https://github.com/Mohsem35/AWS-Learning/assets/58659448/cdf2a6fb-58b8-4ca9-b212-d605666327be)



Direct Connect is a **`dedicated physical network connection`** from your on-premises data center to AWS.

- Dedicated **`physical`** network connection
- Connects your **`on-premises`** data center to **`AWS`**
- Data travels over a **`private network`** (over the public internet দিয়ে data travel করে না )
- Supports a **`hybrid`** environment

A hybrid cloud is a combination of public and private clouds.

![Screenshot from 2023-10-18 18-40-35](https://github.com/Mohsem35/AWS-Learning/assets/58659448/65b8fa56-6fc1-4b0a-86d6-5ee63a152a82)


##### Use cases of Direct Connect

1. **`Large datasets`**: Transfer large datasets to AWS 
2. **`Business-critical data`**: Transfer internal data directly to AWS, bypassing your internet service provider
3. **`Hybrid model`**: Build hybrid environments


#### AWS VPN

**`Site-to-Site VPN`** creates a secure connection between your internal networks and your AWS VPCs. 

- **`Similar to Direct Connect`**, but data travels over the **`public internet`** 
- **`Data`** is automatically **`encrypted`**


**Moving Applications**: A **`Site-to-Site`** VPN makes moving applications to the cloud easier.


Site-to-Site VPN in the Real World

![Screenshot from 2023-10-18 18-55-24](https://github.com/Mohsem35/AWS-Learning/assets/58659448/dea8be83-b874-4c9e-b802-f90d62be59d0)

**`Virtual Private Gateway`**: The VPN connector on the AWS side
**`Customer Gateway`**: The VPN connector on the customer side

AWS VPN is **`slightly cheaper`** than AWS Direct Connect



#### API Gateway

API Gateway allows you to build and manage APIs

- **`Share`** data between systems
- **`Integrate`** with services like **`Lambda`**

API Gateway in the Real World

![Screenshot from 2023-10-18 19-02-47](https://github.com/Mohsem35/AWS-Learning/assets/58659448/0b0de208-21fc-46d1-b095-13defcba8858)




> _Note_: Things to Remember When 

`Route 53`: Don't forget Route 53 performs _health checks_ on AWS resources and supports a _hybrid_ model.

`Direct Connect`: Remember that Direct Connect supports a _hybrid_ model.

`Site-to-Site VPN`: Remember that a Site-to-Site VPN supports a _hybrid_ model. Don't forget to review components such as the `virtual private gateway` and `customer gateway`

### Utilizing Databases

#### Amazon Relational Database Service (RDS)

![Amazon-RDS](https://github.com/Mohsem35/AWS-Learning/assets/58659448/274a3c6d-b07d-4e68-a940-994dbc52a0ce)


RDS is a **`service`** that makes it easy to **`launch and manage relational`** databases


- Supports popular **`database engines`**
- Offers **`high availability`** and fault tolerance using **`Multi-AZ`** deployment option
- **`AWS manages`** the database with _automatic software patching,  automated backups, operating system maintenance,_ and more.
- Launch **`read replicas`** across Regions in order to provide enhanced **`performance`** and **`durability`**



#### Amazon Aurora

Aurora is a relational database compatible with **`MySQL`** and **`PostgreSQL`** that was created by AWS.

- Supports MySQL and PostgreSQL database engines
- **`5x`** faster than normal MySQL and **`3x`** faster than normal PostgreSQL
- **`Scales automatically`** while  providing durability and high availability 
- Managed by **`RDS`**

#### Amazon DynamoDB


![amazondynamodb](https://github.com/Mohsem35/AWS-Learning/assets/58659448/293e472c-fb5b-4d79-99ca-13dff8c3fe85)


DynamoDB is a fully managed _NoSQL_ **`key-value`** and **`document`** database.

- **`NoSQL`** key-value database
- Fully managed and **`serverless`**
- Non-relational
- Scales automatically to massive workloads with fast performance



#### Amazon DocumentDB

DocumentDB is a **`fully managed document database`** that supports **`MongoDB`**

- Document database
- **`MongoDB`** compatible
- Fully managed and **`serverless`**
- Non-relational



#### Amazon ElastiCache

ElastiCache is a fully managed **in-memory datastore** compatible with Redis or Memcached.

- In-memory datastore
- Compatible with **`Redis`** or **`Memcached`** engines
- **Data can be lost**
- Offers **high** performance and **low latency**

Amazon ElastiCache for Redis is fully managed, scalable, and secure. This makes it an **ideal candidate to power high-performance use cases** such as web, mobile apps, gaming, ad-tech, and IoT


#### Amazon Neptune

Neptune is a fully managed **`graph database service`** that supports highly connected datasets.


- Supports highly connected datasets like **`social media`** networks
- Fully managed and **`serverless`**
- Fast and reliable



Let's take a closer look at databases in the real world.


_Q1: Migrate an on-premises Oracle database to the cloud_
- RDS

_Q2: Migrate an on-premises PostgreSQL database to the cloud._

- RDS & Aurora

_Q3. Alleviate database load for data that is accessed often_
- ElastiCache

_Q4. Process large sets of user profiles and social interactions _

- Neptune

_Q5. NoSQL database fast enough to handle millions of requests per second._

- DynamoDB

_Q6. Operate MongoDB workloads at scale._

- DocumentDB


> _Note_: Things to Remember

RDS: RDS is only for relational databases. Don't forget the supported database engines: Amazon Aurora, PostgreSQL, MySQL, MariaDB, Oracle Database, and SQL Server.

DynamoDB: DynamoDB is a NoSQL database.

Aurora: Aurora only supports PostgreSQL and MySQL.

ElastiCache: ElastiCache is an in-memory datastore

Neptune: Neptune helps you create social media graphs.

DocumentDB: DocumentDB supports MongoDB.


### Exploring Migration and Transfer Services

A lot of companies are migrating to the cloud, and they need inexpensive, fast, and secure ways to move their on-premises data to AWS


#### Database Migration Service (DMS)

<img width="461" alt="Screenshot 2023-10-20 at 6 32 54 PM" src="https://github.com/Mohsem35/AWS-Learning/assets/58659448/52ad948d-1363-494f-8685-22085119c0aa">


DMS helps you **`migrate databases to or within AWS`**

- Migrate on-premises databases to AWS
- **`Continuous`** data replication
- Supports **`homogeneous`** and **`heterogeneous`** migrations
- Virtually **`no downtime`**



##### DMS in the Real World

Let's discuss when you would use DMS in the real world.

1. **`Oracle to Aurora MySQL`**: Migrate an on-premises Oracle database to Aurora MySQL 
2. **`Oracle to Oracle`**: Migrate an on-premises Oracle database to Oracle on EC2
3. **`RDS Oracle to Aurora MySQL`**: Migrate an RDS Oracle database to Aurora MySQL



#### Server Migration Service (SMS)

<img width="371" alt="Screenshot 2023-10-20 at 6 33 05 PM" src="https://github.com/Mohsem35/AWS-Learning/assets/58659448/c2a2f068-aff1-442d-a54e-5786ee366fc3">

SMS allows you to **`migrate on-premises servers to AWS`**

- Migrates **`on-premises`** servers to AWS
- Server saved as a new **`Amazon Machine Image (AMI)`**
- Use **`AMI`** to launch servers as **`EC2`** instances

![Screenshot from 2023-10-18 20-45-46](https://github.com/Mohsem35/AWS-Learning/assets/58659448/aa81be60-e429-4bb2-b05b-cd2806ec2150)

##### Snow Family

The Snow Family allows you to transfer **`large`** amounts of on-premises data to AWS using a **`physical device`**


**Showcone**

- The **`smallest`** member of data transport devices
- **`8 terabytes`** of usable storage
- **`Offline`** shipping
- **`Online`** with **`DataSync`**


**Showball & Snowball Edge**

- **`Petabyte`**-scale data transport solution 
- Transfer data **`in`** and **`out`**
- **`Cheaper`** than internet transfer
- Snowball Edge supports **`EC2`** and **`Lambda`**


**Showmobile**


- **`Multi-petabyte`** or **`exabyte`** scale
- Data loaded to **`S3`**
- **`Securely`** transported





#### DataSync

DataSync allows for **`online data transfer`** from on-premises to AWS storage services like **`S3 or EFS`**

- Migrates data from **`on-premises`** to AWS
- Copy data over **`Direct Connect`** or the **`internet`**
- Copy data **`between`** _AWS storage services_
- Replicate data **`cross-Region`** or **`cross-account`**





> _Note_: Things to Remember

- Snowball Edge: When going into the exam, don't forget the services natively supported by Snowball Edge, like EC2 and Lambda.

- Snowmobile: Don't forget Snowmobile is the largest member of the transport family and supports exabyte-scale data.

- Snowball: Remember that Snowball transfers petabytes of data and is cheaper than transferring over the internet.

- DataSync: Don't forget DataSync transfers data online and can be used to replicate data cross-Region or cross-account.



### Leveraging Analytics Services


Q: What is a data warehouse?

A data warehouse is a **`data storage`** solution that **`aggregates`** massive amounts of historical data from **`disparate sources`**.

Q: What are the benefits of a data warehouse?

Data warehouses support _querying, reporting, analytics, and business intelligence_. They are _not used for transaction processing_


#### Amazon Redshift
 
<img width="402" alt="Screenshot 2023-10-20 at 7 06 27 PM" src="https://github.com/Mohsem35/AWS-Learning/assets/58659448/65da6c7c-7041-44b8-9dd9-c6aa84d50d47">

Redshift is a scalable data warehouse solution

- **`Data warehousing`** solution
- Improves **`speed`** and **`efficiency`**
- Handles **`exabyte`**-scale data


##### Use Cases

1. _Data consolidation_: When you need to consolidate **`multiple data sources`** for reporting

2. _Relational databases_: When you want to run a database that **`doesn't`** require **`real-time transaction`** processing (insert, update, and delete)



#### Athena

<img width="352" alt="Screenshot 2023-10-20 at 7 06 39 PM" src="https://github.com/Mohsem35/AWS-Learning/assets/58659448/4250f5ad-abec-4e0c-8d57-490597894232">


Athena is a **`query service`** for Amazon S3

- Analyze **`S3`** data using **`SQL`**
- Pay **`per query`**
- Considered **`serverless`**



#### Glue

Glue **`prepares and load your data for analytics`**

- Extract, transform, load (**`ETL`**) service
- Helps to **`better understand`** your data



#### Kinesis

<img width="378" alt="Screenshot 2023-10-20 at 7 06 54 PM" src="https://github.com/Mohsem35/AWS-Learning/assets/58659448/eb838ed5-17c6-47b2-865d-30e2a80ad6f9">


Kinesis allows you to _analyze data_ and **`video streams`** in real time.


- Analyze real-time, **`streaming`** data
- Supports **`video`**, **`audio`**, application logs, website clickstreams, and **`IoT`**



#### Elastic MapReduce (EMR)

EMR helps you **`process large`** amounts of data

- Process **`big data`**
- Analyze data using **`Hadoop`**
- Works with **`big data`** frameworks



#### Data Pipeline

Data Pipeline helps you **`move data between`** _compute and storage services_ running either on _AWS or on-premises_


- Moves data at specific **`intervals`**
- Moves data based on **`conditions`**
- Sends **`notifications`** on success or failure


#### QuickSight

QuickSight helps you visualize your data.

- Build **`interactive dashboards`**
- **`Embed`** dashboards in your applications



Q: Search data in S3 ?
 
Athena

Q: Log analytics?

Kinesis


### Machine Learning Services


#### Rekognition

Rekognition allows you to **`automate your image and video analysis`**


- Image and video analysis
- Identify **`custom labels`** in images and videos
- **`Face and text detection`** in images and videos



##### Use cases

_Analyze pizza images_: Rekognition could help Alfredo _identify the toppings_ on his pizzas to _make sure they are being made consistently_


#### Comprehend

Comprehend is a natural-language processing (**`NLP`**) service that finds relationships in text.


- Uncovers **`insights`** and **`relationships`**
- **`Analyzes text`**


##### Use cases

_Review social media posts_: Comprehend could help Alfredo process social media posts by looking for words that show customer sentiment about his pizza — words like _delicious, tasty, cold, or bad taste_. This is a great way to tell if his customers are happy.


#### Polly

Polly **`turns text into speech`**

- **`Mimics`** natural-sounding **`human speech`**
- **`Several voices`** across many languages
- Can create a **`custom voice`**



##### Use cases

_Add complementary audio_: Polly could convert the text on a _blog post to speech that could then be downloaded or replayed in MP3 format_



#### SageMaker

SageMaker helps you _build, train, and deploy_ machine learning **`models quickly`** 


- **`Prepare data`** for models
- **`Train`** and **`deploy`** models
- Provides Deep Learning Amazon Machine Learning Images(**`AMIs`**)


##### Use cases

_Recommendation engine_: Companies like **`Netflix`** and **`Amazon`** use machine learning models to _recommend movies and products to buy_. SageMaker is a great tool for creating these models.




#### Translate

Translate provides language translation.

- Provides **`real-time`** and batch language **`translation`**
- Supports **`many languages`**
- **`Translates`** many content formats

##### Use cases

_Add localization to websites or applications_: 
Translate allows you to add localization to your applications to support your diverse user base. Translate supports several popular languages.



#### Lex

Lex helps you _build conversational interfaces_ like **`chatbots`**

- Recognizes speech and understands language
- Build highly engaging chatbots
- Powers Amazon **`Alexa`**


##### Use cases
_Integrate voice into a device:_ Amazon used the **`same technologies`** that power Lex to integrate Amazon Alexa with the Echo device.



> _Note_: Things to Remember


Comprehend: Don't forget Comprehend is used for natural language processing (NLP).

Rekognition: Don't forget Rekognition processes videos and images.

### Developer Tools

#### Cloud9

Cloud9 allows you to write code within an integrated development environment (**`IDE`**) from within your **`web browser`** 

- **`Write`** and **`debug`** code
- Supports popular **`programming languages`**


##### Use cases

_Build serverless applications_: Cloud9 preconfigures the development environment with the needed **`SDKs and libraries`**. You can easily write the code for your **`Lambda`** function directly in your web browser. 


#### CodeCommit

CodeCommit is a **`source control system`** for _private Git repositories_

- Create **`repositories`** to store code
- Commit, branch, and merge **`code`**
- Collaborate with other software developers


##### Use cases


_Manage versions of source code files for your applications_: CodeCommit can be used to manage source code and the different versions of application files.  CodeCommit is **`similar to GitHub`**



#### CodeBuild

CodeBuild allows you to build and test your application source code. 

- **`Compiles`** source code and **`runs`** tests
- Enables continuous **`integration`** and **`delivery`**
- Produces **`build s`** ready to be deployed


##### Use cases

_Run tests before deploying a new version of an application to production_: CodeBuild allows you to run as many parallel streams of tests as needed, allowing you to deploy your changes to production more quickly. 



#### CodeDeploy

CodeDeploy _manages_ the **`deployment of code`** to compute services in the cloud or on-premises.

- **`Deploys code`** to _EC2, Fargate, Lambda, and on-premises_
- Maintains application **`uptime`**

##### Use cases


_Maintain application uptime when rolling out a new version:_ CodeDeploy **`eliminates the downtime`** of your application when deploying a new version due to its rolling deployments.


#### CodePipeline

CodePipeline automates the **`software release process`**

- **`Quickly`** deliver new features and updates
- Integrates with **`CodeBuild`** to run builds and **`unit tests`**
- Integrates with **`CodeCommit`** to retrieve source code
- Integrates with **`CodeDeploy`** to deploy your changes



##### Use cases

_Add automation to the building, testing, and deployment of your application:_ When combined with other developer tools, CodePipeline helps development teams implement **`DevOps`** practices that automate testing and the movement of code to production. 


#### X-Ray

X-Ray helps you **`debug production applications`**

- **`Analyze`** and **`debug`** production applications
- **`Map`** application components
- **`View requests`** end to end

##### Use cases

_Trace calls to an RDS database_: X-Ray can help you **`map requests made to your RDS database`** from within your application. You can track information about the SQL queries generated and more.



#### CodeStar

<img width="350" alt="Screenshot 2023-10-20 at 8 30 49 PM" src="https://github.com/Mohsem35/AWS-Learning/assets/58659448/fcceac00-6654-4403-a827-3c4717f3b032">


CodeStar helps developers **`collaboratively`** work on development projects


- Developers **`connect`** their development environment
- Integrates with **`CodeCommit, CodeBuild, and CodeDeploy`**
- Contains **`issue tracking dashboard`**



##### Use cases

_CodeStar can manage the development pipeline:_



> _Note_: Things to Remember

CodeCommit: Don't forget CodeCommit offers a service similar to GitHub that works with Git repositories. 

CodeDeploy: Remember that CodeDeploy allows you to deploy an application to servers running on-premises and in the cloud.

Cloud9: Don't forget Cloud9 offers an integrated development environment (IDE) that runs inside a web browser.

CodePipeline: Don't forget CodePipeline allows you to implement a **`CI/CD`** pipeline.




### Deployment and Infrastructure Management Services

These services help you _quickly stand up new applications_, _automate the management of infrastructure_, and _provide real-time visibility into system health_


**`IaC`** allows you to write a **`script`** to provision AWS resources. The benefit is that you provision resources in a **`reproducible`** manner that saves time


```
# json script
"MyBucket" : {

      "Type" : "AWS::S3::Bucket"
 }
```
```
# yaml script
MyBucket:
    Type: AWS::S3::Bucket
```


> _Note_: There's no need to use the S3 Management Console to create a bucket


#### CloudFormation

CloudFormation allows you to **`provision AWS resources`** using Infrastructure as Code (**`IaC`**)


- Provides a **`repeatable process`** for provisioning resources
-  Works with **`most`** AWS services 
- Create **`templates`** for the resources you want to **`provision`**


##### Use cases

_Automate the infrastructure-provisioning process for EC2 servers:_ You can use CloudFormation to **`automate the creation of EC2 instances`** in your AWS account.



#### Elastic Beanstalk



Elastic Beanstalk is an easy-to-use service for **deploying** and **scaling web applications and services** developed with Java, .NET, PHP, Node.js, Python, Ruby, Go, and Docker on familiar servers such as Apache, Nginx, Passenger, and Internet Information Services (IIS)..

You can **simply upload your code**, and AWS Elastic **Beanstalk automatically handles the deployment**, from **capacity provisioning**, load balancing, and **auto scaling** to **application health monitoring**. At the same time, you retain full control over the AWS resources powering your application and can access the underlying resources at any time.

- Orchestration service that **`provisions`** resources
- Automatically handles the **`deployment`**
- **`Monitors`** application health via a **`health dashboard`**

In reality, Elastic Beanstalk is a **compute service**, but it's used when you are ready to deploy your application


_Quickly deploy a scalable Java-based web application to AWS_

<img width="764" alt="Screenshot 2023-10-20 at 8 54 19 PM" src="https://github.com/Mohsem35/AWS-Learning/assets/58659448/2818c4ba-69c5-4aab-873e-3915ddf5eb6f">




#### OpsWorks

OpsWorks allows you to use **`Chef`** or **`Puppet`** to _automate the configuration_ of your servers and deploy code.

- **`Deploy`** code and **`manage`** applications
- Manage **`on-premises`** servers or **`EC2 instances`** in AWS Cloud


##### Use cases

_Automate software configurations and infrastructure management for your application_



> _Note_: Things to Remember

CloudFormation: Don't forget CloudFormation supports infrastructure automation using Infrastructure as Code (IaC)

Elastic Beanstalk: Don't forget Elastic Beanstalk is only used to deploy applications to the AWS Cloud — it is not used to deploy applications on-premises.


OpsWorks: Remember that OpsWorks can deploy applications on-premises, and it also automates infrastructure management using Chef or Puppet.



### Utilizing Messaging and Integration Services: SQS

#### Simple Queue Service (SQS)

SQS is a message queuing service that allows you to build **`loosely coupled distributed systems`** with **`FIFO`**


- Allows **`component-to-component`** communication using **`messages`**
- Multiple components (or producers) can **`add`** messages to the **`queue`**
- Messages are processed in an **`asynchronous`** manner



##### Use cases

<img width="800" alt="Screenshot 2023-10-21 at 8 08 03 AM" src="https://github.com/Mohsem35/AWS-Learning/assets/58659448/b50589f0-a14d-481d-b691-a996fd973547">


_Build a money transfer app that performs well under heavy load:_ SQS lets you build an app that is loosely coupled, allowing components to send, store, and receive messages. The use of a messaging queue helps to improve performance and scalability. 


> _Note:_ Things to Remember


SQS: 
- Don't forget messages in queues are processed in FIFO order.
- Remember that message queues support loose coupling.



### Utilizing Messaging and Integration Services: SNS and SES


#### Simple Notification Service (SNS)

SNS allows you to **`send emails and text messages`** from your applications.

- Publish messages to a **`topic`**
- **`Subscribers`** receive messages


##### Use cases

_Send an email when CPU utilization of an EC2 instance goes above 80%:_ SNS works with **`CloudWatch`** when an alarm's metric threshold is breached to send an email.

<img width="442" alt="Screenshot 2023-10-21 at 8 17 43 AM" src="https://github.com/Mohsem35/AWS-Learning/assets/58659448/a3dd9875-65ce-4855-bbe5-09a2c4074237">



#### Simple Email Service (SES)

SES is an **`email service`** that allows you to send richly **`formatted HTML`** emails from your applications

- Ideal choice for **`marketing campaigns`** or **`professional`** emails
- Unlike SNS, SES sends **`HTML`** emails


##### Use cases

_Send a marketing email and track open or click-through rates_ 


> _Note_: Things to Remember

SNS: Don't forget SNS sends text messages and plain text emails

SES: Remember that SES sends HTML-formatted emails for marketing campaigns.



### Auditing, Monitoring, and Logging Services

1. Who signed in and made changes via the AWS Management Console?
2. What is the current load on this EC2 instance? 
3. What is the root cause of this application error?
4. Which execution path resulted in this error?



#### CloudWatch

CloudWatch is a **`collection of services`** that help you **`monitor and observe`** your cloud resources

- Collects **`metrics`**, **`logs`**, and **`events`**
- Detect **`anomalies`** in your environment
- Set **`alarms`**
- **`Visualize`** logs


_CloudWatch Alarms_: Set high resolution alarms

_CloudWatch Logs_: Monitor application logs

_CloudWatch Metrics_: Visualize **`time-series data`**

_CloudWatch Events_: **`Trigger an event`** based on a **`condition`**


##### Use cases

_Provide real-time monitoring on EC2 instances_


<img width="500" alt="Screenshot 2023-10-21 at 8 43 52 AM" src="https://github.com/Mohsem35/AWS-Learning/assets/58659448/de894384-6c10-41f8-b608-4860ac39fc32">



_Receive a notification when root user activity is detected in your account:_ Create a **`CloudWatch event rule`** to notify you when root user API calls are detected in your account indicating root user activity.

<img width="500" alt="Screenshot 2023-10-21 at 8 44 30 AM" src="https://github.com/Mohsem35/AWS-Learning/assets/58659448/bfca2724-de9f-411d-82f0-448e64d46fc6">


#### CloudTrail


CloudTrail tracks **user activity** and **API calls within your account** 

- **Log** and **retain** account activity
- Track activity through the **`console`**, **`SDKs`**, and **`CLI`**
- Identify **which user made changes**
- **Detect unusual activity** in your account
- The AWS API call history produced by CloudTrail enables _security analysis_, _resource change tracking_, and _compliance auditing_

##### Use cases of CloudTrail

_Track the time a particular event occurred in your account:_ 
You can troubleshoot events over the **past 90 days** using the **`CloudTrail event history log`** to find the **specific time** an event occurred on a **per-Region** basis. You can create a custom trail to extend past 90 days


##### Things You Can Track with CloudTrail

<img width="500" alt="Screenshot 2023-10-21 at 8 52 29 AM" src="https://github.com/Mohsem35/AWS-Learning/assets/58659448/7f3c5603-1314-4afe-9ba1-36de44efdf12">

1. Username 
2. Event time and time
3. IP Address
4. Access Key
5. Region
6. Error Code

> _Note_: Things to Remember

CloudWatch: Don't forget you can use CloudWatch to monitor your EC2 instances and notify you when certain events occur.

CloudTrail: Don't forget the things you can track with CloudTrail: username, event time and name, IP address, access key, Region, and error code.


### Exploring Additional Services


#### Amazon WorkSpaces

Amazon WorkSpaces allows you to **`host virtual desktops`** in the cloud

- Virtualize Windows or Linux desktops
- Enables employees to **`work from home`**


#### Amazon Connect

Amazon Connect is a cloud **`contact center service`**

- Provides customer service functionality
- Improves productivity of help desk agents





Q: Which service enables you to centralize and automate data protection across AWS services?

AWS backup

Q: What service could you recommend to a developer to automate the software release process?

CodePipeline

Q: Amazon EC2 offers a variety of pricing options. Which of the following EC2 pricing options is the cheapest?

Spot instances

Q: In which of the following is CloudFront content cached?

Edge Location

Q: Which of the following are true statements about Simple Queue Service (SQS)?

- Standard queues provide a loose-FIFO capability
- SQS FIFO queues always preserve the exact order

Q:Which machine learning service helps you build, train, and deploy models quickly?

SageMaker

Q: Which machine learning service allows you to add image analysis to your applications?

Amazon Rekognition

Q: Which service allows you to host virtual desktops in the cloud?

Amazon WorkSpaces

Q: Which service can you use to deploy applications both on-premises or in the cloud, using Chef or Puppet?

OpsWorks

Q: Which of the following is true of Amazon Route 53?

- Amazon Route 53 supports domain name registration.
- Amazon Route 53 performs health checks on AWS resources.
- Amazon Route 53 is a DNS service that routes users to applications.

Q: Which migration service allows you to migrate databases to or within AWS over the internet easily and securely?

AWS DMS

Q: Which AWS networking service enables you to provision a logically isolated section of the AWS cloud where you can launch AWS resources in a virtual network that you define?

Virtual Private Cloud (VPC)

Q: Which networking and content delivery service makes content globally available with low latency?

Amazon CloudFront

Q: What is CloudWatch?

It is a collection of services designed to monitor and observe cloud resources.

Q: Which AWS service can send both text and email messages from your applications?

Simple Notification Service (SNS)

_Q: Objects stored in S3 are stored in a single, central location within AWS._

False

True: Objects stored in S3 are stored in multiple servers, in multiple facilities across AWS.


_Q: Which services allow you to build hybrid environments by connecting on-premises infrastructure to AWS_
- Site-to-Site VPN
- AWS Direct Connect

_Q: Which service is used to allow resources in your VPC to access the internet?_

Internet Gateway

_Q: Which service allows you to practice Infrastructure as Code by provisioning your AWS resources via scripted templates?_

AWS CloudFormation

_Q: Which services allow you to run containerized applications without having to manage servers or clusters?_

- Amazon Elastic Container Service (Amazon ECS)
- Amazon Elastic Kubernetes Service (EKS)
- AWS Fargate

_Q: What data transport solution allows moving terabytes to petabytes of data to AWS, with additional capability of running computing locally, even when there is no network connection available?_

AWS Snowball Edge

_Q: Which storage service is a scalable file system that only works with Linux-based workloads?_

Amazon Elastic File System (EFS)

_Q: Which service routes user traffic through AWS's global network infrastructure to ensure low latency for your gaming application?_

AWS Global Accelerator

Which database services make it easy for you to set up, operate, and scale relational databases in the cloud?

- Amazon Relational Database Service (RDS)
- Amazon Aurora

Q: Which monitoring service helps you observe your cloud resources and provides actionable insights?

CloudWatch

Q: Which AWS service provides a secure and resizable compute platform with choice of processor, storage, networking, operating system, and purchase model?

EC2

Q: Which machine learning service allows you to add image analysis to your applications?

Amazon Rekognition

Q: What AWS services are used for notifications and messaging?

- Simple Email Service (SES)
- Simple Notification Service (SNS)

Q: In which of the following is CloudFront content cached?

Edge Location

Which service supports workloads that need to remain on-premises due to latency or data sovereignty needs?

AWS Outposts

Q: Objects stored in S3 are stored in a single, central location within AWS.

False

Q: Which EC2 storage mechanism is recommended when running a database on an EC2 instance?

AWS EBS

Q:Which EC2 pricing option is best for short-term, irregular workloads that should not be interrupted?

On-Demand

Q: Which machine learning service helps you build, train, and deploy models quickly?

Sagemaker

Which services allow you to send emails from your applications?

#### chapter 3
### Security and Compliance 
#### (25%)

#### Shared Responsibility Model

In the public cloud, there is a shared security responsibility between you and AWS.

`AWS' Responsibility`: Security **`of`** the Cloud
`Your Responsibility`: Security **`in`** the Cloud

#### Security of the Cloud
AWS is responsible for _protecting and securing their infrastructure_

1. _AWS Global Infrastructure_: AWS is responsible for its global infrastructure elements: **`Regions`**, **`edge locations`**, and **`Availability Zones`**
2. _Building Security_: AWS controls access to its **`data centers`** where your data resides.
3. _Networking Components_: AWS maintains networking components: **`generators`**, uninterruptible power supply (**`UPS`**) systems, computer room air conditioning (**`CRAC`**) units, **`fire suppression systems`**, and more
4. _Software_: AWS is responsible for any **`managed service`** like **`RDS`**, **`S3`**, **`ECS`**, or **`Lambda`**, **`patching of host operating systems`**, and **`data access endpoints`**

#### Security in the Cloud

You are responsible for how the services are implemented and managing your application data. 

1. _Application Data_: You are responsible for **`managing application data`**, which includes **`encryption`** options.
2. _Security Configuration_: You are responsible for securing your **`account and API calls`**, **`rotating credentials`**, **`restricting internet access from your VPCs`**, and more.

3. _Patching_: You are responsible for the **`guest operating system (OS)`**, which includes _updates and security patches._

4. _Identity and Access Management_: You are responsible for **`application security and identity and access management.`**

5. _Network Traffic_: You are responsible for **`network traffic protection`**, which includes **`security group firewall configuration.`**

6. _Installed Software_: You are responsible for your **`application code`**, **`installed software`**, and more. You should frequently _scan for and patch vulnerabilities in your code._


##### Who is responsible for what?

Firewall configuration - you

Data center security for physical building -  AWS

Encryption of EBS volumes - you

Language version of Lambda - AWS

Taking DB backups in RDS - you

Updating the firmware on the underlying EC2 hosts - AWS

Ensuring data is encrypted at rest - you

Managing the network infrastructure - AWS

Patching the guest operating system for EC2 - you

Physically destroying storage media at end of life - AWS



#### Well-Architected Framework

The **`6 pillars`** of the Well-Architected Framework describe **key concepts**, **design principles** and **best practices for running workloads** in the cloud.

<img width="301" alt="Screenshot 2023-10-24 at 6 44 56 PM" src="https://github.com/Mohsem35/AWS-Learning/assets/58659448/2052e08d-d5b8-407b-a5ed-75805489ced0">


##### Real-world use cases of well-architected framework


OS RP CS

1. **`Operational Excellence`**: The operational excellence pillar focuses on **running and monitoring systems**, and **continually improving processes and procedures**. You can use AWS **`CodeCommit`** for version control to enable tracking of code changes and to version-control **`CloudFormation`** templates of your infrastructure

2. **`Security`**: The security pillar focuses on **protecting information and systems**. You can configure **central logging** of all actions performed in your account using **`CloudTrail`**

3. **`Reliability`**: The reliability pillar focuses on workloads **performing their intended functions** and how to **recover quickly from failure** to meet demands. You can use Multi-AZ deployments for enhanced availability and reliability of **`RDS databases`**

4. **`Performance Efficiency`**: The performance efficiency pillar focuses on **structured** and **streamlined allocation of IT and computing resources**. You can use AWS **`Lambda`** to run code with zero administration


5. **`Cost Optimization`**: The cost optimization pillar focuses on **avoiding unnecessary costs**.You can use **`S3 Intelligent-Tiering`** to automatically move your data between access tiers based on your usage patterns


6. **`Sustainability`**: The sustainability pillar focuses on **minimizing the environmental impacts of running cloud workloads**. You can use **`EC2 Auto Scaling`** to ensure you are _maximizing utilization_

> _Note_: Things to Remember

Well-Architected Framework: Going into the exam, remember the 6 pillars and their real-world use cases



#### IAM Users 


#### 1. Identity and Access Management (IAM)

![AWS-Identity-and-Access-Management_IAM](https://github.com/Mohsem35/AWS-Learning/assets/58659448/b3776656-39b0-48cc-a618-03ae81699ce9)


IAM allows you to **`control`** access to your **`AWS services`** and **`resources`** 

- Helps you **`secure`** your cloud resources
- You define **`who`** has access
- You define **`what`** they can do
- A **`free global service`**

<img width="361" alt="Screenshot 2023-10-24 at 7 09 21 PM" src="https://github.com/Mohsem35/AWS-Learning/assets/58659448/dddcf3d6-f59b-4930-b26c-1d4b579586bf">



##### Identities vs. Access 

_Identities_: **Who** can access your resources

- _Root user_
- _Individual users_
- _Groups_
- _Roles_


_Access_: **What** resources they can access

- Policies
- AWS managed policies
- Customer managed policies
- Permissions boundaries


##### Authentication ("Who") vs. Authorization ("What")

Authentication is where you present your identity (_username_) and provide verification (_password_) where Authorization determines _which services and resources the authenticated identity has access to_


#### 2. Users

Users are entities you create in IAM to represent the **`person`** or **`application`** _needing to access your AWS resources_



**1. ROOT USER**

The root user is created when you _first open your AWS account_

What can only the root user do?
- Close your account
- Change email address 
- Modify your support plan

**2. INDIVIDUAL USER**

_Individual users are created in IAM and are used for everyday tasks_

What can individual users do?

- Perform **administrative tasks** 
- Access application code
- Launch EC2 instances
- **Configure databases**

Don't forget activity performed by users in your account is **`billed`** to your account!


**3. APPLICATIONS**

Did you know applications can be users?

You'll create a user in IAM so you can generate access keys for an _application running on-premises that needs access to your cloud resources_

_Applications can also be user_

<img width="550" alt="Screenshot 2023-10-24 at 7 39 12 PM" src="https://github.com/Mohsem35/AWS-Learning/assets/58659448/a7e8dc51-0829-43a6-95ec-5166a34d6f06">


<img width="550" alt="Screenshot 2023-10-24 at 7 38 56 PM" src="https://github.com/Mohsem35/AWS-Learning/assets/58659448/c5d171bf-6b86-424a-bd9d-48d64998131d">

##### The least privilege principle

The principle of least privilege involves giving a user the **`minimum access`** required to get the job done.



#### 3. GROUP 

**GROUPS**: A group is a **`collection of IAM users`** that helps you apply common access controls to all group members.

`Administrators`: Administrators perform administrative tasks such as **`creating new users`**

`Developers`: Developers use **`compute and database services`** to build applications.

`Analysts`: Analysts run **`budget and usage reports`**

> **_Note:_** Do not confuse security **groups for EC2 with IAM groups**. EC2 security groups act as **firewalls**, while IAM groups are **collections of users**.


KEY TAKEAWAYS 

**IAM Groups**

- [x] Used to group users that perform similar tasks.
- [x] Access permissions apply to all members of the group.
- [x] Access is assigned using policies and roles.


> _Note_: Things to Remember

_Users and groups_: Going into the exam, understand the differences between users and group.

_Root user tasks_: Remember the tasks that only the root user can do. 

_Principle of least privilege_: Don't forget about the principle of least privilege

_Real-world use cases_: Don't forget the real-world use cases for IAM.



#### IAM Permissions

#### Roles

Roles define **access permissions** and are _temporarily assumed by an IAM user or service_

##### KEY TAKEAWAYS
 
Roles

1. You assume a role to perform a task in a **`single session`**
2. Assumed by any **`user or service`** that needs it.
3. Access is assigned **`using policies`**
4. You grant **`users in one AWS account`** access 

<img width="750" alt="Screenshot 2023-10-24 at 8 33 50 PM" src="https://github.com/Mohsem35/AWS-Learning/assets/58659448/168b501b-9c3d-4660-bc2a-6b93acd5b1d7">


|   | Role | AWS Services  |
| ------------- | ------------- | ------------- |
| User  | DevOps-Engineer Role  | CodeCommit, CodePipeline
| Lambda  | Lambda-Execution Role | S3, DynamoDB 


##### Roles in Real World

**`Attach a role to an EC2 instance for access to S3`**: You can attach a role to an instance that provides privileges (e.g., uploading files to S3) to applications running on the instance. Roles help you avoid sharing long-term credentials like access keys and protect your instances from unauthorized access.

<img width="500" alt="Screenshot 2023-10-24 at 8 35 10 PM" src="https://github.com/Mohsem35/AWS-Learning/assets/58659448/e3d05220-091f-44e2-8f3d-26428a1f5b6d">


#### Policies

You _manage permissions for IAM users, groups, and roles_ by **creating a policy document** in **`JSON format`** and attaching it.

1. **`Custom policy`** for User

<img width="500" alt="Screenshot 2023-10-24 at 8 40 28 PM" src="https://github.com/Mohsem35/AWS-Learning/assets/58659448/e0447371-d23c-49b2-b3dd-3c53e72ee8be">


2. **`Managed Policy`** for Developer Group & Role

<img width="500" alt="Screenshot 2023-10-24 at 8 40 41 PM" src="https://github.com/Mohsem35/AWS-Learning/assets/58659448/77167f0c-350a-4744-98c1-dc993729c0b2">

> _Note:_ If you're going to use an AWS-managed policy, just make sure you look at the policy
and you understand everything that it really gives access to.

<img width="500" alt="Screenshot 2023-10-24 at 8 41 20 PM" src="https://github.com/Mohsem35/AWS-Learning/assets/58659448/ceaec967-8b64-47f6-a0dd-084512f7a62c">


##### Policies in the Real World

**You can limit access to an Amazon S3 bucket to specific users**: You can add a bucket access policy directly to an Amazon S3 bucket to grant IAM users access permissions for the bucket and the objects in it.


##### IAM Best Practices

1. **`Enable MFA for privileged users`**: You should enable multi-factor authentication (MFA) for the root user and other administrative users.

2. **`Implement strong password policies`**: You should require _IAM users to change their passwords after a specified period of time_, _prevent users from reusing previous passwords_, and _rotate security credentials regularly_

3. **`Create individual users instead of using root`**: You _shouldn't use the root user for daily tasks_

4. **`Use roles for Amazon EC2 instances`**: You should _use roles for applications_ that run on EC2 instances _instead of long-term credentials like access keys_


#### IAM Credential Report

The IAM credential report lists all users in your account and the status of their various credentials.

- Lists all users and status of **`passwords`**, **`access keys`**, and **`MFA`** devices
- Used for **`auditing`** and **`compliance`**



> _Note_: Things to Remember

Users, groups, roles, and policies: Going into the exam, understand the differences between users, groups, roles, and policies.

IAM best practices: Don't forget to familiarize yourself with IAM best practices.

Real-world use cases: Don't forget the real-world use cases for IAM.

IAM credential report: Don't forget the importance of the IAM credential report




#### AWS Security Services (Software Based)


AWS has several _software-based security tools_ available to help you _monitor and protect_ your resources


#### Web Application Firewall (WAF)

WAF helps protect your web applications against **`common web attacks`**

- **`Protects`** apps against common attack patterns
- Protects against **`SQL injection`**
- Protects against **`cross-site scripting`**

##### WAF in the Real World


You can deploy a web application directly to an EC2 instance and protect it _from cross-site scripting attacks using WAF_. You can even deploy **`WAF on CloudFront`** as part of your **CDN solution** to **`block malicious traffic`**

<img width="500" alt="Screenshot 2023-10-24 at 9 38 16 PM" src="https://github.com/Mohsem35/AWS-Learning/assets/58659448/c1cfa428-f24d-4933-8f18-735cc44fe05d">


Have you heard about DDoS?

A DDoS attack causes a **`traffic jam`** on a website or web application in an attempt to cause it to crash.

<img width="700" alt="Screenshot 2023-10-24 at 9 39 06 PM" src="https://github.com/Mohsem35/AWS-Learning/assets/58659448/41591560-b1c4-4d6a-bb0f-d29a94c6d103">


#### Shield

Shield is a managed Distributed Denial of Service (**`DDoS`**) _protection service_

- **`Always-on`** detection
- Shield **`Standard`** is free
- Shield **`Advanced`** is a **paid** service


1. _Shield Standard_: Provides **`free`** protection against common and frequently occurring attacks

2. _Shield Advanced_: Provides enhanced protections and 24/7 access to AWS experts for a **`fee`**


DDoS protection via Shield Advanced is supported on several services

<img width="500" alt="Screenshot 2023-10-24 at 9 44 48 PM" src="https://github.com/Mohsem35/AWS-Learning/assets/58659448/66cfb548-0693-4fff-bd96-35359e234b50">



##### Shield in the Real World


Shield Advanced will give you _notifications of DDoS attacks_ via **`CloudWatch metrics`**.Additionally, with Shield Advanced, you have 24/7 access to AWS experts to assist during an attack. 


#### Macie

Macie helps you **`discover and protect sensitive data`**

- Uses **`machine learning`** 
- Evaluates **`S3`** environment
- Uncovers **`personally identifiable information`** (PII) 



##### Macie in the Real World


Macie can be used to find sensitive data like **`passport numbers`**, **`social security numbers`**, and **`credit card numbers`** on S3.


> _Note:_ Things to Remember


WAF: Going into the exam, don't forget WAF protects against SQL injection and cross-site scripting attacks.

Shield: Don't forget Shield provides DDoS protection and works with CloudFront, Route 53, Elastic Load Balancing, and AWS Global Accelerator.


Macie: Remember that Macie helps you find sensitive information. 


#### Additional Security Services

#### Config

![AWS-Config](https://github.com/Mohsem35/AWS-Learning/assets/58659448/d1a025b9-e9be-4ff9-81f8-bdc100947a94)

Config allows you to _assess, audit, and evaluate_ the **`configurations`** of your resources

- **`Track configuration changes`** over time
- Delivers _configuration history_ file to **`S3`**
- Notifications via Simple Notification Service (**`SNS`**) of **every configuration change**


##### Config in the Real World

_Identify system-level configuration changes made to your EC2 instances_: Config allows you to record configuration changes within your EC2 instances. You can view **`network`**, **`software`**, and **`operating system (OS)`** configuration changes, **`system-level updates`**, and more



#### GuardDuty

GuardDuty is an **intelligent threat detection** system that **`uncovers unauthorized behavior`**

- Uses **`machine learning`**
- **`Built-in detection`** for EC2, S3, and IAM 
- Reviews CloudTrail, VPC Flow Logs, and DNS **`logs`**


##### GuardDuty in the Real World

_Detect unusual API calls in your account_: GuardDuty's anomaly detection feature **`evaluates all API requests`** in your account and identifies events that are associated with common techniques used by **`attackers`** 


#### Inspector

Inspector **`works with EC2`** instances to **`uncover and report`** **vulnerabilities**

- Agent installed on EC2 instance 
- **`Reports vulnerabilities`** found
- **`Checks`** access from the **`internet`**, **`remote root login`**, **`vulnerable software versions`**, etc.

##### Inspector in the Real World

_Identify unintended network access to an EC2 instance via a detailed report of security findings:_ Inspector has several built-in rules to access your EC2 instances to find vulnerabilities and report them prioritized by level of severity.



#### Artifact

![pict--aws-artifact-aws-security,-identity-and-compliance-vector-stencils-library](https://github.com/Mohsem35/AWS-Learning/assets/58659448/0680d2c8-12ac-405a-a1ed-01bd84b3751e)


Artifact offers on-demand access to **`AWS security and compliance reports`**

- Central repository for **`compliance reports`** from third-party auditors
- _Service Organization Controls_ (**`SOC`**) reports
- _Payment Card Industry_ (**`PCI`**) reports


##### Artifact in the Real World

_You need to access AWS' certification for ISO compliance:_ Artifact provides a central repository for AWS' security and compliance reports via a **`self-service portal`**


#### Cognito

Cognito helps you **`control access to mobile and web applications`**


- Provides **`authentication`** and **`authorization`**
- Helps you **`manage users`** 
- Assists with **`user sign-up`** and **`sign-in`**


##### Cognito in the Real World


_You need to add a social media sign-in to your web application:_ Cognito provides functionality that allows your users to sign in to your application through social media accounts like **`Facebook`** and **`Google`**

> _Note_: Things to Remember


Config: Remember that Config allows you to identify changes to various resources over time.

GuardDuty: Don't forget GuardDuty identifies malicious or unauthorized activities in your AWS account.

Inspector: Don't forget Inspector **`only works for EC2 instances`**

Artifact: Don't forget Artifact provides you with compliance reports

Cognito: Don't forget Cognito controls access to mobile and web applications



#### Data Encryption and Secrets Management Services

Data encryption **`encodes`** data so it **`cannot be read`** by unauthorized users

data in flight vs. data at rest




**Data in Flight VS. Data at Rest**

_Data in Flight_: Data in Flight also called data in **`transit`** or data in motion

- **`Data`** that is moving from **`one location to another`**
- An **`API`** that queries the **`database`** to send data back to the **`front end application`** or sending a text message, or data that is going across the internet or a **`private network`**


_Data at Rest_: Data that is **`inactive or stored`** for later use

- Think about data stored in **`S3`** or in a database like **`MySQL`**



#### Key Management Service (KMS)

KMS allows you to generate and store encryption keys

- **`Key generator`**
- **`Store`** and **`control`** keys
- **`AWS manages`** encryption keys
- Automatically **`enabled`** for certain services like **CloudTrail logs**, **S3 Glacier**, and **Storage Gateway**



##### KMS in the Real World

_Create encrypted Amazon EBS volumes:_ When you create an encrypted Amazon **`EBS`** volume, you're able to specify a KMS customer **`master key`**



#### CloudHSM

CloudHSM is a **`hardware security module`** (HSM) used to **`generate encryption keys`**

- **`Dedicated hardware`** for security
- Generate and manage your **`own`** encryption keys
- AWS does **`not`** have access to your keys


##### CloudHSM in the Real World


CloudHSM allows you to _meet corporate, contractual, and regulatory compliance requirements for data security_ by using dedicated hardware in the cloud.


#### Secrets Manager

Secrets Manager allows you to **`manage`** and **`retrieve secrets`** (passwords or keys)

- Rotate, manage, and retrieve secrets
- **`Encrypt`** secrets at rest
- **`Integrates`** with services like **RDS**, **Redshift**, and **DocumentDB**

##### Secrets Manager in the Real World

_Retrieve database credentials needed for your application code:_ Secrets Manager allows you to **`retrieve database credentials with a call to Secrets Manager APIs`**, _removing the need to hardcode sensitive information in plain text_ within your application code.


> _Note:_ Things to Remembe

KMS: Going into the exam, don't forget **`AWS manages KMS keys`**

CloudHSM: Don't forget **`you manage`** the keys generated with CloudHSM

Secrets Manager: Don't forget Secrets Manager has built-in integration for RDS, Redshift, and DocumentDB.


_Which service can integrate with a Lambda function to automatically take remediation steps when it uncovers suspicious network activity when monitoring logs in your AWS account?_

Amazon GuardDuty

_Which of the following are tasks that only the root user can complete?_


- Change the account name and email address.
- Close your AWS account.

_In the shared responsibility model, what is the customer responsible for?_

- Firewall configuration and application security
- Patching the guest operating system (OS)

_Which service protects your web application from cross-site scripting attacks?_

AWS Web Application Firewall (WAF)

_Which service helps you control access to mobile and web applications?_

Cognito

_What is the purpose of CloudHSM?_

Its purpose is to enable you to easily create and use your own encryption keys

_How do you manage permissions for multiple users at once using AWS Identity and Access Management (IAM)?_

Groups

_Which service allows you to locate credit card numbers stored in Amazon S3?_

Amazon Macie

_Which service has a feature that can assist with compliance and auditing by offering a downloadable report that provides the status of passwords and MFA devices in your account?_

AWS Identity and Access Management (IAM)

_Which service allows you to generate encryption keys managed by AWS?_

AWS Key Management Service (KMS)

_Select the TRUE statement regarding the pillars of the AWS Well-Architected Framework._


- The Performance Efficiency pillar enables the ability to use computing resources efficiently as demand and technology changes.


- The Security pillar enables the ability to protect data, systems, and assets to improve your cloud security.


- The Operational Excellence pillar enables the ability to support development, run workloads effectively, gain operational insights, and improve supporting processes and procedures.

_Which service allows you to create access keys for someone needing to access AWS via the command line interface (CLI)?_

AWS Identity and Access Management (IAM)


#### chapter 4
### Pricing, Billing and Governance 
#### (16%)

### AWS Pricing

There are 3 fundamental drivers of cost

1. **`Compute`**: Hourly from launch to termination
2. **`Storage`**: The data you store in the cloud
3. **`Outbound data transfer`**: Data in flight moving between systems


**Free Offer Types**

There are 3 different types of free offers available depending on the service you choose


1. _12 months free_: 12 months' free usage following your initial sign-up date to AWS

2. _Always free_: Offers do not expire and are available to all AWS customers

3. _Trials_: Short-term free trials starting from the date you activate a particular service


> _Note:_ AWS services are priced independently!

##### EC2 Pricing

Don't forget, there are 5 ways to pay for Amazon EC2 instances.

<img width="550" alt="Screenshot 2023-10-28 at 12 46 48 PM" src="https://github.com/Mohsem35/AWS-Learning/assets/58659448/e02c52d4-e6af-451c-baa5-73d97c1a1efb">


##### Lambda Pricing

Don't forget how you're charged when using Lambda.

<img width="500" alt="Screenshot 2023-10-28 at 2 06 08 PM" src="https://github.com/Mohsem35/AWS-Learning/assets/58659448/b256f531-3bde-408b-be81-de42cea7b464">

##### S3 Pricing

Don't forget with S3, **`you pay for the storage you use`**
![Uploading Screenshot 2023-10-28 at 12.56.35 PM.png…]()

- _Storage class_: various **`storages`** classes

- _Storage_: **`number`** and **`size`** of objects
- _Data transfer_: data **`transferred out`** of S3 region 
- _Request and data retrieval_: requests made for **`data`** and amounts of **`requests`**


##### RDS Pricing

Let's discuss the RDS features that **`drive pricing`**

1. _Running clock hours_
2. _Type of database_
3. _Storage_
4. _Purchase type_
5. _Database count_
6. _API requests_
7. _Deployment type_
8. _Data transfer_

#### Total Cost of Ownership (TCO)?

TCO is a **`financial estimate`** that helps you understand both the **`direct`** and **`indirect`** costs of AWS.

> _Note:_ There used to be a `TCO Calculator` that is **`no longer available`**. However, you will see the term TCO on the exam, so understanding what it means is important. 


#### Application Discovery Service

Application Discovery Service helps you **plan migration projects to the AWS Cloud**

- Plan **`migration`** projects
- Used to **`estimate TCO`**
- Works with other services to **`migrate servers`**


##### A Few Ways to Reduce Your TCO Using AWS


1. **Minimize capital expenditures**: AWS helps you **`minimize large capital expenditures`**, which reduces your TCO.


2. **Utilize Reserved Instances**: AWS provides **`Reserved Instances`** to help you lock in savings and reduce your TCO.

3. **Right size your resources**: AWS helps you **`match`** the **`provisioning`** of resources to your **`usage needs`** to reduce your TCO.


#### AWS Price List API

The Price List API allows you to **`query`** the price of AWS services


- **Query** using **`JSON`** or **`HTML`**
- Receive **`price alerts`** when prices change 


> _Note_: Things to Remember

_Pricing Calculator_: Don't forget the Pricing Calculator helps you calculate the TCO.

_TCO_: Don't forget the ways **`a company can reduce their TCO`**.

_Pricing_: Don't forget how pricing is calculated for EC2, Lambda, S3, and RDS.

_Price List API_: Don't forget the Price List API is one way to determine the cost of services.




### Billing Services

There are several tools available to help you **`track`** your **`ongoing spend`**

#### Budgets

Budgets allows you to set custom budgets that **`alert`** you when your costs or usage **`exceed`** your budgeted amount.

- Improve **`planning`** and **`cost control`**
- **`Cost`**, **`usage`**, and **`reservation`** budgets
- Budget alerts

##### Budget Types

- _Cost Budgets:_ Plan how much you want to **`spend`** on a service
- _Usage Budgets:_ Plan how much you want to **`use`** on one or more services
- _Reservation Budgets:_ Set Rls or Savings Plans **`utilization`** or coverage **`targets`**.


##### Budgets in the Real World


_Monitor Free Tier usage so you don’t incur unwanted costs:_ You can monitor Free Tier usage to ensure you don't accidentally exceed Free Tier limits and incur unwanted costs. You can set up an alert notification for when your account is approaching a particular dollar amount.


#### Cost and Usage Report

The Cost and Usage Report contains the most **comprehensive set of cost and usage data**.

- **`Aggregate`** usage data on a _daily, hourly, or monthly level_


##### Cost and Usage Report in the Real World

_View the most granular data about your AWS bill_: The Cost and Usage Report gives you the ability to do a deep dive into your AWS cost and usage data. Once set up, you can download the report using the Amazon S3 console.


#### Cost Explorer

![AWS-Config](https://github.com/Mohsem35/AWS-Learning/assets/58659448/d1a025b9-e9be-4ff9-81f8-bdc100947a94)

Cost Explorer allows you to **`visualize and forecast`** your costs and usage over time

- Visualize costs over time
- View **`past 12 months`**
- **`Forecast`** for up to 12 months

##### Cost Explorer in the Real World

_Analyze your EC2 usage over the past 7, 30, or 60 days_: If you are considering your options for Savings Plans, AWS Cost Explorer can analyze your EC2 usage over the past **`7, 30, or 60`** days.



#### Cost Allocation Tags

Tags are useful for **`tracking spend`**

1. Tags allow you to **`label`** resources using a **`key and value pair`**

2. Tags allow you to **`track`** costs via the cost allocation **`report`**


> _Note:_ Things to Remember

Budgets: Going into the exam, don't forget you can be alerted when your usage exceeds a defined threshold using Budgets.

Cost and Usage Report: Remember that the Cost and Usage Report provides the most detailed set of AWS cost and usage data available.

Cost Explorer: Don't forget Cost Explorer helps you visualize and forecast spending.

Cost Allocation Tags: Don't forget that tags can help you track spend.


### Governance Services


**`Governance`** and management services help you **`maintain control`** over **cost**, **compliance**, and **security** **`across`** your AWS accounts.

#### Organizations

![images](https://github.com/Mohsem35/AWS-Learning/assets/58659448/9fac1156-57e0-442e-944b-04f3b4047d5e)


Organizations allows you to centrally **`manage multiple AWS accounts under one umbrella`** 

- Group **`multiple`** accounts
- **`Single payment`** for all accounts
- **`Automate`** account creation
- _Allocate resources and apply policies_ **`across accounts`**




1. **Master Payer/Root Organization**: An organization is an entity that allows you to **`consolidate multiple AWS accounts into one`**. And that root account is called the master payer account, and it _pays for all member accounts using what's called consolidated billing._




2. **Service control policies(SCP)**: are a _type of organization policy_ that you can use to manage permissions in your organization. They are used to **`enforce permissions`** that you want **`everyone`** in the organization to follow.

3. **Organization units(OUs)**: Are a **`groupings of AWS accounts`** that are similar. In this example, **`accounts are grouped by departmental area`**. We have the _IT organization_, we have the _Shared Services organization_ and we have the _Marketing organization_

4. **Member accounts**: Member accounts are the standard **`individual AWS accounts`**
that contain your AWS resources


##### What are the benefits?

Organizations offers many benefits

1. _Consolidated Billing_: The advantage of consolidated **`billing`** is that you receive **`one bill`** for multiple accounts.

2. _Cost Savings_: You'll receive **`volume discounts`** since usage is combined across accounts. 

3. _Account Governance_: You have a quick and automated way to **`create`** accounts or **`invite`** existing accounts. 


##### Organizations in the Real World


_Reduce costs by sharing resources across accounts_: Organizations allows you to save money using **`Reserved Instance (RI) sharing`**. RI sharing allows all accounts in the organization to receive the **`hourly cost-benefit of RIs`** purchased by any other account. You can always _turn off RI sharing using the master payer (or root) organization_


#### Control Tower

Control Tower helps you ensure your accounts **`conform`** to _company-wide policies_

- Helps set up **`new accounts`** using a multi-account strategy
- **`Works`** directly with **AWS Organizations**
- Enforces the **`best use of services`** across accounts
- Provides a **`dashboard`** to manage accounts

##### Control Tower in the Real World

_Disallow public write access to all S3 buckets across your accounts:_ Control Tower allows you to **`govern your multi-account`** environment by enabling **`cross-account security audits`** or preventing or detecting security issues through mandatory or optional **`guardrails`**



#### Systems Manager

Systems Manager gives you **`visibility`** and **`control`** over your **`AWS resources`**

- **`Automate`** operational **`tasks`** on your resources
- **`Group resources`** and take **`action`**
- **`Patch`** and **`run commands`** on multiple EC2 instances or manage RDS instances


##### Systems Manager in the Real World


_Deploy operating system and software patches automatically across a large group of instances:_ Systems Manager allows you to auto-patch software running on EC2 instances according to a schedule.


#### Trusted Advisor

![AWS-Trusted-Advisor](https://github.com/Mohsem35/AWS-Learning/assets/58659448/11189983-2504-403b-9e78-68d504f12f97)


Trusted Advisor provides **`real-time guidance`** to help you **`provision your resources`** following AWS best practices. 

- Helps you understand **`best practices`**

Here are a few popular recommendations made by Trusted Advisor

_Free Check_

_EC2_: Checks for unrestricted access for specific **`ports`** on EC2 instances

_S3_: Checks S3 **`bucket permissions`** to determine if public access

_Root User_: Checks for multi-factor authentication (**`MFA`**) on root account 

_RDS_: Checks for RDS **`public snapshots`**


_Enterprise or Business support required_

_IAM_: Checks IAM **`password policy`**

Checks for service usage greater than **`80% over service limit`**

_Keys_: Checks for **`exposed access keys`**

_CloudFront_: Checks for CloudFront content delivery **`optimization`**


##### Trusted Advisor in the Real World



_Check read and write capacity service limits for DynamoDB:_ Trusted Advisor helps **`reduce your overall costs by monitoring service limits`**



#### License Manager

License Manager helps you manage software licenses
- Manage **`on-premises`** and **`AWS licenses`**
- Track licenses for **`Oracle`**, **`Microsoft`**, **`SAP`**, and more



#### Certificate Manager

Certificate Manager helps you provision and manage **`SSL/TLS certficates`**

- Provides **`public`** and **`private`** certificates for **`free`**
- Integrates with **`Elastic Load Balancing`**, **`API Gateway`**, and more


> _Note:_ Things to Remember

Organizations: Don't forget Organizations saves you money through consolidated billing. Also, remember the importance of SCPs.

Control Tower: Don't forget Control Tower helps you enforce best use of services across your organization.

Systems Manager: Remember that Systems Manager helps you maintain your resources through automatic patching and updates.

Trusted Advisor: Remember the recommendations made by Trusted Advisor.

License Manager: Remember that License Manager helps you manage on-premises or AWS-based Oracle licenses.

Certificate Manager: Remember that Certificate Manager provides free public certificates.


### Utilizing Management Services

There are expert teams available that help you _manage_ and _operate_ your cloud environment. 

#### Managed Services

Managed Services helps you efficiently **operate your AWS infrastructure**

- **Augments** your internal staff
- Provides **ongoing management** of your **infrastructure**
- **Reduces operational risks** and overhead


##### Managed Services in the Real World

_Develop application-specific health monitoring using CloudWatch_: Managed services can increase your operational efficiency by helping you develop application-specific health monitoring using CloudWatch.


#### Professional Services

Professional Services helps enterprise customers **move to a cloud-based operating model**

- **Implements** solutions

##### Professional Services in the Real World


_Get help with evaluating an application for migration to the cloud_: You can quickly move on-premises applications to the cloud using AWS Professional Services.


#### AWS Partner Network (APN)

APN is a **global community** of approved partners that offer software solutions and consulting services for AWS

- Offers **technology** partners that provide **software solutions**
- Provides **consulting** partners that offer **professional services**
- Find **approved vendors** with deep AWS expertise



##### APN in the Real World

_You need help designing and building a new application_: If your team lacks the technical expertise to build and deploy cloud applications, the APN could help you get up and running quickly.



#### Marketplace

Marketplace is a digital catalog of prebuilt solutions you **can purchase or license**. You may also **sell your own solutions** to others via Marketplace

- **Buy** third-party software
- **Sell** solutions to AWS customers
- **Search** the catalog of software listings and install with the click 
of a button


##### Marketplace in the Real World

_Try out an application before making a long-term commitment_: Some products listed on Marketplace offer free trials. The free trial allows you to try the software before you buy it


#### Personal Health Dashboard

Personal Health Dashboard **alerts you to events** that might impact your AWS environment and remediation guidance

- Provides **troubleshooting guidance** 
- Feedback tailored to your **specific environment**

While the **Service Health Dashboard** displays the **general status of AWS services**, AWS Health Dashboard gives you a **personalized view** into the performance and availability of the AWS services underlying your AWS resources

With AWS Health Dashboard, **alerts are automatically triggered by changes** in the health of AWS resources, giving you **event visibility and guidance** to help quickly diagnose and resolve issues.

> _Note:_ Things to Remember

Managed Services: Don't forget Managed Services augments your staff and helps improve your overall operational efficiency

Marketplace and APN: Remember that AWS recognizes partners and providers from these networks

Professional Services: Don't forget Professional Services can help you migrate from on-premises to the cloud. 

Personal Health Dashboard: Don't forget Personal Health Dashboard provides tailored advice.


### Exploring Support Plans


#### Support Plans

There are 4 support plans.

1. **`Basic`**: Basic Support is included for **free** for all AWS accounts. 

- Account and billing, 
- Service limit increases

Customer Service: 24/7 access via email only

2. **`Developer`**: Developer Support starts at **$29** a month and is recommended for **testing and development**.

- Account and billing, 
- Service limit increases
- Technical support

1 primary contact, unlimited cases

Customer Service: Business-hours access via email only

3. **`Business`**: Business Support starts at **$100** a month and is recommended for **production workloads**.

- Account and billing, 
- Service limit increases
- Technical support

Unlimited Contacts, Unlimited Cases, **Full Set** of Trusted Advisor Checks

Customer Service: 24/7 access via email, phone, or chat

4. **`Enterprise`**: Enterprise Support starts at **$15,000** a month and is recommended for **business or mission-critical** production workloads.


- Account and billing, 
- Service limit increases
- Technical support

Unlimited Contacts, Unlimited Cases, **Technical Account Manager (TAM)**, **Concierge** Support Team, **Infrastructure Event** Management, Full Set of Trusted Advisor Checks

Customer Service: Business-hours access via email only

#### Support Case Types

There are 3 types of support cases you can open with AWS Support.

1. **Account and billing**: Account-related and billing cases can be opened by all customers
2. **Service limit increases**: Default service quota (or limit) increases can be opened by all customers.
3. **Technical support**: Technical support cases can only be opened by customers on the Developer, Business, or Enterprise plans. 


> _Note_: AWS Support does **not** allow cases for _code development_, _debugging custom software_, or _performing system administration tasks_.


> _Note:_ Things to Remember


_Basic Support_: Don't forget how to open tickets and the types of tickets you're allowed to open

_Developer Support_: Don't forget how to open tickets and the types of tickets you're allowed to open

_Business Support_: Don't forget how to open tickets and the types of tickets you're allowed to open. Remember this support plan includes the full set of Trusted Advisor checks.

_Enterprise Support_: Don't forget how to open tickets and the types of tickets you're allowed to open.Remember this support plan includes the full set of Trusted Advisor checks.

Don't forget this support plan provides access to a **Technical Account Manager (TAM)** and the Concierge **Support Team**.


##### Questions

_Which AWS Trusted Advisor real-time guidance recommendations are available for AWS Basic Support and AWS Developer Support customers?_

- Security Groups - Specific Ports Unrestricted
- Amazon S3 bucket permissions
- Service limit checks

_Who can assist with accelerating the migration of legacy contact center infrastructure to AWS?_

- AWS Professional Services
- AWS Partner Network consulting partners

_Which service allows you to select and deploy operating system and software patches automatically across large groups of Amazon EC2 instances?_

AWS Systems Manager

_Which of the following usage types will always be free even after the 12-month Free Tier plan has expired?_

1 million AWS Lambda requests per month

_Which cost management tool gives you the ability to be alerted when the actual or forecasted cost and usage exceeds your desired threshold?_

AWS Budgets

_Which service provides the easiest way to set up and govern a secure, multi-account AWS environment?_

Control Tower

_Which API allows you to receive price alerts when prices change?_

Price List API

_Which tool allows you to compare your estimated service costs per Region?_

AWS Pricing Calculator

_Which service best reduces the operational overhead for your existing AWS cloud specialists?_

AWS Managed Services

_Which service alerts you to events that might impact your AWS environment?_

Personal Health Dashboard

_Which service helps you manage on-premises and AWS licenses?_

License Manager

_Which feature allows you to track AWS costs by labeling resources using a key and value pair?_

Cost allocation tags

_Which cost management tool allows you to see the most detailed information about your AWS bill?_

AWS Cost and Usage Reports

_Which types of issues are covered by AWS Support?_

- "How to" questions about AWS services and features
- Problems detected by health checks

_What is the easiest way for a customer on the AWS Basic Support plan to increase service limits?_

Open a service limit increase support case via email.

_Q: Which cost management tool allows you to view costs from the past 12 months, current detailed costs, and forecasts costs for up to 3 months?_

AWS Cost Explorer

_Q: Which service provides public and private certificates for free?_

Certificate Manager

_Q: Which features of AWS reduce your total cost of ownership (TCO)?_

- Elastic computing
- Pay-as-you-go pricing model
- Multi-tenancy


