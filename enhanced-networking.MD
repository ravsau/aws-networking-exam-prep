### Enhanced Networking 

#### Reference: 
https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/enhanced-networking.html


### What is it? 
- Enhanced networking uses single root I/O virtualization (SR-IOV) to provide high-performance networking capabilities on supported instance types. 
- SR-IOV is a method of device virtualization that provides higher I/O performance and lower CPU utilization when compared to traditional virtualized network interfaces.
- Enhanced networking provides higher bandwidth, higher packet per second (PPS) performance, and consistently lower inter-instance latencies. 
- There is no additional charge for using enhanced networking.
- Amazon EC2 provides enhanced networking capabilities through the Elastic Network Adapter (ENA). 
  - To use enhanced networking, you must install the required ENA module and enable ENA support.
  - [ENA](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/enhanced-networking-ena.html) is a different construct from ENI


