## Reference
https://docs.aws.amazon.com/whitepapers/latest/aws-vpc-connectivity-options/aws-vpn-cloudhub.html


What you can do with it?
- Connect multiple on-prem offices without a VPC on AWS. Talk with your office resources across several networks. VPN Cloudhub facilitates that connectivity.

Building on the AWS managed VPN options described previously, you can securely communicate from one site to another using the AWS VPN CloudHub. The AWS VPN CloudHub operates on a simple hub-and-spoke model that you can use with or without a VPC. Use this approach if you have multiple branch offices and existing internet connections and would like to implement a convenient, potentially low-cost hub-and-spoke model for primary or backup connectivity between these remote offices.

The following figure shows the AWS VPN CloudHub architecture, with dashed lines indicating network traffic between remote sites being routed over their AWS VPN connections.

![image](https://user-images.githubusercontent.com/22568316/92329405-47fe4300-f035-11ea-8d6c-d3208624e81f.png)


Figure 11 - AWS VPN CloudHub

AWS VPN CloudHub uses an Amazon VPC virtual private gateway with multiple customer gateways, each using unique BGP autonomous system numbers (ASNs). Your gateways advertise the appropriate routes (BGP prefixes) over their VPN connections. These routing advertisements are received and re-advertised to each BGP peer so that each site can send data to and receive data from the other sites. The remote network prefixes for each spoke must have unique ASNs, and the sites must not have overlapping IP ranges.
