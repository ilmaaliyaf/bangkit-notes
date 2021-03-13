# DNS
We are hard in remembering bits. We remember words instead.

==Domain Name System==
> A global and highly distributed network service that resolves strings of letters into IP addresses for you

DN -> IP address
Example
IP address: 8.8.88
Domain Name: www.google.com

DNS lets organization decide which user get which IP depends on the user's region.

The hierarchy - remember!
1. IP address
2. Subnet mask
3. Gateway for a host
4. DNS server

## Types of DNS servers
- Caching name servers: store known domain name lookups *for certain amount of time*, ISP provided this
	- TTL: a value (in seconds) that can be configured by the owner of a domain name for how loang a name server is allowed to cache an entry before it should discard it and perform a full resolution again.
		Days ago TLL is in days, now in minutes or hours because of bandwidth improvement.
- Recursive name servers
- Root name servers
	- recieve full www.google.com
- TLD name servers
	- .com .net and such part
- Authoritative name servers
	- google.com and such part

Anycast: a technique that's used to route traffic to different destinations depending on factors like location, congestion, or link health

![[Pasted image 20210313114436.png]]

## DNS and UDP
The most common protocol.

Remember! Difference between TCP and UDP: UDP is connectionless. Check [[Transport layer]]

TCP: 44 packets
![[Pasted image 20210313115348.png]]

UDP: 8 packets
![[Pasted image 20210313115529.png]]
 UDP doesn't have any error recovery. Just ask DNS again. But UDP cannot cary big packet when the connection gets more complex. The server will change to TCP for that.
 
 ## Resource Record Types
 
 - A record: certain domain name with IPv4
	 - Round robin concept: iterate through everyone (IPs)
 - AAAA or Quad A: for IPv6
 - CNAME record: canonical name, redirections, we get to microsoft page both by access microsoft.com and www.microsoft.com
 - MX record: mail exchange, 
 - SRV record: service exchange
	 stipulating specifications of the DNS such as the port numbers, servers, hostname, priority and weight, and IP addresses of defined or cataloged services servers
 - TXT record: communicate configuration between companies in human languange within domain name

## Zones
They don't overlap. Easier control over multiple level of domain name.
en.google.com
id.google.com
etc

Zone file
- Start of Authoraty (SOA)
- NS record
- and other record like above serource records
- Reverse lookup zone files
- PTR: resolves an IP to a name
 
# Anatomy of a Domain Name
 
- TLD: Top Level Domain
	- .com .org .net .co.id
	- handled by ICANN, sister of IANA
- Domain: the name
	- google
	- must meet the criteria of TLEs
- Subdomain
	- www part

Fully qualified domain name (FQDN): combine all above parts

Registrar: company who control the domain

DNS can handle to 127 levels domain name
Each section can be 63 char long
FQDN 255 char long
