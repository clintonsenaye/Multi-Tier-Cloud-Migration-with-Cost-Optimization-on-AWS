<h1>Multi-Tier Cloud Migration with Cost Optimization on AWS</h1>


<h2>Description</h2>
This project outlines a cost-effective strategy for migrating a multi-tier application (presentation, application, database) from an on-premises data center to the AWS cloud. 

<br />Key aspects include:

  - Utilizing appropriate AWS services like EC2, RDS, S3, CloudWatch, and Route 53 for each application tier.
  - Implementing cost-saving measures like Auto Scaling, optimized storage tiers, and data transfer acceleration.
  - Leveraging CloudFront, a Content Delivery Network, to improve user experience and potentially reduce costs associated with serving static content.
  - Following AWS Well-Architected best practices for security, monitoring, and disaster recovery.

This approach ensures a smooth and cost-optimized migration to the AWS cloud, providing scalability, reliability, and improved performance for your application.
<br />



<h2>Architectural Diagram: </h2>

<img width="1062" alt="Screenshot 2024-04-27 at 10 08 02 PM" src="https://github.com/clintonsenaye/Multi-Tier-Cloud-Migration-with-Cost-Optimization-on-AWS/assets/57267374/68761ee4-c710-4eef-86e7-92d78934fdec">

<h3>Planning and Assessment:</h3>

- Tier Identification: Start by identifying the different tiers in your application (presentation, application logic, database). This will help determine the most suitable AWS services for each tier.
- Workload Assessment: Analyze your workloads (CPU, memory, storage) to understand resource requirements and potential for scaling.
- Cost Estimation: Use the AWS Pricing Calculator https://calculator.aws/ to estimate potential costs for different service configurations.

<h3>Migration Strategy:</h3>

- Phased Approach: I Considered a phased migration technique to minimize downtime and risk; migrating one tier at a time, starting with the least critical tier.
- Migration Tools: Tools like AWS Server Migration Service (SMS) or AWS Database Migration Service (DMS) for automated and efficient migration of VMs and databases can be used.

<h3>Services:</h3>

- EC2 (Elastic Compute Cloud): Provides on-demand compute instances to host migrated application components.
- Amazon RDS (Relational Database Service): Managed database service for hosting migrated relational databases.
- Amazon S3 (Simple Storage Service): Object storage service for storing application data, logs, and backups.
- Amazon CloudFront (Content Delivery Network): Delivers static content (images, videos, etc.) with high performance and low latency.
- Amazon Route 53:  DNS service directs traffic to the Application Load Balancer.
- Reserved Instances (RI): Provides discounted pricing for EC2 instances used for predictable workloads.
- Auto Scaling: Automatically scales EC2 instances up or down based on predefined conditions.
- Spot Instances: Provides cost-effective compute capacity for workloads with flexible start and stop times.
- Application Load Balancer: automatically distributes incoming traffic across multiple targets.
- Amazon VPC: Virtual Private Cloud (VPC) for a secure and isolated network environment for your application.
- AWS CloudTrail: CloudTrail for logging all API calls made to AWS account, aiding in cost monitoring and security analysis.

<h3>Following Best Practices:</h3>

- Security: security best practices like IAM roles for least privilege access control and Amazon Security Groups for network access control.
- Monitoring and Logging: Amazon CloudWatch for monitoring application performance, resource utilization, and cost metrics.

<h3>Data Flow:</h3>



<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
