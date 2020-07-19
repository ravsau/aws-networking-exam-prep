

## AS Path and AS PATH Prepending 
https://www.noction.com/blog/as-path-and-as-path-prepending

What is an AS PATH?
- The main purpose of the AS path is to **avoid loops**. 
- The BGP AS path is a well-known mandatory attribute, which means that it’s present for all prefixes exchanged between BGP neighbors. When a BGP router sends out an update to a neighbor in a different autonomous system (i.e., an external or eBGP neighbor), it adds its own AS number to the front (left side) of the AS path. So the AS path lists all the ASes that need to be traversed to reach the location where the prefix that the path is attached to is advertised from. As such, a traceroute should encounter those same ASes.

## Why AS PATH prepend? 
- https://www.juniper.net/documentation/en_US/junos/topics/usage-guidelines/policy-prepending-as-numbers-to-bgp-as-paths.html
- Prepending an AS path makes a shorter AS path look longer and therefore less preferable to BGP.
- You can prepend one or more autonomous system (AS) numbers at the beginning of an AS path. The AS numbers are added at the beginning of the path after the actual AS number from which the route originates has been added to the path. 


