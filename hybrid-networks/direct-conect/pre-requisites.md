### Prerequisites
- For connections to AWS Direct Connect with port speeds of 1 Gbps or higher, ensure that your network meets the following requirements:

- Your network must use single-mode fiber with a 1000BASE-LX (1310 nm) transceiver for 1 gigabit Ethernet or a 10GBASE-LR (1310 nm) transceiver for 10 gigabit Ethernet.

- Auto-negotiation for the port must be disabled. Port speed and full-duplex mode must be configured manually.

- 802.1Q VLAN encapsulation must be supported across the entire connection, including intermediate devices.

- Your device must support Border Gateway Protocol (BGP) and BGP MD5 authentication.

- (Optional) You can configure Bidirectional Forwarding Detection (BFD) on your network. Asynchronous BFD is automatically enabled for AWS Direct Connect virtual interfaces, but does not take effect until you configure it on your router.

- https://docs.aws.amazon.com/directconnect/latest/UserGuide/getting_started.html#get-started-prerequisites
