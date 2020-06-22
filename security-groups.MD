- Security groups are associated with ENI's not EC2 intances. 
  - Security groups are associated with network interfaces. Changing an instance's security groups changes the security groups associated with the primary network interface (eth0).
    - https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-security-groups.html
    
