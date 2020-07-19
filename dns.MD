# What is DNS? 
- https://aws.amazon.com/route53/what-is-dns/


# types of DNS Service: Authoritative DNS & recursive DNS
- Authoritative DNS: An authoritative DNS service provides an update mechanism that developers use to manage their public DNS names. It then answers DNS queries, translating domain names into IP address so computers can communicate with each other. Authoritative DNS has the final authority over a domain and is responsible for providing answers to recursive DNS servers with the IP address information. Amazon Route 53 is an authoritative DNS system.

- Recursive DNS: Clients typically do not make queries directly to authoritative DNS services. Instead, they generally connect to another type of DNS service known a resolver, or a recursive DNS service. A recursive DNS service acts like a hotel concierge: while it doesn't own any DNS records, it acts as an intermediary who can get the DNS information on your behalf. If a recursive DNS has the DNS reference cached, or stored for a period of time, then it answers the DNS query by providing the source or IP information. If not, it passes the query to one or more authoritative DNS servers to find the information.
- Route 53 had only the Authoritative type of DNS until Route 53 Resolver for hybrid clouds was launched in Nov 2018. 
