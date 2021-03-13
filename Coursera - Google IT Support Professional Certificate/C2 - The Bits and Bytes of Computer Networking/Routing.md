## Router
a network device that forwards traffic depending on the destination addreses of that traffic

RFC

## Routing
Basic steps:
1. recieve data packet
2. examines destination IP
3. looks up IP destination network in routing table
4. forwards traffic to destination


## Routing table
contains:
- IP address
- Subnet Mask
- CIDR ID
- next hop
- total hops: find shortest path
- interface

## Routing protocols
### interior gateway protocols
sharing in single autonomous system
- link state protocol
	every router know every other routers
- distance-vector protocol
	every router only know direct neighboard routers
### exterior gateway protocols
IANA - internet assigned numbers authority, managed things like
- ip address allocations
- autonomous system number (ASN)



## RFC
Non-routable address space