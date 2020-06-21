AWS Documentation reference: 
https://docs.aws.amazon.com/vpc/latest/userguide/vpc-endpoints.html



There are 2 types of VPC endpoints 
1) Gateway endpoints
    - A gateway endpoint is a gateway that you specify as a target for a route in your route table for traffic destined to a supported AWS service. The following AWS services are supported:

        - Amazon S3

        - DynamoDB
2) Inerface endpoints ( powered by Privatelink)
    - An interface endpoint is an elastic network interface with a private IP address from the IP address range of your subnet that serves as an entry point for traffic destined to a supported service. Interface endpoints are powered by AWS PrivateLink, a technology that enables you to privately access services by using private IP addresses. AWS PrivateLink restricts all network traffic between your VPC and services to the Amazon network. You do not need an internet gateway, a NAT device, or a virtual private gateway.
    - An interface VPC endpoint (interface endpoint) enables you to connect to services powered by AWS PrivateLink. These services include some AWS services, services hosted by other AWS customers and Partners in their own VPCs (referred to as endpoint services), and supported AWS Marketplace Partner services. The owner of the service is the service provider, and you, as the principal creating the interface endpoint, are the service consumer.

      The following services are supported:

      Amazon API Gateway

      Amazon AppStream 2.0

      AWS App Mesh

      Application Auto Scaling

      Amazon Athena

      AWS Auto Scaling

      AWS Certificate Manager Private Certificate Authority

      Amazon Cloud Directory

      AWS CloudFormation

      AWS CloudTrail

      Amazon CloudWatch

      Amazon CloudWatch Events

      Amazon CloudWatch Logs

      AWS CodeBuild

      AWS CodeCommit

      AWS CodePipeline

      AWS Config

      AWS Data Exchange

      AWS DataSync

      AWS Device Farm

      Amazon EC2

      EC2 Image Builder

      Amazon EC2 Auto Scaling

      AWS Elastic Beanstalk

      Amazon Elastic File System

      Elastic Load Balancing

      Amazon Elastic Container Registry

      Amazon Elastic Container Service

      Amazon EMR

      Amazon Fraud Detector

      AWS Glue

      AWS Key Management Service

      Amazon Keyspaces (for Apache Cassandra)

      Amazon Kinesis Data Firehose

      Amazon Kinesis Data Streams

      AWS License Manager

      Amazon Managed Blockchain

      Amazon Quantum Ledger Database (Amazon QLDB)

      Amazon RDS Data API

      Amazon Rekognition

      Amazon SageMaker and Amazon SageMaker Runtime

      Amazon SageMaker Notebook

      AWS Secrets Manager

      AWS Security Token Service

      AWS Server Migration Service

      AWS Service Catalog

      Amazon Simple Email Service (Amazon SES)

      Amazon SNS

      Amazon SQS

      AWS Step Functions

      AWS Systems Manager

      AWS Storage Gateway

      AWS Transfer for SFTP

      Amazon WorkSpaces

      Endpoint services hosted by other AWS accounts

      Supported AWS Marketplace Partner services
