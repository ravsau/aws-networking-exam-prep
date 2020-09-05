## Hybrid Connectivity
This section focuses on securely connecting your cloud resources with your on-premises data centers.
There are two approaches for enabling hybrid connectivity:
1. One-to-one connectivity — In this setup, a VPN connection and/or Direct Connect private VIF is
created for every VPC. This is accomplished by leveraging the virtual private gateway (VGW). This
option is great for small numbers of VPCs, but as a customer scales their VPCs, managing hybrid
connectivity per VPC can become difficult.
2. Edge consolidation — In this setup, customers consolidate hybrid IT connectivity for multiple VPCs
at a single endpoint. All the VPCs share these hybrid connections. This is accomplished by leveraging
AWS Transit Gateway and the Direct Connect Gateway.

#### Reference
https://d1.awsstatic.com/whitepapers/building-a-scalable-and-secure-multi-vpc-aws-network-infrastructure.pdf
