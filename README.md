1.How many resources do we have in IAM ?
ans;-Users:- Individual users.
Groups:- number of user.
Roles:- comunicate two services
Policies:-  define permission
MFA (Multi-Factor Authentication) Devices
====================================================================================================
2.Deployment model in IAM ?
ans:-1.On-premises
2.Cloud
3.Hybrid IAM platform
=================================================================================================================
3.Identities in IAM ?
ans;-An IAM identity represents a human user or programmatic workload, and can be authenticated and then authorized to perform actions in AWS
===================================================================================================================
4.What is an IAM User ?
ans:-IAM user is a resource in IAM that has associated credentials and permissions. An IAM user can represent a person or an application that uses its credentials and use
aws services or resources
=========================================================================================================================
5.What is the IAM Group ?
ans;-the group is an identity that specifies a collection of IAM users and Groups make permissions easier to manage for large sets of users.
=========================================================================================================================
6.What is the IAM Policy ?
ans;-policies define permissions for an action regardless of the method that you use to perform the operation ex-aws cli ,s3,ec2 etc
================================================================================================================================
7.What is the IAM Role ?
ans;-A role is a set of permissions that grant access to actions and resources in AWS. These permissions are attached to the role, not to an IAM User or a group.
==========================================================================================================================================================
8.Where do we attach Identity Based Policy ?
ans;-Identity-based policies are attached to an IAM user, group, or role. 
=================================================================================================================================
9.Where do we attach Resource Based Policy ?
ans;- resource-based policies attach to Amazon S3 buckets, Amazon SQS queues, VPC endpoints, and AWS Key Management Service encryption keys.
===============================================================================================================================
10.If one user has created it by default, which permission has been assigned to that user ?
ans;-that user iam full access either administrator full access
=================================================================================================================================
11.What is dominator policy ?
ans;-

Example- if in one group 5 members (users) are present in those users 1 user has administrator access it’s called dominator policy.

=================================================================================================================================
12.What is ARN ? What are the fields in ARN ?
ans;-1.Amazon Resource Names is uniquely identify AWS resources. We require an ARN when you need to specify a resource 
     2.arn:partition:service:region:account-id:resource
========================================================================================     
13.what is tag ?
ans:- Tags are key-value pairs that you can attach to AWS resources. Tags are used to label and categorize resources.
========================================================================================
14.Difference between Block storage & Object Storage ?
==========================================================================
block storage

Block storage has a powerful performance with transactional data and database
The higher the distance among application and storage, the greater the latency.
Addressing needs limits scalability.
Block storage will take any file apart into individual data blocks. It stores the blocks like data's separated pieces.
-All data's pieces contain the distinct address. Hence it does not require being stored within any file structure.
High Performance
High speed, Low latency, Redundancy, etc.

=======================================================================================
object storage

Object storage performs great for high flow throughput and big content.
Using Object storage, data can be saved within multiple regions.
Object storage can scale boundlessly to petabytes.
Object storage will take data's each piece and makes it as any object. Data will be stored in the isolated storehouses. It is bundled with related metadata and
-a specific identifier.
Distributed access and scalability
Resource optimization, reduced cost, faster data improvement, infinite scalability, and data analytics.

============================================================================================================================================
Difference between static website & dynamic website ?
============================================================================================================================================
static website

In static web pages, Pages will remain same until someone changes it manually
Static Web Pages are simple in terms of complexity.
In static web pages, Information are change rarely.
In Static Web Pages, database is not used.
Static web pages are written in languages such as: HTML, JavaScript, CSS, etc.
Static web pages does not contain any application program .
---------------------------------------------------------------------------------------------------------------------------------------------
dynamic website

In dynamic web pages, Content of pages are different for different visitors
Dynamic web pages are complicated.
In dynamic web page, Information are change frequently
Dynamic web page takes more time for loading
In dynamic web pages, database is used.
Dynamic web pages are writhn in languages such as: CGI, AJAX, ASP, ASP.NET, etc.
Dynamic web pages contains application program for different services.
====================================.========================================================================================================
16.What are the naming rules ?
ans;-Bucket names must be between 3 (min) and 63 (max) characters long.
Bucket names can consist only of lowercase letters, numbers, dots (.), and hyphens (-).
Bucket names must begin and end with a letter or number.
Bucket names must not contain two adjacent periods.
Bucket names must not be formatted as an IP address (for example, 192.168.5.4).
Bucket names must not start with the prefix xn--.
============================================================================================================================================
17.What is the major resource of S3 Bucket ?
ans;-resource of s3 bucket is create bucket,object storage,access control,versioning,lifecycle rule,replication rule,storage class,kms,
static website hosting,sns,cloudtrail,transper accleration,etc
==========================================================================================================================================
18.Why do we need to host static websites instead of dynamic websites ?
ans;-Static websites typically have lower hosting costs as they don't require server-side processing.
Static websites are simpler to set up and maintain.
They load faster because there's no server-side processing, making them more responsive to user requests.
==========================================================================================================================================
19.What is versioning & Why do we need versioning ?
ans;- S3 Versioning feature to preserve, retrieve, and restore every version of every object stored in your buckets.
In software development, versioning allows development teams to keep track of changes they make to the project code. The changes may include new functions,
features or bug fixes.
==========================================================================================================================================
20.What are the objects and types of objects that we are uploading into the S3 Bucket ?
ans:-s3 object uploading images, backups, data, movies,any other objects and types of objects file,logs,databases,Archives
==========================================================================================================================================
21.Why is MFA Delete important in S3 Bucket object level ?
ans;-This adds an extra layer of protection to prevent accidental or unauthorized deletions. To block accidental or malicious deletion.
Prevents Accidental Deletions.
Enhances Security.
Secures Critical Data.
Prevents Malicious Actions.
============================================================================================================================================
22.What is S3 Multipart upload ?
ans;-Simple Storage Service (S3) that allows you to upload large objects in parts.
Instead of uploading the entire object in a single request, you can break it into smaller parts and upload them concurrently. 
This method is particularly useful for large files, as it provides benefits such as improved performance, fault tolerance, and the ability to resume uploads.

============================================================================================================================================
23.What are the storage classes in Amazon S3 ?
ans;-there are s3 storage classes-1. Standard 2.Intelligent-Tiering 3.Standard-IA (Infrequent Access) 4.One Zone-IA 5.Glacier 6.Glacier Deep Archive
===========================================================================================================================================
24.What is ACL ?
ans:-acl stands for Access Control List. An Access Control List is a list of permissions associated with an object or
a bucket that specifies which AWS accounts or groups are granted access and what actions are allowed or denied.
==========================================================================================================================================
25.Why do we need ACL ?
ans;-Access Control Lists (ACLs) are essential for controlling and managing access to resources, such as buckets and objects, 
in Amazon S3 and other cloud services
==========================================================================================================================================
26.What is a Life cycle policy ? Why do we need to use the life cycle rule ?
ans;-lifecycle policy storage cost optimization ,lifecycle rule is s3 object automatically class change in our set opration
==========================================================================================================================================
27.How can we make our bucket public ?
ans:-firstly s3 open go to bucket and open then permission go on bucket policy is public
=========================================================================================================================================
28.Aws pricing factor of the S3 Service.
ans;-aws pricing factor is estimate the cost of using the s3  service.
=========================================================================================================================================
29.How can we make our object public ?
ans;-yes., i can change my s3 bucket ojject is bublic --step= open the bucket and select the object and go to the action then make acl object public
=====================================================================================================================================
30.How can we configure the static website logs in s3 ?
ans;- s3-->Permissions-->Edit Bucket Policy-->Block all public access-->uncheck-->Save Changes
=======================================================================================================================================
31.what is cors ?
ans;-CORS stands for Cross-Origin Resource Sharing. It is a security feature implemented by web browsers that controls how web pages in
one domain can request and interact with resources hosted on another domain.
========================================================================================================================================================
32.What is S3 Inventory ?
ans;-
Amazon S3 Inventory is a feature provided by Amazon Simple Storage Service (S3), which is a scalable and secure object storage 
service offered by Amazon Web Services (AWS). S3 Inventory enables you to generate reports about your S3 objects and their metadata on
a regular basis. These reports can provide valuable insights into your object storage, helping you with tasks such as compliance, auditing, and data lifecycle management.
========================================================================================================================================
33.Why do we need ACL ?
ans;- access control list is using spacial permission {read ,write ,exicute} 
======================================================================================================================================
34.What is a Life cycle policy ? Why do we need to use the life cycle rule ?
ans;


2>Assume a lot of data is updated in an S3 bucket regularly, and if all the data is maintained by standard storage it will cost you
more(even if previous data is of no use after some time). So, to avoid extra expenses and to maintain data as per requirement only 
life cycle management is needed. 
====================================================================================================================================
35.How can we make our bucket public ?
ans;- a bucket object is using publically and access for data .
==================================================================================================================================
36.How can we give public access to our bucket ?
ans;-s3 service open and go to permission and block public access edit and save change
==================================================================================================================================
37.Aws pricing factor of the S3 Service.
ans;-Storage Class
Storage Amount GB orTB
Requests pay
Data Transfer
Transfer Acceleration
Data Retrieval 
Cross-Region Replication
Data Transfer Acceleration
=================================================================================================================================
How can we make our object public ?
ans;- because publically access for s3 object data
=================================================================================================================================
How can we configure the static website logs in s3 ?
ans;-
================================================================================================================================
What does it mean by Requester pays ?
ans;-Requester Pays, the person or entity making requests to the bucket is responsible for the associated costs.
===================================================================================================================================
What is the secondary word to Transfer acceleration ?Why do we need to use this transfer acceleration ?
ans;-1>Transfer Acceleration." Amazon S3 Transfer Acceleration is a feature provided by Amazon Simple Storage Service (Amazon S3) that
allows for faster uploading and downloading of objects to and from an S3 bucket. The accelerated transfers are achieved by using
Amazon CloudFront's globally distributed edge locations to route the data, optimizing the delivery path.
2>transfer accleration is use for uploading and downloading data spped of transfer and improve performance
=============================================================================================================================
What is a cloud trail ?
ans;-Cloudwatch is a monitoring tool that you can use to monitor your various AWS resources.
Like health check, network, Application, etc.
===============================================================================================================================
Why do we use trails, what is the exact purpose of enabling the trail in cloud production accounts ?
ans;-CloudTrail logs are valuable for troubleshooting issues that may arise in the production environment.
Trails in AWS CloudTrail are used to maintain a detailed record of activities within your AWS account.
Security teams can use CloudTrail logs to detect and investigate potential security threats or unauthorized actions in the production environment
================================================================================================================================
Explain how we can create a trail in aws cloud trail ?
ans;- open a cloudtrail service and create trail-->trail name-->storage location-->next-->Choose log events--all-->API activity-->all-->next
review and create.
=================================================================================================================================
How can we enable logging for S3 bucket using cloud trails ?
ans;-
=================================================================================================================================
How do you get the list of all created trailers in your production account ?
ans;-
=================================================================================================================================
Can we create a trail for a multi region, if yes then how can we configure it ?
ans;-
=================================================================================================================================
How can we disable the logging for certain events, services in cloud trail, If yes so explain how ?
ans;-
=================================================================================================================================
Real time use case of cloud trail ?
ans;-Security and Compliance Monitoring-Detecting Unauthorized Access.
Troubleshooting and Debugging-Investigating Incidents, Identifying Root Causes.
Auditing and Governance-User Activity Monitoring, Resource Change Tracking.
Automated Alerts and Notifications-Setting up Alarms, Automated Responses.
Forensic Analysis-Post-Incident Analysis.
Enhancing Security Monitoring.
=================================================================================================================================
What is cloud trail event history ?
ans;-AWS CloudTrail Event History is like a detailed diary for your AWS account. It keeps a record of every action or change that happens in your AWS environment, such as creating a new server or modifying security settings.
This information includes details like creating or deleting resources, logging in, or changing settings. This "diary" is the CloudTrail Event History.
================================================================================================================================
What is log file integrity validation in cloud trail ?
ans;-CloudTrail log file integrity validation is a feature that allows users to determine if a CloudTrail log file has been modified,
deleted, or remained unchanged since it was delivered to the specified Amazon S3 bucket.
====================================================================================================================================================================
What is SNS ?
Ans;-SNS stands for Simple Notification Service. SNS is a web service that makes it easy to
notifications from the cloud. You can set up SNS to receive email notification or message notification.
====================================================================================================================================
Why do we use SNS ?
ans;-SNS is typically used for applications that need realtime notifications,
===================================================================================================================================
What are the different delivery formats and transports in AWS SNS ?
ans;- delivery format is= HTTP, HTTPS, Email-JSON and SQS 
===================================================================================================================================
56.Difference between Amazon SNS & Amazon SQS.
ans;- sns
1.sns is simple notification service
2.sns user for notification to performance to that service
3.sns is use in service is s3,autocaling,cloudtrail etc
4.sns is endpoint is- mobile sms ,email,lamda,http etc
sqs---------------------------------------------------------------------------------------
1.
=======================================================================================================================================
57.What are the different delivery formats and transports in AWS SNS ?
ans;-  sns for deliveries formats HTTP, HTTPS, Email-JSON and SQS and transportesis
=====================================================================================================================================
58.On which services are configured with the AWS SNS ?
ans;-Amazon SQS (Simple Queue Service)
AWS Lambda
Amazon EC2 (Elastic Compute Cloud)
Amazon S3 (Simple Storage Service)
Amazon CloudWatch
=====================================================================================================================================
What is the difference between SNS FIFO & Standard while creating the SNS topic.
ans;-
====================================================================================================================================
What is 10DLC in AWS ?
ans;-Stands for 10-Digit Long Code
It is related to SMS (Short Message Service) messaging. Specifically, it is a type of long code that is used for sending Application-to-Person (A2P) messages.
========================================================================================================
what is ec2 ?
ans;-
EC2 stands for Elastic Compute Cloud. EC2 is an on-demand computing service on the AWS cloud platform. 
Under computing, it includes all the services a computing device can offer to you along with the flexibility
of a virtual environment. It also allows the user to configure their instances as per their requirements i.e.
allocate the RAM, ROM, and storage according to the need of the current task. Even the user can dismantle 
the virtual device once its task is completed and it is no more required. For providing, all these
scalable resources AWS charges some bill amount at the end of every month, the bill amount is entirely dependent on your usage.
EC2 allows you to rent virtual computers. The provision of servers on AWS Cloud is one of the easiest ways in EC2. 
EC2 has resizable capacity. EC2 offers security, reliability, high performance, and cost-effective infrastructure so as to meet the demanding business needs.
=================================================================================================================================================
Why do we need EC2 service in cloud computing ?
ans;-
Amazon Elastic Compute Cloud (Amazon EC2) provides on-demand, scalable computing capacity in the Amazon Web Services (AWS) Cloud.
Using Amazon EC2 reduces hardware costs so you can develop and deploy applications faster.
============================================================================================================================================
Features of Amazon EC2 ?
ans;-
Amazon EC2 provides the broadest and deepest instance choice to match your workload’s needs. General purpose, compute optimized, 
memory optimized, storage optimized, and accelerated computing instance types are available that provide the optimal compute, memory,
storage, and networking balance for your workloads. Processors from Intel, AMD, NVIDIA and AWS power these instance types and provide
additional performance and cost optimizations. Local storage and enhanced networking options available with instance types further help
optimize performance for workloads that are disk or network I/O bound. Many instance types also offer bare metal instances that
provide your applications with direct access to the processor and memory of the underlying server for running in non-virtualized 
environments or for applications where you want to use your own hypervisor. To find the right instance for your workload, 
visit the EC2 instance types page. You can also use the AWS Compute Optimizer to get recommendations on optimal AWS Compute resources 
for your workloads to reduce costs and improve performance.
=====================================================================================
What is Hypervisor ? and its types ?
ans;-
Hyper visor is a firmware or low level program that acts as a virtual machine manager. A system on which hypervisor
is running one or more virtual machines is known as host machine. Each virtual machine is called guest machine. One can classify
hypervisor into two categories :
1. Type 1 / native / Bare-Metal
2.Type 2 / Hosted
===========================================================================================
Where we use hypervisor ?
ans;-
A hypervisor is a software that you can use to run multiple virtual machines on a single physical machine. Every virtual machine
has its own operating system and applications. The hypervisor allocates the underlying physical computing resources such as 
CPU and memory to individual virtual machinesas required.
=======================================================================================
Steps to create an EC2 instance.
ans;= following steps
Sign in to the AWS Management Console
Choose a name for your instance
Choose an Amazon Machine Image (AMI)
Choose an Instance Type
Create a key pair
Configure Security Group
Add Storage
Review and Launch
==============================================================================================
EC2 Instance state ?
ans;= 1> 2/2 =helthey   2> 1/2 =software error    3> 0/1=hardware error 
=================================================================================================
How many types of EC2 Instance-State codes ?
ans;-
0: pending
16: running
32: shutting-down
48: terminated
64: stopping
80: stopped
==================================================================================
What is the meaning of server hibernating mode ?
ans;=
In computing, hibernation is a power-saving mode that saves the current state of a computer's system to the hard drive before
shutting down. It's also known as "suspend to disk" or "Safe Sleep" on Macintosh computers. 
Both shut down and hibernated systems may consume standby power unless they are unplugged. Hibernation is a means of avoiding
the burden of saving unsaved data before shutting down and restoring all running programs and re-opening documents and browser tabs.
======================================================================================
AWS Amazon EC2 Instance types ?
ans;-General Purpose Instances,Compute Optimized Instances ,Memory-Optimized Instances,Storage Optimized Instances,Accelerated Computing Instances.
============================================================================================
How many types of status checks happen in aws ?
ans;-Amazon EC2, there are two types of status checks, commonly known as "instance status checks" and "system status checks.
" These checks help ensure the health and proper functioning of your EC2 instances and the underlying infrastructure.
=====================================================================================
When we see the global view option in ec2 service ?
ans;-
====================================================================================
When we logged into the cloud account by default why do we always jump into the north virginia region, why it’s most popular ?
ans;- aws  there might be changes or updates to cloud services, so it's always a good idea to check the current information. However,
as of that time, the U.S. East (North Virginia) region of Amazon Web Services (AWS) was one of the most popular and heavily used regions
==========================================================================================================
What are EBS Volumes and its types ?
ans;-General Purpose SSD,Provisioned IOPS SSD,Throughput Optimized HDD ,Cold HDD ,Magnetic (standard
============================================================================================
Purpose of Using EBS volumes ?
ans;- 1.Data backup and disaster recovery: Customers can use EBS snapshots to capture production data for testing and other purposes
      2.Primary storage: For data that needs frequent updates, such as system drives and database applications
============================================================================================
How many types of purchasing options do we have in aws ec2 ?
ans;-On-Demand Instances ,Reserved Instances ,Savings Plans ,Spot Instances ,Dedicated Hosts ,Dedicated Instances,Capacity Reservations
===============================================================================================
Difference between AWS AMI Image & AWS Template ?
ans;- aws ami
1.ami are primarily used to create virtual machine (ec2 instance) by providing a pre -configured snpshot of the root file system including
the operating system application and configurations
2.primarily used for deploying ec2 instance
3.used for individual instance deploying and scaling
4.created and managed thought the ec2 service
---aws template-----------------------------------------------------------------------------
1.cloud formation templates are used for defining and provisioning aws infrastucture as code allowing younto manage and 
version-control your entire aws environment
2.used for provisioning and managing a complate set of aws resources
3.manages the complate lifecycle of aws resources supporteding creation update and deletion
4.created managed and executed thought the aws cloud formation  service
============================================================================================
What is NIC & it’s types ?
ans;- nic is a hardware component without which a computer cannot be connected over a network. It is a circuit board installed in 
a computer that provides a dedicated network connection to the computer. It is also called network interface controller
types of nic ;-Internal Network Cards,External Network Cards
===========================================================================================
What is elastic IP ? & WHY were we used ?
ans;-a static IPv4 address that's designed for dynamic cloud computing. It's a static public address associated with your AWS account. 
     These are ipv4 address which are used to connect the instance from internet, they are chargedif the instances are not attached to it
========================================================================================
What is the snapshot of why we use it ?
ans;-It can back up the data on the EBS Volume. Snapshots are incremental backups.
• If this is your first snapshot it may take some time to create. Snapshots are point in time
copies of volumes.
==============================================================================================
What is the lifecycle manager in snapshot ?
ans;-Lifecycle Manager provides a simple and automated way for you to manage your EBS snapshot backups
==================================================================================================
How does the Amazon lifecycle manager work ?
ans;-S3 Lifecycle Manager automates the management of objects in S3 buckets over time. 
You can define rules to transition objects between storage classes or expire them after a specified period, helping optimize storage costs. 
It simplifies data lifecycle management by automatically applying policies to objects based on your specified criteria.
Procedure;
Select the "Management" tab for the bucket, and then choose "Lifecycle"
Create rules specifying transitions, expiration actions, or both. 
Specify the actions to be taken, such as transitioning to a different storage class, moving to Glacier, or deleting objects.
Review your configuration, and save the lifecycle policy.
===================================================================================
Difference between Security Group & NACL ?
ans security group
1. It supports only allow rules, and by default, all the rules are denied. You cannot deny the rule for establishing a connection.
2.It is associated with an EC2 instance.
3.It is the first layer of defense.
-nacl----------------------------------------------
1.It supports both allow and deny rules, and by default, all the rules are denied. You need to add the rule which you can either allow or deny it.
2.It is associated with a subnet.
3.It is the second layer of defense.
======================================================================================
How many IP Addresses can we attach to the instances ?
ans;- Amazon Web Services (AWS), a Virtual Private Cloud (VPC) can have a maximum of 5 IP addresses per Elastic Network Interface (ENI) 
and a maximum of 8,000 IP addresses per VPC. This means that a VPC can have a maximum of 8,000 public IP addresses, if you are using
the IPv4 addressing protocol.
==========================================================================================
How many types of volume states do we have ?
ans;- creating ,avilable ,in use,deleting,deleted,error
==============================================================================
What is a key pair, and its types ?
Ans:Key-pairs are secure login information for your instances/virtual machines. To connect to the
instances we use key-pairs that contain a public-key and private-key.
=================================================================================
What is load balancer and its types ?
ans;-A load balancer is a device or service that distributes incoming network traffic across multiple servers or resources t
o ensure that no single server becomes overwhelmed with too much traffic. Load balancing is commonly used to enhance the availability,
reliability, and scalability of applications or websites by evenly distributing the incoming requests.
types of loadblancer;-1.Application Load Balancer 2.Network Load Balancer 3.Classic Load Balancer 
=============================================================================
Features of Load Balancers ?
ans;-Distributes traffic among multiple servers to avoid overload.
Checks server health regularly to ensure traffic goes to healthy servers.
Uses smart algorithms to evenly spread traffic across servers.
Manages encryption, reducing the workload on backend servers.
Associates with security groups to provide an additional layer of security.
Supports real-time communication applications like chat (ALB, NLB).
Handles traffic over the newer IPv6 protocol

===========================================================================================
What is ASG ? & Its types ?
ans;-Auto scaling allows you to automatically scale-up and scale-down the number of instances
depending on the CPU utilization or memory utilization.
types of auto scalling;-1. horizontal scaling 2.vertical scaling
==========================================================================================
What is a Health Check ?
ans;-Auto Scaling in AWS, a health check is like a regular checkup for your instances. It's a way for Auto Scaling to make sure each 
instance in your group is doing well and ready to handle traffic. 

The health check monitors things like if the instance is responding, reachable, and overall in good shape.
=====================================================================================================
What is the threshold ?
ans;-threshold is like a limit or a point at which Auto Scaling takes action. It's a set level or condition that, when reached, triggers 
a response from Auto Scaling.
Example;
 Imagine you set a CPU usage threshold at 70%. This means that if any of your instances' CPU usage goes beyond 70%, it's a 
signal for Auto Scaling to take action.
===============================================================================================
What is the group of LB ?
ans;- autoscaling load balancer
=====================================================================================================
Difference between Web server & Application server ?
ans;- web server
1.In web server,HTML and HTTP protocols are used.
2.Web server encompasses web container only.
3.Web server is useful or fitted for static content.	
4.Web Server examples are Apache HTTP Server , Nginx.
--appliction server--------------------------------------------------------------------------------------
1.While in this, GUI as well as HTTP and RPC/RMI protocols are used.
2.While application server encompasses Web container as well as EJB container.
3.Whereas application server is fitted for dynamic content.
4.Application Servers example are JBoss , Glassfish.
=================================================================================================================================
What is the target group ?
ans;- target group is a component of the Elastic Load Balancing (ELB) service. ELB distributes incoming application traffi
c across multiple targets, such as Amazon EC2 instances, in multiple Availability Zones.
===================================================================================================================================
What is the desired capacity in ASG ?
ans;-the asg is minimum desired capacity is 1 and maximumis is required .
=================================================================================================================================
How many types of the Scaling option ?
ans;- there are scaling option 1.Dynamic Scaling 2.Scheduled Scaling 3.Manual Scaling
===================================================================================================================================
Scaling plans ?
ans;-1.Target Tracking Scaling 2.Step Scaling
===================================================================================================================================
Types Auto scaling
ans;-1.Amazon EC2 Auto Scaling 2.Dynamic Scaling 3.Scheduled Scaling 4.Predictive Scaling
===================================================================================================================================
Difference between vertical scaling andInvolves adding or removing instances to handle the load.
ans;-    vertical scaling
1.vertical scaling is scaling up
2.Adjusts the resources of an individual server or virtual machine
3.Typically involves adding more CPU, memory, or storage to a single machine.
Example:	
 Increasing the RAM of a database server to handle larger datasets.	
---horizontal scaling-------------------------------------------------------------------------------------------------------------
1.horizontal scaling is scaling out
2.Involves adding or removing instances to handle the load.
3.Adjusts the number of instances in a distributed system.
4.Example:
 Adding more web server instances to a load balancer to handle increased web traffic.
==============================================================================================
Difference between AMI & Snapshot ?
ans;- ami
1.ami  is a pre-configured virtual machine image, which includes an operating system, application server, and applications. 
It serves as the template for creating instances (virtual servers) in Amazon EC2 
2.You can create custom AMIs based on your EC2 instances, share them with other AWS accounts, and use them to launch new instances with the same configuration.
3.ami use backup
--snapshot----------------------------------------------------------------------------------------------------------------------
1.Snapshot is a point-in-time copy of an Amazon EBS volume. EBS provides block-level storage volumes 
2.snapshot is backup for volume use
3.migrate data between regions, and restore volumes to a previous state. 
=========================================================================================================================
103.What is difference between EBS/EFS/S3
ans;-
1>.ebs
1.It is used to provide the block-level storage volumes for the use of EC2 instances.	
2.It is mainly used for data that should be quickly accessible and requires long term durability.
3.Pay for provisioned capacity based on chosen volume type (gp2, io1, st1, sc1
4.Block storage, suitable for operating systems and applications.	.
2>.efs---------------------------------------------------------------------------------------------------------------
1.It is simple to use.
2.It is used in modernize application development
3.Industries use this for enhancing content management systems
3.Pay for the storage capacity used
4.File storage, suitable for shared access by multiple instances
3>.s3 ---------------------------------------------------------------------------------------------------------------
1.s3 is a store service
2.Object storage with different storage classes, including Standard, Intelligent-Tiering, Glacier, etc.
3.Pay for the storage used, data transfer, and requests made, with various storage classes offering different pricing.
4.Object storage, suitable for static content, backups, data archiving, and scalable storage.
==========================================================================================================================================================================
103.What is VPC ?
ans;-VPC stands for Virtual Private Cloud, and it is a fundamental component of Amazon Web Services (AWS). A VPC allows you to create
a logically isolated section of the AWS Cloud where you can launch and run resources in a virtual network that you define. It provides 
a way to customize your network configuration, such as IP address ranges, subnets, route tables, and network gateways.
=====================================================================================================================================
104.What are the Subnets when working with VPC ?
ans;-Each VPC network consists of one or more IP address ranges called subnets. Subnets are regional resources, and have IP address
ranges associated 
===================================================================================================================================
105.What is NAT Device ?
ans NAT  device is a networking device that performs Network Address Translation. NAT is a technique used to modify network address information
in packet headers while in transit, typically in routers or firewalls. The primary purpose of a NAT device is to allow multiple devices within
a private network to share a single public IP address for connecting to the internet.
========================================================================================================================================
106.What is the difference between stateful & stateless filtering ?
ans;-
1.Filtering decision Based on information in packet headers
2.Memory and CPU intensive low
3.stateful security is low
4.performanace is fast 
---stateless filtering-------------------------------------------------------------------------------------------------------------------
1.Filtering decision Based on flows
2.Memory and CPU intensive high
3.stateful security is high
4.performanace is low
=======================================================================================================================================
107.What are the advantages of using default VPC ?
ans;-
1.Internet access
A default VPC includes internet access by default, along with an internet gateway and public subnets with corresponding route tables.
This is not available by default in non-default VPCs.
2.IPv4 CIDR block
All default VPCs are associated with an IPv4 CIDR block with a 172.31.0.0/16 address range. This gives you 65,536 possible IP addresses, 
minus some AWS reserved addresses.
3.Public IPv4 addresses
In a default VPC, servers within the public subnet are assigned a public IP address. This allows servers to reach the outside internet,
and the outside internet to reach the servers
=================================================================================================================================
108.What is the internet gateway in VPC ?
ans;- internet gateway is a horizontally scaled, redundant, and highly available VPC component that allows communication between your VPC and 
the internet
===================================================================================================================================
109.What is Network ACL in VPC ?
ans;-A network access control list (ACL) allows or denies specific inbound or outbound traffic at the subnet level.
=======================================================================================================================================
110.What is the Security Group in VPC ?
ans;-a Security Group is a virtual firewall that controls inbound and outbound traffic for instances (virtual machines) within a VPC. 
Security Groups act as a fundamental component of the network security model in AWS, allowing you to define rules that determine
what kind of traffic is allowed or denied to and from instances.
=================================================================================================================================
111.What is an Elastic IP Address in VPC, and why do we need to use, realtime example ?
ans;-VPC is a static IPv4 address designed for dynamic cloud computing. It is associated with your AWS account, allowing you to allocate
it to instances within a VPC. Elastic IP addresses are particularly useful when you need a consistent public IP address for your
instance
2>.elastic ip uses- 1.Static IP Address 2.Avoiding IP Address Changes 3.Disaster Recovery and Redundancy 4.Portability and Reusability
3>. realtime elastic ip example in ;- web server running on an EC2 instance in your VPC, and you want to host a website with a consistent public IP address
=======================================================================================================================================
112.Can we attach one Production Elastic IP to the new Prod server ?
ans;-yes
=========================================================================================================================================
113.How does ELB Affect a VPC ?
ans;-
=============================================================================================================================
114.What are the limitations of VPC’s, Gateway and subnets ?
ans;-limitations of VPC
The default limit for VPCs per region is 5.
The limit is made up of primary CIDR block plus 4 secondary CIDR blocks.
VPC endpoints and services must be in the same region.
VPC endpoints only support IPv4 traffic.
Endpoints can't be transferred from one VPC or service to another.
--gateway------------------------------------------------------------------------------------------------------------------------
The major disadvantage of using a gateway is its implementation cost.
The default gateway IP address doesn't change when the network topology changes.
--Subnets--------------------------------------------------------------------------------------------------------------------------
As the number of sub-networks increases, the complexity of the network also increases.
This makes maintaining and troubleshooting the errors in the network more difficult. 
===================================================================================================================================
115.What is a Public IP Address and why do we use it ?
ans;- 1>A public IP address is a unique numerical label assigned to devices connected to a computer network that uses the Internet
Protocol for communication. This address is globally unique and is routable over the internet.
2>Require remote access to their networks
Need to host websites or online services
Want to take advantage of cloud computing 
================================================================================================================================
116.Explain Bastion Host Concept ?
ans;-What is the concept of bastion host?
What is a Bastion Host?
A bastion host is a server used to manage access to an internal or private network from an external network - sometimes called bastin host
===================================================================================================================================
117.When do we need to create a new customised VPC ?
ans;-when there is a requirement to create your own network for your own purpose or your company
================================================================================================================================
118.When do we need to create a new customised VPC ?
ans;-when there is a requirement to create your own network for your own purpose or your company
===============================================================================================================================
119.What is Peering ? Why do we need to peer at two VPC’s ?
ans;- 1> VPC peering is a networking connection that allows traffic to be routed between two VPCs using private IP addresses
      2>
===============================================================================================================================
120.What is VPN, Where do we use VPN Tunnel ?
ans;-1> VPN or Virtual Private Network creates a private network connection between devices through the internet. VPNs are used to safely and 
anonymously transmit data over public networks. They work by masking user IP addresses and encrypting data so it's unreadable by
anyone not authorized to receive it.
2>A VPN tunnel is a secure, encrypted connection between a user's device and the internet through a virtual private network. 
The VPN tunnel encrypts the user's internet traffic and routes it to a remote VPN server. From there, the data is decrypted and
delivered to its intended destination
======================================================================================================================================
