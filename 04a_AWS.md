# National Geospatial-Intelligence Agency (NGA)

# Moving Target Indicator (MTI) Software Modernization

## Attachment 04a: AWS Cloud Service Availability 

*Note: The implementation of some of these services is unique to TS C2S. Further exploration needed)*

*Assumption: SC2S will implement AWS services in the same way as TS C2S.*

| |   |
| --- | --- |
|Amazon EC2 Auto Scaling | 1. Launching Spot Instances not supported. 2. Unable to invoke a Lambda function - AWS Lambda not available. 3. Amazon EC2 launches instances into a VPC. 4. Amazon Resource Names and endpoints have different values. 5. Only signature version 4 signing supported. |
|AWS Billing and Cost Management |   |
|AWS CloudFormation | 1. Might need modify AWS CloudFormation sample templates and template snippets.2. Doesn&#39;t support AWS CloudFormation features and functionality after June 6, 2017.3. Does not support AWS Config 4. Does not support Amazon CloudWatch Logs 5. Cannot launch a stack using an IAM service role 6. CloudFormer not available 7. Amazon Resource Names and endpoints have different values 8. Amazon EC2 launches instances and Amazon RDS DB instances into a VPC 9. Only signature version 4 signing supported |
|AWS CloudHSM | 1. Unique commands to install AWS CloudHSM CLI tools 2. Need to add a configuration file to use AWS CloudHSM CLI tools 3. AWS CloudHSM not integrated with Amazon RDS for Oracle |
|AWS CloudTrail | 1. Amazon Resource Names and endpoints have different values.2. Only signature version 4 signing supported. |
|Amazon CloudWatch | 1. CloudWatch dashboards in the console are not available 2. Amazon Resource Names and endpoints have different values.3. Only signature version 4 signing supported. |
|Amazon CloudWatch Events | 1. Scheduleing events is not avaliable 2. Only Amazon SNS and Amazon Kinesis services are supported as targets for CloudWatch Events rules 3. Amazon Resource Names and endpoints have different values.4. Only signature version 4 signing supported. |
|Amazon CloudWatch Logs | 1. Amazon Resource Names and endpoints have different values.2. Only signature version 4 signing supported. |
|AWS CodeDeploy | 1. Integration with AWS Lambda not supported 2. Integration with AWS CloudFormation not supported 3. Integration with GitHub not supported 4. Integration with Elastic Load Balancing Application Load Balancers not supported 5. Amazon Resource Names and endpoints have different values.6. Only signature version 4 signing supported. | 
|AWS Config | 1. Does not support recording Amazon EC2 Dedicated Host, Amazon EC2 Systems Manager, Elastic Load Balancing, AWS CloudFormation Stacks 2. AWS Config Rules not supported |  
|AWS Database Migration Service | 1. Amazon Resource Names and endpoints have different values.2. Only signature version 4 signing supported. |
|AWS Data Pipeline | 1. Amazon Resource Names and endpoints have different values.2. Only signature version 4 signing supported. |
|AWS Diode |
|AWS Direct Connect | 1. Currently in closed Beta |
|Amazon DynamoDB | 1. Tagging for DynamoDB not available yet 2. DynamoDB Streams not available yet 3. Amazon Resource Names and endpoints have different values.4. Only signature version 4 signing supported. |
|Amazon Elastic Block Store | 1. Encypted snapshots and AIMs cannot be shared 2. Does not not support modifying the Size, IOPS or Type 3. Cross-region features are not supported 4. Amazon EC2 launches instances into a VPC instead of using the EC2-Classic platform 5. Amazon Resource Names and endpoints have different values.6. Only signature version 4 signing supported. |
|Amazon Elastic Compute Cloud | 1. Spot Instances are not available 2. Limited to running a total of 20 Reserve Instances 3. Dedicated Instances are available, but Dedicated Reserve Instances are not supported 4. Amazon EC2 launches instances into a VPC instead of using the EC2-Classic platform 5. Automatic Instance Recovery not supported 6. Amazon Resource Names and endpoints have different values 7. Only signature version 4 signing supported 8. VM Export not available  |
|Elastic Load Balancing | 1. Application Load Balancers not available 2. Does not support Route 53 features 3. Does not support IPv 64. Amazon EC2 launches instances into a VPC instead of using the EC2-Classic platform 5. Amazon Resource Names and endpoints have different values.6. Only signature version 4 signing supported. |
|Amazon EMR | 1. Only Hadoop version 2 supported 2. Hunk not available 3. MapR not available 4. Debugging not available 5. Amazon EC2 launches instances into a VPC instead of using the EC2-Classic platform 6. Amazon Resource Names and endpoints have different values.7. Only signature version 4 signing supported. |
|Amazon ElastiCache | 1. Exporting ElasticCache snapshots to Amazon S3 bucket not supported 2. Amazon EC2 launches instances into a VPC instead of using the EC2-Classic platform 3. Amazon Resource Names and endpoints have different values. 4. Only signature version 4 signing supported. |
|Amazon Glacier | 1. Amazon Resource Names and endpoints have different values.2. Only signature version 4 signing supported. |
|AWS Identity and Access Management | 1. No concept of root or account user. All C2S users are IAM users 2. Does not support adding multi-factor authentication (MFA) to IAM user or account 3. Web identity federation not available 4. Cannont upload and associate an X.509 certification with an individual IAM user 5. Cannont use IAM tags to add metadata to IAM user or role 6. Cannot use IAM tags to control permissions 7. No AWS services currently support service-linked roles 8. Amazon Resource Names and endpoints have different values.9. Only signature version 4 signing supported. |
|AWS Key Management Service | 1. Following services integrated with AWS KMS: AWS CloudTrail, Amazon EBS, Amazon EMR, Amazon Redshift, Amazon RDS (MySQL), Amazon S 32. Amazon Resource Names and endpoints have different values | 
|Amazon Kinesis | 1. Kinesis Firehose and Kinesis Analytics not available 2. Amazon Resource Names and endpoints have different values.3. Only signature version 4 signing supported. |
|Amazon Redshift | 1. Amazon Redshift clusters must be launch in an Amazon VPC 2. Snapshot copy not supported 3. Amazon Resource Names and endpoints have different values.4. Only signature version 4 signing supported. |
|Amazon Relational Database Service | 1. Support MySQL, MariaDB, PostgreSQL and Oracle DB engines supported 2. Oracle TDE with AWS CloudHSM not supported 3. MySQL 5.1 minor versions not supported 4. Cross-region features, such as DB snapshot-copying across regions, not supported 5. Sharing DB snapshot with other accounts not supported 6. Enhanced Monitoring for Amazon RDS not supported 7. Amazon EC2 launches instances into a VPC instead of using the EC2-Classic platform 8. Amazon RDS DB must use exisiting VPC security groups 9.  Amazon Resource Names and endpoints have different values.10. Only signature version 4 signing supported. |
|Amazon Simple Storage Service | 1. Data always encypted when object uploaded or copied 2. Cross-region copy operations not supported 3. Cross-region replication not supported 4. Reduced Redundancy Storage (RRS) storage class not supported 5. AWS Inport/Export service not available 6. BitTorrent support not available 7. Amazon S3 Transfer Acceleration not available 8. Amazon CloudFront not available 9. Amazon Resource Names and endpoints have different values.10. Only signature version 4 signing supported. |
|Amazon Simple Notification Service | 1. Cannot communicate to endpoint outside of the region 2. SMS or mobile puch notification not supported 3. Amazon SNS signs all notification deliveries using private-public key pair based on certificates 4. Amazon Resource Names and endpoints have different values.5. Only signature version 4 signing supported. | 
|Amazon Simple Queue Service | 1. Amazon Resource Names and endpoints have different values.2. Only signature version 4 signing supported. |
|Amazon Simple Workflow Service | 1. Amazon Resource Names and endpoints have different values.2. Only signature version 4 signing supported. |
|AWS Snowball | 1. Amazon Resource Names and endpoints have different values.2. Only signature version 4 signing supported. |
|Amazon Virtual Private Cloud | 1. Amazon EC2 launches instances into a VPC instead of using the EC2-Classic platform 2. VPC Internet gateways do not connect to the public Internet 3. Amazon Resource Names and endpoints have different values.4. Only signature version 4 signing supported. |


## NGA Base Services residing on AWS

* Active Directory
* Domain Name Service (DNS)
* Microsoft Patching WSUS
* VPC Creation Scripts
* Software repositories such as YUM
* SMTP
* HBSS
* BMC Patrol
* ACAS (Security Scanning tool)
* Arcsight
* Carbon Black
* VDSS
* F5
* Vormetric

## Available through NGA GEOINT Services

### Developer Tools

* Apigee
* EventKit
* GeoGig
* GeoPackage
* GeoWave
* HiPER LOOK
* MAGE
* MrGeo
* OpenSensorHub
* OpenStreetMap
* PostgreSQL DBaaS from Crunchy Data Solutions
* Rocket.Chat

## DevOps Tools

* Apigee
* GitLab
* Jenkins
* Nexus
* Pivotal Cloud Foundry (Dev-East, Ops-East, Ops-West)
* Redmine
* SonarQube
* Swagger
* ThreadFix
