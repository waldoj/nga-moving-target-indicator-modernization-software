# National Geospatial-Intelligence Agency (NGA)

# Moving Target Indicator (MTI) Software Modernization

## Attachment 04a: AWS Cloud Service Availability 

*Note: The implementation of some of these services is unique to TS C2S. Further exploration needed. All of the below services are available on .mil, SC2S, and TSC2S Environments.*

*Assumption: SC2S will implement AWS services in the same way as TS C2S.*

| |   |
| --- | --- |
|Amazon EC2 Auto Scaling | 1. Launching Spot Instances not supported.<br>2. Unable to invoke a Lambda function - AWS Lambda not available.<br>3. Amazon EC2 launches instances into a VPC.<br>4. Amazon Resource Names and endpoints have different values.<br>5. Only signature version 4 signing supported. |
|AWS Billing and Cost Management |   |
|AWS CloudFormation | 1. Might need to modify AWS CloudFormation sample templates and template snippets.<br>2. Does not support AWS CloudFormation features and functionality after June 6, 2017.<br>3. Does not support AWS Config<br>4. Does not support Amazon CloudWatch Logs<br>5. Cannot launch a stack using an IAM service role<br>6. CloudFormer not available<br>7. Amazon Resource Names and endpoints have different values<br>8. Amazon EC2 launches instances and Amazon RDS DB instances into a VPC<br>9. Only signature version 4 signing supported |
|AWS CloudTrail | 1. Amazon Resource Names and endpoints have different values.<br>2. Only signature version 4 signing supported. |
|Amazon CloudWatch | 1. CloudWatch dashboards in the console are not available<br>2. Amazon Resource Names and endpoints have different values.<br>3. Only signature version 4 signing supported. |
|Amazon CloudWatch Events | 1. Scheduleing events is not avaliable<br>2. Only Amazon SNS and Amazon Kinesis services are supported as targets for CloudWatch Events rules<br>3. Amazon Resource Names and endpoints have different values.<br>4. Only signature version 4 signing supported. |
|Amazon CloudWatch Logs | 1. Amazon Resource Names and endpoints have different values.<br>2. Only signature version 4 signing supported. |
|AWS CodeDeploy | 1. Integration with AWS Lambda not supported<br>2. Integration with AWS CloudFormation not supported<br>3. Integration with GitHub not supported<br>4. Integration with Elastic Load Balancing Application Load Balancers not supported<br>5. Amazon Resource Names and endpoints have different values.<br>6. Only signature version 4 signing supported. | 
|AWS Config | 1. Does not support recording Amazon EC2 Dedicated Host, Amazon EC2 Systems Manager, Elastic Load Balancing, AWS CloudFormation Stacks<br>2. AWS Config Rules not supported |  
|AWS Database Migration Service | 1. Amazon Resource Names and endpoints have different values.<br>2. Only signature version 4 signing supported. |
|AWS Data Pipeline | 1. Amazon Resource Names and endpoints have different values.<br>2. Only signature version 4 signing supported. |
|AWS Diode |
|AWS Direct Connect | |
|Amazon DynamoDB | 1. Tagging for DynamoDB not available yet<br>2. DynamoDB Streams not available yet<br>3. Amazon Resource Names and endpoints have different values.<br>4. Only signature version 4 signing supported. |
|Amazon Elastic Block Store | 1. Does not not support modifying the Size, IOPS or Type<br>2. Cross-region features are not supported<br>3. Amazon EC2 launches instances into a VPC instead of using the EC2-Classic platform<br>4. Amazon Resource Names and endpoints have different values.<br>5. Only signature version 4 signing supported. |
|Amazon Elastic Compute Cloud | 1. Spot Instances are not available<br>2. Dedicated Instances are available, but Dedicated Reserve Instances are not supported<br>3. Amazon EC2 launches instances into a VPC instead of using the EC2-Classic platform<br>4. Automatic Instance Recovery not supported<br>5. Amazon Resource Names and endpoints have different values<br>6. Only signature version 4 signing supported<br>7. VM Export not available  |
|Elastic Load Balancing | 1. Does not support Route 53 features<br>2. Does not support IPv 6<br>3. Amazon EC2 launches instances into a VPC instead of using the EC2-Classic platform<br>4. Amazon Resource Names and endpoints have different values.<br>5. Only signature version 4 signing supported. |
|Amazon EMR | 1. Only Hadoop version 2 supported<br>2. Hunk not available<br>3. MapR not available<br>4. Debugging not available<br>5. Amazon EC2 launches instances into a VPC instead of using the EC2-Classic platform<br>6. Amazon Resource Names and endpoints have different values.<br>7. Only signature version 4 signing supported. |
|Amazon ElastiCache | 1. Exporting ElasticCache snapshots to Amazon S3 bucket not supported<br>2. Amazon EC2 launches instances into a VPC instead of using the EC2-Classic platform<br>3. Amazon Resource Names and endpoints have different values.<br>4. Only signature version 4 signing supported. |
|Amazon Glacier | 1. Amazon Resource Names and endpoints have different values.<br>2. Only signature version 4 signing supported. |
|AWS Identity and Access Management | 1. No concept of root or account user. All C2S users are IAM users<br>2. Does not support adding multi-factor authentication (MFA) to IAM user or account<br>3. Web identity federation not available<br>4. Cannont upload and associate an X.509 certification with an individual IAM user<br>5. Cannot use IAM tags to add metadata to IAM user or role<br>6. Cannot use IAM tags to control permissions<br>7. No AWS services currently support service-linked roles<br>8. Amazon Resource Names and endpoints have different values.<br>9. Only signature version 4 signing supported. |
|AWS Key Management Service | 1. Following services integrated with AWS KMS: AWS CloudTrail, Amazon EBS, Amazon EMR, Amazon Redshift, Amazon RDS (MySQL), Amazon S3<br>2. Amazon Resource Names and endpoints have different values | 
|Amazon Kinesis | 1. Kinesis Firehose and Kinesis Analytics not available<br>2. Amazon Resource Names and endpoints have different values.<br>3. Only signature version 4 signing supported. |
|Amazon Redshift | 1. Amazon Redshift clusters must be launch in an Amazon VPC<br>2. Snapshot copy not supported<br>3. Amazon Resource Names and endpoints have different values.<br>4. Only signature version 4 signing supported. |
|Amazon Relational Database Service | 1. Support MySQL, MariaDB, PostgreSQL and Oracle DB engines supported<br>2. Oracle TDE with AWS CloudHSM not supported<br>3. MySQL 5.1 minor versions not supported<br>4. Cross-region features, such as DB snapshot-copying across regions, not supported<br>5. Sharing DB snapshot with other accounts not supported<br>6. Enhanced Monitoring for Amazon RDS not supported<br>7. Amazon EC2 launches instances into a VPC instead of using the EC2-Classic platform<br>8. Amazon RDS DB must use exisiting VPC security groups<br>9.  Amazon Resource Names and endpoints have different values.<br>10. Only signature version 4 signing supported. |
|Amazon Simple Storage Service | 1. Data always encypted when object uploaded or copied<br>2. Cross-region copy operations not supported<br> 3. Cross-region replication not supported<br> 4. Reduced Redundancy Storage (RRS) storage class not supported<br> 5. AWS Import/Export service not available (though can be simulated with Snowball)<br> 6. BitTorrent support not available<br> 7. Amazon S3 Transfer Acceleration not available<br> 8. Amazon CloudFront not available<br> 9. Amazon Resource Names and endpoints have different values.<br>10. Only signature version 4 signing supported. |
|Amazon Simple Notification Service | 1. Cannot communicate to an endpoint outside of classified networks<br>2. SMS or mobile push notification not supported<br>3. Amazon SNS signs all notification deliveries using private-public key pair based on certificates<br>4. Amazon Resource Names and endpoints have different values.<br>5. Only signature version 4 signing supported. | 
|Amazon Simple Queue Service | 1. Amazon Resource Names and endpoints have different values.<br>2. Only signature version 4 signing supported. |
|Amazon Simple Workflow Service | 1. Amazon Resource Names and endpoints have different values.<br>2. Only signature version 4 signing supported. |
|AWS Snowball | 1. Amazon Resource Names and endpoints have different values.<br>2. Only signature version 4 signing supported. |
|Amazon Virtual Private Cloud | 1. Amazon EC2 launches instances into a VPC instead of using the EC2-Classic platform<br>2. VPC Internet gateways do not connect to the public Internet<br>3. Amazon Resource Names and endpoints have different values.<br>4. Only signature version 4 signing supported. |


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
* Chat

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
