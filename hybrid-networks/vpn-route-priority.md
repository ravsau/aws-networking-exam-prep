

## Route tables and VPN route priority
Route tables determine where network traffic from your VPC is directed. In your VPC route table, you must add a route for your remote network and specify the virtual private gateway as the target. This enables traffic from your VPC that's destined for your remote network to route via the virtual private gateway and over one of the VPN tunnels. You can enable route propagation for your route table to automatically propagate your network routes to the table for you.

We use the most specific route in your route table that matches the traffic to determine how to route the traffic (longest prefix match). If your route table has overlapping or matching routes, the following rules apply:

If propagated routes from a Site-to-Site VPN connection or AWS Direct Connect connection overlap with the local route for your VPC, the local route is most preferred even if the propagated routes are more specific.

If propagated routes from a Site-to-Site VPN connection or AWS Direct Connect connection have the same destination CIDR block as other existing static routes (longest prefix match cannot be applied), we prioritize the static routes whose targets are an internet gateway, a virtual private gateway, a network interface, an instance ID, a VPC peering connection, a NAT gateway, a transit gateway, or a gateway VPC endpoint.

For example, the following route table has a static route to an internet gateway, and a propagated route to a virtual private gateway. Both routes have a destination of 172.31.0.0/24. In this case, all traffic destined for 172.31.0.0/24 is routed to the internet gateway — it is a static route and therefore takes priority over the propagated route.

Destination	Target
10.0.0.0/16	Local
172.31.0.0/24	vgw-11223344556677889 (propagated)
172.31.0.0/24	igw-12345678901234567 (static)


## Reference
https://docs.aws.amazon.com/vpn/latest/s2svpn/VPNRoutingTypes.html#vpn-route-priority
