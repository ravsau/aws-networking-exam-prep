Local preference communities for private virtual interface
Q. What is this feature?

This feature provides support for local preference communities for private virtual interfaces. With communities, customers can influence the return path for traffic sourced from VPC address space.




https://aws.amazon.com/directconnect/faqs/#Local_preference_communities_for_private_virtual_interface



- Local preference BGP community tags are evaluated before any AS_PATH attribute, and are evaluated in order from lowest to highest preference (where highest preference is preferred).

- If you do not specify local preference community tags, the default local preference is based on the distance to the AWS Direct Connect location.


https://docs.aws.amazon.com/directconnect/latest/UserGuide/routing-and-bgp.html

