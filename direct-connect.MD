##  What connection capacities are supported by AWS Direct Connect?

 - For Dedicated Connections, 1Gbps and 10Gbps ports are available.
 - For Hosted Connections, capacities of 50Mbps, 100Mbps, 200Mbps, 300Mbps, 400Mbps, 500Mbps, 1Gbps, 2Gbps, 5Gbps and 10Gbps may be ordered from approved AWS Direct Connect Partners.
## Q. Are there limits on the number of routes I can advertise towards AWS using AWS Direct Connect?

 - Yes, you can advertise up to 100 routes over each Border Gateway Protocol session using AWS Direct Connect.

## Q. Can I use AWS Direct Connect and a VPN Connection to the same VPC simultaneously?

Yes. However, only in fail-over scenarios. The Direct Connect path will always be preferred, when established, regardless of AS path prepending.

## Private VIF
- A private VIF is associated with a single VGW in a VPC.
