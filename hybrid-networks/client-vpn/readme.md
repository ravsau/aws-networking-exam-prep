## Split tunnel 
https://docs.aws.amazon.com/vpn/latest/clientvpn-admin/split-tunnel-vpn.html

Split-tunnel on AWS Client VPN endpoints
PDF
RSS
By default, when you have an AWS Client VPN endpoint, all client traffic is routed over the AWS Client VPN tunnel. When you enable split-tunnel on the AWS Client VPN endpoint, we will push the routes on the AWS Client VPN endpoint route table to the device which is connected to the AWS Client VPN. This ensures that only traffic with a destination to the network matching a route from the AWS Client VPN endpoint route table is routed via the Client VPN tunnel.

You can use a split-tunnel AWS Client VPN endpoint when you do not want all user traffic to route through the AWS Client VPN endpoint.

Split-tunnel on AWS Client VPN endpoints benefits
Split-tunnel on AWS Client VPN endpoints offers the following benefits:

With split-tunnel, customers can optimize the routing of traffic from the client, by having only the AWS destined traffic traverse the VPN tunnel.

By optimizing the traffic, customers also reduce the volume of outgoing traffic from AWS, therefore reducing the data transfer cost.
