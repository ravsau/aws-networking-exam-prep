- VGWs are Not VPC Transitive 
- VGW VPN throughput capped at 1.25 Gbps
- VGW use single VPN tunnel endpoint when returning traffic to a network. Even if you have 2 VPN attached to a VPC. 
- Each AWS VPN IPsec tunnel only supports a single pair of one-way security associations
  - you have to wait until one tunnel times out to use a seperate set of security association
  - solution is to use only 1 policy for all network devices
  - another solution is to use route based VPN instead of policy based VPN
- Site to Site VPN only supports IPSec protocol 
- only iPv4 supported 




Credits: 
- ACG Course 
