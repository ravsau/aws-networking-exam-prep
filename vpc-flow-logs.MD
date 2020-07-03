## Reference
https://docs.aws.amazon.com/vpc/latest/userguide/flow-logs.html

## Flow logs basics
- You can create a flow log for a VPC, a subnet, or a network interface. If you create a flow log for a subnet or VPC, each network interface in that subnet or VPC is monitored.

- You can create flow logs for network interfaces that are created by other AWS services, such as:

    Elastic Load Balancing

    Amazon RDS

    Amazon ElastiCache

    Amazon Redshift

    Amazon WorkSpaces

    NAT gateways

    Transit gateways

    Regardless of the type of network interface, you must use the Amazon EC2 console or the Amazon EC2 API to create a flow log for a network interface.
