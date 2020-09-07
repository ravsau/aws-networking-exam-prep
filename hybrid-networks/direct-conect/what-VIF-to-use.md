https://aws.amazon.com/premiumsupport/knowledge-center/public-private-interface-dx/

## Which type of virtual interface should I use to connect different resources in AWS?


AWS Direct Connect (DX) provides three types of virtual interfaces: public, private, and transit. How do I determine which type I should use to connect different resources (public or private) in AWS?
Resolution
To connect to AWS resources that are reachable by a public IP address (such as an Amazon Simple Storage Service bucket) or AWS public endpoints, use a public virtual interface. With a public virtual interface, you can:

- Connect to all AWS public IP addresses globally.
- Create public virtual interfaces in any DX location to receive Amazon’s global IP routes.
- Access publicly routable Amazon services in any AWS Region (except the AWS China Region).

To connect to your resources hosted in an Amazon Virtual Private Cloud (Amazon VPC) using their private IP addresses, use a private virtual interface. With a private virtual interface, you can:

- Connect VPC resources (such as Amazon Elastic Compute Cloud (Amazon EC2) instances or load balancers) on your private IP address or endpoint.
- Connect a private virtual interface to a DX gateway. Then, associate the DX gateway with one or more virtual private gateways in any AWS Region (except the AWS China Region).
- Connect to multiple VPCs in any AWS Region (except the AWS China Region), because a virtual private gateway is associated with a single VPC.


To connect to your resources hosted in an Amazon VPC (using their private IP addresses) through a transit gateway, use a transit virtual interface. With a transit virtual interface, you can:

-  Connect multiple VPCs in the same or different AWS account using DX.
-  Associate up to three transit gateways in the same AWS Region when you use a transit virtual interface to connect to a DX gateway.
-  Attach VPCs in the same AWS Region to the transit gateway. Then, access multiple VPCs in different AWS accounts in the same AWS Region using a transit virtual interface.
