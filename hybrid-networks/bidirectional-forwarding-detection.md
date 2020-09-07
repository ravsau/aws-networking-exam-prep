BFD is a detection protocol to provide fast forwarding path failure detection times, which allows for a faster routing reconvergence time. BFD is a mechanism independent of media, routing protocols, or data. It's a best practice to enable BFD for fast link failure detection and failover when connecting to AWS services over DX connections and AWS VPNs. Enabling BFD for your DX connection allows the Border Gateway Protocol (BGP) neighbor relationship to be torn down quickly after notifications from BFD. Otherwise, by default, BGP waits for three keep-alive failures of 90 seconds.

Asynchronous BFD is automatically enabled for DX virtual interfaces on the AWS side. However, you must configure your router for asynchronous BFD to enable it for your connection.

- Mainly used to detect DX failures
## Reference
https://aws.amazon.com/premiumsupport/knowledge-center/enable-bfd-direct-connect/
