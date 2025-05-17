1. Compute Services
🔹 Amazon EC2 (Elastic Compute Cloud)
📖 Definition: Virtual servers in the cloud.
⚙️ Usage: Host websites, applications, backend services.
✅ Flexible instance types, scalable, supports auto-scaling and load balancing.
⚠️ Requires management of OS, patching, and scaling if not automated.
🎯 Use Cases: Web hosting, application servers, batch processing.
📝 Note: Pay for what you use (On-Demand, Reserved, Spot Instances).
🔹 AWS Lambda
📖 Definition: Serverless compute service to run code in response to events.
⚙️ Usage: Event-driven tasks, microservices, automation.
✅ No server management, auto-scaling, pay-per-use.
⚠️ Cold start latency, limited runtime (15 mins).
🎯 Use Cases: Image resizing, API backend, IoT data processing.
📝 Note: Part of serverless stack with API Gateway and DynamoDB.
🔹 AWS Elastic Beanstalk
📖 Definition: Platform-as-a-Service to deploy web apps.
⚙️ Usage: Deploy web apps with minimal infrastructure management.
✅ Simplifies deployment, auto-scaling, supports many languages.
⚠️ Less control over infrastructure.
🎯 Use Cases: Fast app deployment for developers.
📝 Note: Handles EC2, ELB, Auto Scaling, etc. under the hood.
🔹 AWS Lambda@Edge
📖 Definition: Run Lambda functions at AWS Edge Locations.
⚙️ Usage: Customize CDN content delivery.
✅ Low latency, global delivery.
⚠️ Debugging can be harder.
🎯 Use Cases: Content personalization at CDN level.
📝 Note: Works with Amazon CloudFront.
✅ 2. Storage Services
🔹 Amazon S3 (Simple Storage Service)
📖 Definition: Object storage service with high durability.
⚙️ Usage: Store static files, backups, big data.
✅ Scalable, secure, durable (11 9s), multiple storage classes.
⚠️ Charges for requests, storage, and data transfer.
🎯 Use Cases: Media storage, website hosting, backup.
📝 Note: Versioning, lifecycle policies, and access control.
🔹 Amazon EBS (Elastic Block Store)
📖 Definition: Block storage for EC2 instances.
⚙️ Usage: Persistent storage for EC2.
✅ High performance, encrypted.
⚠️ Tied to a specific Availability Zone.
🎯 Use Cases: Databases, file systems.
📝 Note: Can take snapshots to S3.
🔹 Amazon EFS (Elastic File System)
📖 Definition: Managed network file system.
⚙️ Usage: Shared file access between EC2.
✅ Scales automatically, POSIX-compliant.
⚠️ Can be costly for large data.
🎯 Use Cases: CMS, shared access environments.
📝 Note: Works across multiple EC2 instances.
🔹 Amazon Glacier / S3 Glacier
📖 Definition: Low-cost archival storage.
⚙️ Usage: Backup, long-term storage.
✅ Very cheap, secure.
⚠️ Retrieval time can be hours.
🎯 Use Cases: Regulatory archive, cold data.
📝 Note: Use lifecycle policies to transition from S3 to Glacier.
✅ 3. Database Services
🔹 Amazon RDS (Relational Database Service)
📖 Definition: Managed relational database (SQL).
⚙️ Usage: Host MySQL, PostgreSQL, Oracle, SQL Server, MariaDB, Aurora.
✅ Automated backups, patching, scaling.
⚠️ Less control over DB server.
🎯 Use Cases: Web apps, e-commerce.
📝 Note: Use Multi-AZ for high availability.
🔹 Amazon DynamoDB
📖 Definition: Managed NoSQL database.
⚙️ Usage: Key-value and document storage.
✅ Fast, scalable, serverless.
⚠️ Complex queries not supported like SQL.
🎯 Use Cases: Gaming, IoT, session storage.
📝 Note: Integrates with Lambda and API Gateway.
🔹 Amazon Redshift
📖 Definition: Data warehouse for analytics.
⚙️ Usage: Run complex queries on big data.
✅ High performance, integrates with BI tools.
⚠️ Higher cost, not real-time.
🎯 Use Cases: Reporting, dashboards.
📝 Note: Columnar storage for speed.
✅ 4. Networking & Content Delivery
🔹 Amazon VPC (Virtual Private Cloud)
📖 Definition: Isolated virtual network in AWS.
⚙️ Usage: Launch AWS resources in private network.
✅ Full control over network config.
⚠️ Requires network knowledge.
🎯 Use Cases: Secure app hosting, private subnets.
📝 Note: Includes subnets, route tables, gateways.
🔹 AWS CloudFront
📖 Definition: CDN to deliver content globally.
⚙️ Usage: Cache and deliver static & dynamic content.
✅ Low latency, integrates with S3, Lambda@Edge.
⚠️ Cache invalidation can cost.
🎯 Use Cases: Media streaming, website acceleration.
📝 Note: Distributes content from Edge Locations.
🔹 AWS Route 53
📖 Definition: DNS service for domain registration and routing.
⚙️ Usage: Manage domain names, health checks.
✅ Scalable, integrates with other AWS services.
⚠️ Charges for hosted zones and queries.
🎯 Use Cases: Domain management, failover routing.
📝 Note: Supports routing policies like latency, geolocation.
✅ 5. Security, Identity & Compliance
🔹 AWS IAM (Identity and Access Management)
📖 Definition: Manage users and permissions.
⚙️ Usage: Grant access to AWS resources.
✅ Granular access, roles, policies.
⚠️ Misconfigured policies can cause vulnerabilities.
🎯 Use Cases: Access control, federated login.
📝 Note: Always follow least-privilege principle.
🔹 AWS KMS (Key Management Service)
📖 Definition: Create and manage encryption keys.
⚙️ Usage: Encrypt data across AWS.
✅ Integrated with many AWS services.
⚠️ Key misuse can lock out data.
🎯 Use Cases: Secure S3, EBS, RDS data.
📝 Note: Supports automatic key rotation.
🔹 AWS Shield
📖 Definition: DDoS protection service.
⚙️ Usage: Protect applications from network attacks.
✅ Always-on detection, free basic tier.
⚠️ Advanced version is paid.
🎯 Use Cases: Protect public-facing apps.
📝 Note: AWS Shield Advanced includes 24/7 support.
✅ 6. Management & Monitoring
🔹 AWS CloudWatch
📖 Definition: Monitoring and observability service.
⚙️ Usage: Collect metrics, logs, alarms.
✅ Real-time insights.
⚠️ Logging large volumes can cost.
🎯 Use Cases: System health monitoring, alerting.
📝 Note: Supports custom metrics.
🔹 AWS CloudTrail
📖 Definition: Logging and monitoring of API calls.
⚙️ Usage: Audit changes and actions.
✅ Records all account activity.
⚠️ Retention costs over time.
🎯 Use Cases: Security auditing, compliance.
📝 Note: Integrates with S3 for log storage.
🔹 AWS Trusted Advisor
📖 Definition: Recommends best practices across AWS.
⚙️ Usage: Cost optimization, security, fault tolerance.
✅ Easy insights, especially with Business/Enterprise support.
⚠️ Limited features in free tier.
🎯 Use Cases: Cost savings, security posture.
📝 Note: Use regularly to optimize.
