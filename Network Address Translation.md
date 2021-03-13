==NAT==
> A technology that allows a gateway, usually a router or firewall, to rewrite the source IP of an outgoing IP datagram while retaining the original IP in order to rewrite it into the response

![[Pasted image 20210313123416.png]]
Network A wants to communicate to Network B
with NAT, router will rewrite the source IP address, become a router's IP on network B.

IP masquerading: hiding the IP of computer 1 from computer 2

One-to-many NAT: the entire computers on Network A is masquaraded by the NAT router

## at the transport layer

Port preservation
> the source port chosen by a client is the same port used by the router

Port forwarding
> a specific destination ports can be configured to always be delivered to specific nodes

this allows for complete masquarade. as if the connection came from another network (?)


# RIR
IANA has primarily been responsible for assigning address blocks to the five regional internet registries or RIRs. The five RIRs are:

-   [**AFRINIC**](https://afrinic.net/), which serves the continent of Africa
-   [**ARIN**](https://www.arin.net/), which serves the United States, Canada and parts of the Caribbean
-   [**APNIC**](https://www.apnic.net/), which is responsible for most of Asia, Australia and New Zealand and Pacific Island nations
-   [**LACNIC**](https://www.lacnic.net/), which covers Central and South America and any parts of the Caribbean not covered by ARIN
-   [**RIPE**](https://www.ripe.net/), which serves Europe, Russia,the Middle East, and portions of Central Asia


IPv4 runs out of [[IP address]]

Then IPv6 is starting to be implemented. But it takes time and efforts.

Some temporary solution: non routable addresses. See [[Routing]].

