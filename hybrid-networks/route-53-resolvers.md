Route 53 Resolver Endpoints

Inbound query capability is provided by Route 53 Resolver Endpoints, allowing DNS queries that originate on-premises to resolve AWS hosted domains. Connectivity needs to be established between your on-premises DNS infrastructure and AWS through a Direct Connect (DX) or a Virtual Private Network (VPN). Endpoints are configured through IP address assignment in each subnet for which you would like to provide a resolver.

 

Conditional Forwarding Rules

Outbound DNS queries are enabled through the use of Conditional Forwarding Rules. Domains hosted within your on-premises DNS infrastructure can be configured as forwarding rules in Route 53 Resolver. Rules will trigger when a query is made to one of those domains and will attempt to forward DNS requests to your DNS servers that were configured along with the rules. Like the inbound queries, this requires a private connection over DX or VPN.

 



When combined, these two capabilities allow for recursive DNS lookup for your hybrid workloads. This saves you from the overhead of managing, operating and maintaining additional DNS infrastructure while operating both environments.


## Reference
https://aws.amazon.com/blogs/aws/new-amazon-route-53-resolver-for-hybrid-clouds/


--

https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/resolver.html#resolver-overview-forward-vpc-to-network
