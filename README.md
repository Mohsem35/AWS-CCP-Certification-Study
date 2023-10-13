Demonstrate: EC2, Lambda. S3,   

## AWS-Learning for AWS Certified Cloud Practitioner Exam

4 exam domains

- **`Cloud Concepts`** (24% of scored content)
- **`Security and Compliance`** (30% of scored content)
- **`Cloud Technology and Services`** (34% of scored content)
- **`Billing, Pricing, and Support`** (12% of scored content)

#### chapter 1
### Foundations of Cloud Computing (24%)

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
### Technology (33%)

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




**_Elastic Load Balancing_** automatically distributes your **`incoming application traffic`** across multiple EC2 instances

<img width="387" alt="Screenshot 2023-10-10 at 5 42 21 PM" src="https://github.com/Mohsem35/AWS-Learning/assets/58659448/a3e03089-161c-4eea-83e6-5672b2220308">

Four types of load balancers are available
1. Classis
2. Application
3. Gateway
4. Network


![download](https://github.com/Mohsem35/AWS-Learning/assets/58659448/72d61e38-f1f2-4ce7-92fa-89a1ecd38bf7)


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

#### EC2 Storage
All EC2 instances must have a root drive. this could be an **`EBS`** volume or an **`instance store drives(physical machine)`**

You can also _attach multiple EBS volumes to a single EC2 instance_. You can think of these as **`hard drives`** that you've installed on the EC2 instance. The important **`distinction`** between EBS drives and instance store drives is that EBS drives are **`persistent`**. You can stop or terminate the instance, or even detach an EBS drive and attach it to a different EC2 instance. They have lower latency, but that data does not persist if an EC2 instance is stopped or terminated.


#### Amazon Elastic File System (EFS)

like dropbox or google drive


So if you have a Site-to-Site VPN or a direct connection to the AWS Cloud, you can use Storage Gateway to hybridize your data storage. You can think of this sort of as a file directory, where some of the files are hosted locally, and some of them are hosted in the cloud.