AWS Cloud Practitioner Essentials Note:

### <u>Intro</u>

- **Intro**:
  - You only pay for what you use!
  - In computing, a **client** can be a web browser, desktop application, and a **server** can be AWS EC2 (Elastic Compute Cloud), a type of virtual computer

- **Cloud computing:**

  - Cloud-based development: Every thing on cloud! Your all parts, migrate existing parts, design and build new parts in the cloud

  - On-premises development:  Also known as private cloud development. Resources are deployed on premises by using virtualization and resource management tools

  - Hybrid development: Cloud-based resources are connected to your on-premises infra.

    *Benefits of cloud computing:*

    - Trade upfront expense for variable expense
    
    - Stop spending money to run and maintain data centers
    
    - Stop guessing capacity
    
    - Benefit from massive economies of scale
    
    - Increase speed and agility
    
    - Go global in minutes
    
### <u>Compute in the cloud</u>

- **Amazon EC2**

  - It provides secure, resizable compute capacity in the cloud as Amazon EC2 instances.
  - How EC2 works:
    - Launch: First, launch an instance with corresponding configuration: OS, application server,...
    - Connect: Next, connect to the instance.
    - Use: Finally, after you have connected to the instance, you can begin using EC2 by running commands, add storage, copy and organize files,...
  - Instance type:
    - General purposes: provide a balance of compute, memory and networking resources.
    - Compute optimized: ideal for compute-bound application that benefit from high-performance processors.
    - Memory optimized: ideal for fast performance of workloads that process large datasets in memory.
    - Accelerated computing: Use hardware accelerators, or coprocessors, to perform some functions more efficiently.
    - Storage optimized: ideal for workloads that require high, sequential read and write access to large datasets on local storage.
  - Pricing:
    - On-demand: ideal for short-term, irregular workloads that cannot be interrupted. No upfronts costs or minimum contracts apply. You pay for compute time you use.
    - Saving plans: Enable you to reduce you compute costs by committing to a consistent amount of compute usage for a 1-year or 3-year term. Usage up to the committed is charged at the saving plans, any usage beyond the committed is charged at the on-demand plan.
    - Reserved instances: billing discount apply to the on-demand instances. There have 3 types of reversed instances: Standard reversed, convertible reversed and scheduled reversed instances.
    - Spot instances: ideal for workloads with flexible start and end time or that can withstand interruptions.
    - Dedicated hosts: physical servers with EC2 instance capacity that is fully dedicated to your use.
  - Auto scaling:
    - automatically add/remove EC2 instances in response to changing application demand.
  
- **Elastic Load balancing:**
  
    - Automatically distributes incoming application traffic across mulitple resources, such as EC2 instances.
    
- **Amazon SNS (Simple notification Service):**
  
  - is a pub/sub model, using Amazon SNS topics, a publisher publishes messages to subscribers
  
- **Amazon SQS (Simple queue service):**
  
  - is a message queue service, using Amazon SQS, you can send, store, and receive messages between software components without losing messages or requiring other services to be available
  
- **AWS Lambda:**
  
  - is a service allow execute code without needing to manage servers
  - you only pay for the compute time you consume
  - you can also build an run containerized applications
  - Amazon ECS (Elastic Container Service):
    - is a highly scalable, high-performance container management system that enables you to run and scale containerized applications on AWS.
  - Amazon EKS (Elastic Kubernetes Service):
    - is a fully managed service that you can use to run Kubernetes on AWS.
  
  - Amazon Fargate:
    - is a serverless compute engine for containers. It works with both ECS and EKS.

### <u>Global infrastructure and reliability</u>
- **Selecting a region:**
  - Compliance with governance and requirements
  - How close to your customers
  - Available services within the region
  - Pricing

- **Availability zones:**
  - is a single data center or a group of data centers within a Region. A Region is a geographical area that contains AWS resources.

- **Edge locations:**
  - is a site the Amazon Cloudfront uses to store cached copies of your content closer to your customer for faster delivery

- **How to interact with AWS resources:**

  Every interaction to AWS resources will be via API calls.

  - AWS management console:
    - is a browser-based interface for accessing and managing AWS services.
  - AWS command line interface:
    - enables you to control multiple AWS services directly from te command line within one tool.
  - Software development kits (SDK):
    - SDK make it easier for you to use AWS services through an API designed for your programming language or platform. It enables you to use AWS services with your existing applications or create entirely new applications that will run on AWS.

- **AWS Elastic Beanstalk:**
  - you provide code and configuration settings, and EB deploys the resources nesessary to perform the following tasks:
    - Adjust capacity
    - Load balancing
    - Automatic scaling
    - Application health monitoring

- **AWS CloudFormation:**
  - you can treat your infrastructure as code. This meas that you can build an enviroent by writing linies of code instead of using the AWS Management Console to individually provision resources.