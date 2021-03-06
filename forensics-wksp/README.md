# Forensics Workshop

This workshop is designed to help you get familiar with AWS Security services and learn how to use them to perform forensics on incidents and to detect threats that cause the incidents.  You'll be working with services such as Amazon GuardDuty, Amazon Inspector, Amazon CloudWatch, AWS Lambda, AWS Systems Manager, AWS Config, AWS CloudTrail, and AWS Athena. You will learn how to use these services to set up a notification and remediation pipeline, investigate threats during and after an attack, and  add additional protections in place to improve the security posture of your environment.

### Scenario

Your company is new to the cloud and has recently performed a lift-and-shift of your infrastructure for piloting purposes.  You are a systems administrator and have been tasked with security monitoring within your AWS environment.  As part of that maintenance you are also responsible for responding to any security event in your environment.

### Architecture overview

For this Workshop you will have a single instance setup in the us-west-2 region. As this was a “lift-and-shift” migration for piloting, you have yet to build redundancy into your application, so you have a single public-facing webserver. The webserver has access to the Internet Gateway through an Elastic Network Interface. Customers access your web server through a DNS entry pointing to the Elastic Network Interface. You store static content in an S3 bucket and use the VPC S3 Endpoint Gateway for access from the webserver.

![Architecture](./images/diagram-basic-arch.png "Lab Workload Architecture")

Before you migrated the application you saw a webinar about AWS security best practices. Because of that webinar, you knew to enable a number of Security services provided by AWS. 

### Region
Please use the **us-west-2 (Oregon)** region for this workshop.

### For instructors
If you would like to teach this workshop to a group of students, the instructions can be found [here](./docs/workshop-delivery-instructions.md).

### Modules
1. [Environment Build and Configuration](./docs/01-environment-setup.md)
2. [Attack Simulation](./docs/02-attack-simulation.md) 
3. [Forensics and Remediation](./docs/03-forensics-and-remediation.md) 
4. [Review and Cleanup](./docs/04-review-and-cleanup.md)

> Total time: &plusmn; 2 hours
