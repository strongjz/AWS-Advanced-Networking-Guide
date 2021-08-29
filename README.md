# AWS-Advanced-Networking-Guide

* AWS Services
* AWS White Papers
* Courses 
* Blog Posts 
* Exam Guide 
* Sample Exams 
* Things to remember


| Domain | % of Exam |
|--------|-------------|
| Domain 1: Design and implement hybrid IT network architectures at scale | 24% |
| Domain 2: Design and implement AWS networks | 28% |
| Domain 3: Automate AWS tasks | 8% |
| Domain 4: Configure network integration with application services | 14% |
| Domain 5: Design and implement for security and compliance | 12% |
| Domain 6: Manage, optimize, and troubleshoot the network|  14% |


## AWS Services
* [VPC](https://aws.amazon.com/vpc/faqs/?ep=sec&sec=spec_advn)
  * NACL
  * Security Groups
  * VPC endpoints
  * Subnets
  * Route Tables
  * EC2
  * Placement groups
  * Enhanced networking
    * Secondary ENI
    * ENA
    * EFA
    * EBS Optimized
    * MTU
    * Throughput to the internet
  * VPC Traffic Mirroring
* [Direct Connect link](https://aws.amazon.com/directconnect/faqs/?ep=sec&sec=spec_advn)
* AWS and IPsec VPN
* Load Balancing
* AWS Global Accelerator
* Gateways 
  * Internet gateway 
  * Egress internet 
  * NAT gateway
  * Virtual GW
  * Customer gateway
  * AWS Transit Gateway
* AWS Config
* Amazon SNS
* AWS Lambda
* CloudFormation
* Amazon CloudWatch
* Amazon CloudWatch Logs
* Network Manager
* [Route 53](https://aws.amazon.com/route53/faqs/?ep=sec&sec=spec_advn)
* Network Security
  * VPC flow log
  * AWS CloudTrail
  * IAM policies
  * AWS KMS
  * AWS WAF
  * GaurdDuty
  * AWS Shield

## Networking Topics
* High availability/load balancing
* VLANs
* 801.q 
* BFD
* Routing
* Subnetting
* DNS
* DHCP
* Sticky Sessions
* DMZ
* Data at rest and in transit
* BGP 





## Whitepapers

* [Best Practices for VPCs and Networking in Amazon WorkSpaces Deployments](https://d1.awsstatic.com/whitepapers/best-practices-vpcs-networking-amazon-workspaces-deployments.pdf)
* [Building a Scalable and Secure Multi-VPC AWS Network Infrastructure](https://docs.aws.amazon.com/whitepapers/latest/building-scalable-secure-multi-vpc-network-infrastructure/welcome.html)
* [Amazon Virtual Private Cloud Connectivity Options](https://docs.aws.amazon.com/whitepapers/latest/aws-vpc-connectivity-options/welcome.html)
* [AWS Best Practices for DDoS Resiliency](https://d1.awsstatic.com/whitepapers/Security/DDoS_White_Paper.pdf)
* [High Performance Computing on AWS Redefines What is Possible](https://d1.awsstatic.com/whitepapers/Intro_to_HPC_on_AWS.pdf)
* [Integrating AWS with Multiprotocol Label Switching](https://d1.awsstatic.com/whitepapers/Networking/integrating-aws-with-multiprotocol-label-switching.pdf)
* [AWS Certified Advanced Networking Official Study Guide: Specialty Exam](https://www.amazon.com/Certified-Advanced-Networking-Official-Study-ebook/dp/B079VKD1CN)

## Courses

## Blog Posts

## Exam Guide

https://d1.awsstatic.com/training-and-certification/docs-advnetworking-spec/AWS-Certified-Advanced-Networking-Specialty_Exam-Guide.pdf

## Sample Exams

## Things to remember 

Route Table Priority

|Priority  |Description|
|----------|-------------|
|1	|Local route, even if a more specific route exists for the CIDR|
|2	|Most specific route (longest-prefix match)|
|3	|Static routes are preferred over dynamic routes for equivalent prefixes|
|4	|Dynamic routes propagated from AWS Direct Connect |
|5	|Static routes configured on a VGW VPN connection |
|6	|Dynamic routes propagated from a VPN |


VPC Endpoints 

Gateway endpoints ( Route Table entry )
  - Amazon Simple Storage Service (Amazon S3) 
  - Amazon DynamoDB. 

Interface endpoints ( ENI in your VPC )
  - Amazon Kinesis Streams
  - Elastic Load Balancing API
  - Amazon EC2 API 
  - Amazon EC2 Systems Manager (SSM)
  - AWS Service Catalog 
  - Endpoint services hosted by other account
  - Partner Solution s 