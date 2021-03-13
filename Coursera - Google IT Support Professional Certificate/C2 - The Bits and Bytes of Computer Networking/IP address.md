32 bit long numbers
six 8 bits

distributed to companies and more structured

DHCP, dynamic host control process
Dynamic IP address
Static IP address

## IP datagram encapsulation
1. version
2. header lenght (20 bytes)
3. service type
	QoS
4. total length
5. identification
6. flag
7. fragmentation
8. TTL (time to live), protect from staying in misconfiguration
9. protocol
	tcp, udp
10. header checksum
11. source ip address
12. destination ip address
13. options, for testing purposes
14. padding, to ensure the header have correct size

## IP address classes
Network ID: first 3 octet
Host ID: last 3 octet
class A start with 0 - 127
class B 128 - 191
class C 192 - 223
class D 224 - 239
class E 240 - 255


## Address resolution protocol
ARP table: list of MAC address and corresponding IP address
	soon expired