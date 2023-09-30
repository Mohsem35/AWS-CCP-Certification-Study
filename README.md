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