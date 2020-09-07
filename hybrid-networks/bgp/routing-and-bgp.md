https://docs.aws.amazon.com/directconnect/latest/UserGuide/routing-and-bgp.html

Public virtual interface routing policies
If you're using AWS Direct Connect to access public AWS services, you must specify the public IPv4 prefixes or IPv6 prefixes to advertise over BGP.

The following inbound routing policies apply:

You must own the public prefixes and they must be registered as such in the appropriate regional internet registry.

Traffic must be destined to Amazon public prefixes. Transitive routing between connections is not supported.

AWS Direct Connect performs inbound packet filtering to validate that the source of the traffic originated from your advertised prefix.

The following outbound routing policies apply:

- AS_PATH is used to determine the routing path, and AWS Direct Connect is the preferred path for traffic sourced from Amazon. Only public ASNs are used internally for route selection.

- AWS Direct Connect advertises all local and remote AWS Region prefixes where available and includes on-net prefixes from other AWS non-Region points of presence (PoP) where available; for example, CloudFront and Route 53.

- AWS Direct Connect advertises prefixes with a minimum path length of 3.

- AWS Direct Connect advertises all public prefixes with the well-known NO_EXPORT BGP community.

- If you have multiple AWS Direct Connect connections, you can adjust the load-sharing of inbound traffic by advertising prefixes with similar path attributes.

- The prefixes advertised by AWS Direct Connect must not be advertised beyond the network boundaries of your connection. For example, these prefixes must not be included in any public internet routing table.

- AWS Direct Connect does not re-advertise customer prefixes to other customers that have been received over AWS Direct Connect public virtual interfaces.

