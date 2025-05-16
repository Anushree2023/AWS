# AWS
## ✅ 1. **Compute Services**

---

### 🔹 Amazon EC2 (Elastic Compute Cloud)

- 📖 **Definition**: Virtual servers in the cloud.
- ⚙️ **Usage**: Host websites, applications, backend services.
- ✅ Flexible instance types, scalable, supports auto-scaling and load balancing.
- ⚠️ Requires management of OS, patching, and scaling if not automated.
- 🎯 Use Cases: Web hosting, application servers, batch processing.
- 📝 **Note**: Pay for what you use (On-Demand, Reserved, Spot Instances).

---

### 🔹 AWS Lambda

- 📖 **Definition**: Serverless compute service to run code in response to events.
- ⚙️ **Usage**: Event-driven tasks, microservices, automation.
- ✅ No server management, auto-scaling, pay-per-use.
- ⚠️ Cold start latency, limited runtime (15 mins).
- 🎯 Use Cases: Image resizing, API backend, IoT data processing.
- 📝 **Note**: Part of serverless stack with API Gateway and DynamoDB.

---

### 🔹 AWS Elastic Beanstalk

- 📖 **Definition**: Platform-as-a-Service to deploy web apps.
- ⚙️ **Usage**: Deploy web apps with minimal infrastructure management.
- ✅ Simplifies deployment, auto-scaling, supports many languages.
- ⚠️ Less control over infrastructure.
- 🎯 Use Cases: Fast app deployment for developers.
- 📝 **Note**: Handles EC2, ELB, Auto Scaling, etc. under the hood.

---

### 🔹 AWS Lambda@Edge

- 📖 **Definition**: Run Lambda functions at AWS Edge Locations.
- ⚙️ **Usage**: Customize CDN content delivery.
- ✅ Low latency, global delivery.
- ⚠️ Debugging can be harder.
- 🎯 Use Cases: Content personalization at CDN level.
- 📝 **Note**: Works with Amazon CloudFront.

---

## ✅ 2. **Storage Services**

---

### 🔹 Amazon S3 (Simple Storage Service)

- 📖 **Definition**: Object storage service with high durability.
- ⚙️ **Usage**: Store static files, backups, big data.
- ✅ Scalable, secure, durable (11 9s), multiple storage classes.
- ⚠️ Charges for requests, storage, and data transfer.
- 🎯 Use Cases: Media storage, website hosting, backup.
- 📝 **Note**: Versioning, lifecycle policies, and access control.

---

### 🔹 Amazon EBS (Elastic Block Store)

- 📖 **Definition**: Block storage for EC2 instances.
- ⚙️ **Usage**: Persistent storage for EC2.
- ✅ High performance, encrypted.
- ⚠️ Tied to a specific Availability Zone.
- 🎯 Use Cases: Databases, file systems.
- 📝 **Note**: Can take snapshots to S3.

---

### 🔹 Amazon EFS (Elastic File System)

- 📖 **Definition**: Managed network file system.
- ⚙️ **Usage**: Shared file access between EC2.
- ✅ Scales automatically, POSIX-compliant.
- ⚠️ Can be costly for large data.
- 🎯 Use Cases: CMS, shared access environments.
- 📝 **Note**: Works across multiple EC2 instances.

---

### 🔹 Amazon Glacier / S3 Glacier

- 📖 **Definition**: Low-cost archival storage.
- ⚙️ **Usage**: Backup, long-term storage.
- ✅ Very cheap, secure.
- ⚠️ Retrieval time can be hours.
- 🎯 Use Cases: Regulatory archive, cold data.
- 📝 **Note**: Use lifecycle policies to transition from S3 to Glacier.

---

## ✅ 3. **Database Services**

---

### 🔹 Amazon RDS (Relational Database Service)

- 📖 **Definition**: Managed relational database (SQL).
- ⚙️ **Usage**: Host MySQL, PostgreSQL, Oracle, SQL Server, MariaDB, Aurora.
- ✅ Automated backups, patching, scaling.
- ⚠️ Less control over DB server.
- 🎯 Use Cases: Web apps, e-commerce.
- 📝 **Note**: Use Multi-AZ for high availability.

---

### 🔹 Amazon DynamoDB

- 📖 **Definition**: Managed NoSQL database.
- ⚙️ **Usage**: Key-value and document storage.
- ✅ Fast, scalable, serverless.
- ⚠️ Complex queries not supported like SQL.
- 🎯 Use Cases: Gaming, IoT, session storage.
- 📝 **Note**: Integrates with Lambda and API Gateway.

---

### 🔹 Amazon Redshift

- 📖 **Definition**: Data warehouse for analytics.
- ⚙️ **Usage**: Run complex queries on big data.
- ✅ High performance, integrates with BI tools.
- ⚠️ Higher cost, not real-time.
- 🎯 Use Cases: Reporting, dashboards.
- 📝 **Note**: Columnar storage for speed.

---

## ✅ 4. **Networking & Content Delivery**

---

### 🔹 Amazon VPC (Virtual Private Cloud)

- 📖 **Definition**: Isolated virtual network in AWS.
- ⚙️ **Usage**: Launch AWS resources in private network.
- ✅ Full control over network config.
- ⚠️ Requires network knowledge.
- 🎯 Use Cases: Secure app hosting, private subnets.
- 📝 **Note**: Includes subnets, route tables, gateways.

---

### 🔹 AWS CloudFront

- 📖 **Definition**: CDN to deliver content globally.
- ⚙️ **Usage**: Cache and deliver static & dynamic content.
- ✅ Low latency, integrates with S3, Lambda@Edge.
- ⚠️ Cache invalidation can cost.
- 🎯 Use Cases: Media streaming, website acceleration.
- 📝 **Note**: Distributes content from Edge Locations.

---

### 🔹 AWS Route 53

- 📖 **Definition**: DNS service for domain registration and routing.
- ⚙️ **Usage**: Manage domain names, health checks.
- ✅ Scalable, integrates with other AWS services.
- ⚠️ Charges for hosted zones and queries.
- 🎯 Use Cases: Domain management, failover routing.
- 📝 **Note**: Supports routing policies like latency, geolocation.

---

## ✅ 5. **Security, Identity & Compliance**

---

### 🔹 AWS IAM (Identity and Access Management)

- 📖 **Definition**: Manage users and permissions.
- ⚙️ **Usage**: Grant access to AWS resources.
- ✅ Granular access, roles, policies.
- ⚠️ Misconfigured policies can cause vulnerabilities.
- 🎯 Use Cases: Access control, federated login.
- 📝 **Note**: Always follow least-privilege principle.

---

### 🔹 AWS KMS (Key Management Service)

- 📖 **Definition**: Create and manage encryption keys.
- ⚙️ **Usage**: Encrypt data across AWS.
- ✅ Integrated with many AWS services.
- ⚠️ Key misuse can lock out data.
- 🎯 Use Cases: Secure S3, EBS, RDS data.
- 📝 **Note**: Supports automatic key rotation.

---

### 🔹 AWS Shield

- 📖 **Definition**: DDoS protection service.
- ⚙️ **Usage**: Protect applications from network attacks.
- ✅ Always-on detection, free basic tier.
- ⚠️ Advanced version is paid.
- 🎯 Use Cases: Protect public-facing apps.
- 📝 **Note**: AWS Shield Advanced includes 24/7 support.

---

## ✅ 6. **Management & Monitoring**

---

### 🔹 AWS CloudWatch

- 📖 **Definition**: Monitoring and observability service.
- ⚙️ **Usage**: Collect metrics, logs, alarms.
- ✅ Real-time insights.
- ⚠️ Logging large volumes can cost.
- 🎯 Use Cases: System health monitoring, alerting.
- 📝 **Note**: Supports custom metrics.

---

### 🔹 AWS CloudTrail

- 📖 **Definition**: Logging and monitoring of API calls.
- ⚙️ **Usage**: Audit changes and actions.
- ✅ Records all account activity.
- ⚠️ Retention costs over time.
- 🎯 Use Cases: Security auditing, compliance.
- 📝 **Note**: Integrates with S3 for log storage.

---

### 🔹 AWS Trusted Advisor

- 📖 **Definition**: Recommends best practices across AWS.
- ⚙️ **Usage**: Cost optimization, security, fault tolerance.
- ✅ Easy insights, especially with Business/Enterprise support.
- ⚠️ Limited features in free tier.
- 🎯 Use Cases: Cost savings, security posture.
- 📝 **Note**: Use regularly to optimize.

---

## ✅ 7. **Pricing & Support**

---

### 🔹 AWS Pricing Models

- On-Demand
- Reserved Instances
- Spot Instances
- Savings Plans
- Free Tier

---

### 🔹 AWS Support Plans

- Basic (free)
- Developer
- Business
- Enterprise

---

### 🔹 AWS Billing Tools

- **Cost Explorer**: Analyze spending patterns.
- **Budgets**: Set cost limits and receive alerts.
- **TCO Calculator**: Compare AWS vs. on-premises.
- **Simple Monthly Calculator**: Estimate AWS costs.

---

## ✅ 8. **Other Important Services in Practitioner**

---

### 🔹 AWS Organizations

- Manage multiple AWS accounts.
- Centralized billing and policy control.

---

### 🔹 AWS Artifact

- Access compliance reports (e.g., ISO, PCI).

---

### 🔹 AWS Well-Architected Tool

- Assess workloads using AWS best practices.

---

### 🔹 AWS Marketplace

- Buy and sell software on AWS.

---

## 🧠 AWS Cloud Practitioner Services Guide (Detailed Notion Doc Format)

---

### ✅ 1. Compute Services

### 🔹 Amazon EC2 (Elastic Compute Cloud)

- **Definition**: Virtual servers in the cloud.
- **Usage**: Host websites, applications, backend services.
- **Advantages**:
    - Flexible instance types
    - Auto-scaling
    - Load balancing
- **Disadvantages**:
    - You manage OS, patching, scaling unless automated.
- **Use Cases**:
    - Web hosting
    - Application backend
    - Batch processing
- **Key Notes**: On-Demand, Reserved, Spot pricing options.

### 🔹 AWS Lambda

- **Definition**: Serverless compute service to run code in response to events.
- **Usage**: Event-driven tasks, microservices, automation.
- **Advantages**:
    - No server management
    - Scales automatically
    - Pay-per-invocation
- **Disadvantages**:
    - Cold starts
    - Max 15-minute runtime
- **Use Cases**:
    - Image processing
    - Backend logic for APIs
    - IoT data handlers
- **Key Notes**: Works well with API Gateway, DynamoDB.

### 🔹 AWS Elastic Beanstalk

- **Definition**: Platform-as-a-Service for app deployment.
- **Usage**: Deploy web applications without managing infrastructure.
- **Advantages**:
    - Auto-provisioning
    - Easy deployment
- **Disadvantages**:
    - Less infrastructure control
- **Use Cases**:
    - Rapid deployment
- **Key Notes**: Abstracts EC2, ELB, Auto Scaling.

### 🔹 Lambda@Edge

- **Definition**: Run Lambda at AWS Edge locations.
- **Usage**: Customize content delivery with CloudFront.
- **Advantages**:
    - Low latency
- **Disadvantages**:
    - Debugging complexity
- **Use Cases**:
    - Personalized content delivery
- **Key Notes**: Integrated with CloudFront.

---

### ✅ 2. Storage Services

### 🔹 Amazon S3

- **Definition**: Object storage with 11 9s durability.
- **Usage**: Store static files, backups, media.
- **Advantages**:
    - Scalable
    - Secure
    - Lifecycle management
- **Disadvantages**:
    - Cost for requests, retrievals
- **Use Cases**:
    - Static website hosting
    - App assets
- **Key Notes**: Versioning, encryption supported.

### 🔹 Amazon EBS

- **Definition**: Block storage for EC2 instances.
- **Usage**: Persistent storage volume attached to EC2.
- **Advantages**:
    - High performance
- **Disadvantages**:
    - Zonal constraints
- **Use Cases**:
    - Databases
    - File systems
- **Key Notes**: Snapshots to S3 for backup.

### 🔹 Amazon EFS

- **Definition**: Scalable file storage.
- **Usage**: Shared file system for EC2.
- **Advantages**:
    - Elastic capacity
    - POSIX compliant
- **Disadvantages**:
    - Higher cost for large data
- **Use Cases**:
    - CMS
    - Analytics platforms

### 🔹 Amazon S3 Glacier

- **Definition**: Archival storage for long-term backups.
- **Usage**: Cold data storage.
- **Advantages**:
    - Very low cost
- **Disadvantages**:
    - Retrieval delays
- **Use Cases**:
    - Compliance data
    - Archives

---

### ✅ 3. Database Services

### 🔹 Amazon RDS

- **Definition**: Managed relational database.
- **Usage**: SQL databases.
- **Advantages**:
    - Automated backups
    - Multi-AZ availability
- **Disadvantages**:
    - Limited control over underlying OS
- **Use Cases**:
    - Web and enterprise apps

### 🔹 Amazon DynamoDB

- **Definition**: NoSQL database.
- **Usage**: Key-value/document storage.
- **Advantages**:
    - Fast
    - Serverless
- **Disadvantages**:
    - Limited querying
- **Use Cases**:
    - Gaming
    - Real-time apps

### 🔹 Amazon Redshift

- **Definition**: Managed data warehouse.
- **Usage**: Analytics, reporting.
- **Advantages**:
    - High performance queries
- **Disadvantages**:
    - Expensive for small data
- **Use Cases**:
    - Business intelligence

---

### ✅ 4. Networking & Content Delivery

### 🔹 Amazon VPC

- **Definition**: Private virtual network.
- **Usage**: Isolate and secure AWS resources.
- **Advantages**:
    - Full network control
- **Disadvantages**:
    - Needs networking knowledge
- **Use Cases**:
    - Secure cloud apps

### 🔹 Amazon CloudFront

- **Definition**: Content Delivery Network.
- **Usage**: Deliver static/dynamic content globally.
- **Advantages**:
    - Low latency
- **Disadvantages**:
    - Cache invalidation costs
- **Use Cases**:
    - Media delivery
    - Websites

### 🔹 AWS Route 53

- **Definition**: DNS and domain routing.
- **Usage**: Manage domains and routing policies.
- **Advantages**:
    - Scalable and global
- **Disadvantages**:
    - Pay per zone/query
- **Use Cases**:
    - Domain hosting
    - Load balancing

---

### ✅ 5. Security, Identity & Compliance

### 🔹 AWS IAM

- **Definition**: Identity and access control.
- **Usage**: Control who can do what on AWS.
- **Advantages**:
    - Granular permissions
- **Disadvantages**:
    - Misconfiguration risks
- **Use Cases**:
    - Secure multi-user access

### 🔹 AWS KMS

- **Definition**: Key management and encryption.
- **Usage**: Encrypt data and manage keys.
- **Advantages**:
    - Integrated with AWS services
- **Disadvantages**:
    - Key misuse risks

### 🔹 AWS Shield

- **Definition**: DDoS protection.
- **Usage**: Protect web apps from attacks.
- **Advantages**:
    - Basic tier free
- **Disadvantages**:
    - Advanced tier is paid

---

### ✅ 6. Management & Monitoring

### 🔹 AWS CloudWatch

- **Definition**: Monitoring service.
- **Usage**: Collect logs and metrics.
- **Advantages**:
    - Real-time monitoring
- **Disadvantages**:
    - Log storage can be costly

### 🔹 AWS CloudTrail

- **Definition**: Log API activity.
- **Usage**: Security and auditing.
- **Advantages**:
    - Full traceability

### 🔹 AWS Trusted Advisor

- **Definition**: Best practice checker.
- **Usage**: Analyze cost, security, and performance.
- **Advantages**:
    - Actionable insights

---

### ✅ 7. Pricing, Billing & Support

- **Pricing Models**:
    - On-Demand
    - Reserved Instances
    - Spot Instances
    - Savings Plans
    - Free Tier
- **Support Plans**:
    - Basic (Free)
    - Developer
    - Business
    - Enterprise
- **Billing Tools**:
    - AWS Budgets
    - Cost Explorer
    - TCO Calculator
    - Simple Monthly Calculator

---

### ✅ 8. Other Essential Services

### 🔍 Additional Services Explained

### 🔹 AWS Organizations

- **Definition**: A service that enables centralized governance and management across multiple AWS accounts.
- **Usage**: Group accounts into organizational units (OUs), apply Service Control Policies (SCPs), and consolidate billing.
- **Benefits**:
    - Central policy control
    - Centralized billing
    - Improved security and compliance
- **Use Cases**:
    - Enterprises managing multiple departments
    - Centralized security for multiple dev/test/prod environments

### 🔹 AWS Artifact

- **Definition**: On-demand access to AWS's compliance documentation.
- **Usage**: Download compliance reports such as ISO, SOC, PCI.
- **Benefits**:
    - Easy access to security and compliance documents
    - Helps organizations meet regulatory requirements
- **Use Cases**:
    - Audits
    - Security assessments
    - Due diligence

### 🔹 AWS Marketplace

- **Definition**: A digital catalog of software solutions and services offered by third-party vendors.
- **Usage**: Discover, purchase, and deploy software (AMIs, SaaS, ML models, etc.) quickly.
- **Benefits**:
    - One-click deploy to AWS
    - Integrated billing
- **Use Cases**:
    - Buying firewall appliances, ML tools, CMS platforms, and data products

### 🔹 AWS Well-Architected Tool

- **Definition**: Helps review and improve workloads based on AWS best practices.
- **Usage**: Evaluate architecture against 6 pillars (operational excellence, security, reliability, performance efficiency, cost optimization, and sustainability).
- **Benefits**:
    - Provides detailed insights and recommendations
    - Helps in building robust and optimized applications
- **Use Cases**:
    - Reviewing app performance
    - Ensuring compliance with AWS design principles

---

---

### 🔒 Security Tools in AWS

---

### 🔹 **AWS Identity and Access Management (IAM)**

- **Definition**: Manage access to AWS services and resources securely.
- **Key Features**:
    - Users, groups, roles, and policies
    - Multi-Factor Authentication (MFA)
    - Least privilege access
- **Use Cases**:
    - Granting users or apps controlled access
    - Federated access via corporate identity systems

---

### 🔹 **AWS Key Management Service (KMS)**

- **Definition**: Create and manage cryptographic keys.
- **Key Features**:
    - Customer Managed Keys (CMKs)
    - Automatic key rotation
    - Integrated with over 70 AWS services
- **Use Cases**:
    - Encrypting S3 data, EBS volumes, RDS
    - Digital signing and custom encryption workflows

---

### 🔹 **AWS Shield**

- **Definition**: DDoS protection service.
- **Versions**:
    - **Shield Standard**: Free, always-on protection
    - **Shield Advanced**: Extra protections, cost protection, and 24/7 access to AWS DDoS Response Team (DRT)
- **Use Cases**:
    - Protecting websites and APIs from external attacks

---

### 🔹 **AWS WAF (Web Application Firewall)**

- **Definition**: Protect web applications from common threats like SQL injection, XSS.
- **Key Features**:
    - Custom rules, managed rule groups
    - Integrates with CloudFront, ALB, API Gateway
- **Use Cases**:
    - Blocking bad bots
    - Securing web applications and APIs

---

### 🔹 **Amazon GuardDuty**

- **Definition**: Intelligent threat detection service using ML and threat intelligence.
- **Key Features**:
    - Continuously monitors AWS accounts, VPC flow logs, DNS logs, and CloudTrail
    - Detects anomalies and suspicious behavior
- **Use Cases**:
    - Intrusion detection
    - Alerting on unauthorized access or crypto-mining

---

### 🔹 **AWS Inspector**

- **Definition**: Automated vulnerability management for EC2 and container workloads.
- **Key Features**:
    - Scans EC2 instances and container images for vulnerabilities
    - Integrates with AWS Security Hub
- **Use Cases**:
    - Ensuring patch compliance
    - Reducing security exposure

---

### 🔹 **AWS Security Hub**

- **Definition**: Central security dashboard aggregating findings from multiple AWS services.
- **Key Features**:
    - Integrates with GuardDuty, Inspector, IAM Access Analyzer, and third-party tools
    - Provides security score and compliance standards (e.g., CIS AWS Foundations)
- **Use Cases**:
    - Centralized security management
    - Continuous compliance monitoring

---

### 🔹 **IAM Access Analyzer**

- **Definition**: Identifies unintended access to resources.
- **Key Features**:
    - Detects publicly or cross-account shared resources
    - Offers policy suggestions
- **Use Cases**:
    - Auditing permissions
    - Preventing accidental exposure of S3, IAM roles, etc.

---

Let me know if you’d like this added directly to your document, or if you'd like a visual **mind map or table format** summarizing all AWS Security tools!

---

### **Migration Strategy**

Use the **6 R’s** (AWS strategy):

| Strategy | Description |
| --- | --- |
| **Rehost** (lift & shift) | Move apps as-is to cloud (quickest) |
| **Refactor** | Modify code to fit cloud (for long-term gains) |
| **Replatform** | Small optimizations without full rewrite |
| **Repurchase** | Move to a new SaaS solution |
| **Retire** | Remove outdated apps |
| **Retain** | Keep certain apps on-prem if needed |

Here’s a detailed section on **Scaling Strategies in AWS**, formatted to fit seamlessly into your study doc:

---

### 📈 Scaling Strategies in AWS (Auto Scaling)

AWS provides multiple ways to scale resources dynamically or manually to match demand. These strategies are most commonly used with **Auto Scaling Groups (ASGs)**.

---

### 🔹 **Manual Scaling**

- **Definition**: Manually change the desired capacity of an Auto Scaling Group.
- **Use Case**: When you know the exact number of instances needed.
- **Pros**:
    - Full control
- **Cons**:
    - Not responsive to real-time traffic changes

---

### 🔹 **Dynamic Scaling**

- **Definition**: Automatically adds/removes instances based on real-time metrics (e.g., CPU usage, network traffic).
- **Types**:
    1. **Simple Scaling**:
        - One scaling action at a time.
        - Example: “If CPU > 70% for 5 minutes, add 1 instance.”
        - May cause delays due to cooldown periods.
    2. **Step Scaling**:
        - Adds/removes instances in steps based on metric ranges.
        - Example:
            - CPU < 30% → remove 2 instances
            - CPU > 70% → add 2 instances
        - More responsive and precise than simple scaling.
    3. **Target Tracking Scaling**:
        - Automatically adjusts to maintain a target metric.
        - Example: Maintain **average ASG CPU utilization around 40%**.
        - Similar to thermostat control.

---

### 🔹 **Scheduled Scaling**

- **Definition**: Scale in/out based on a predefined schedule (e.g., date/time).
- **Use Case**: Anticipating traffic spikes (e.g., sales events, work hours).
- **Pros**: Predictable scaling
- **Cons**: Doesn’t adapt to unexpected load changes

---

### 🔹 **Predictive Scaling (Using Machine Learning)**

- **Definition**: Uses ML to forecast future traffic based on past trends and scales ahead of time.
- **Use Case**: Applications with regular usage patterns (e.g., weekday morning traffic).
- **Pros**:
    - Proactive instead of reactive
    - Improves availability and cost-efficiency
- **Cons**:
    - Requires historical data
    - Might not suit unpredictable traffic

---
