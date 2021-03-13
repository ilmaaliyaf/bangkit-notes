# Ethernet
- protocol on data link layer
- 1983 single collision domain
- carrier sense CSMA/CD
	- random interval

# MAC Address
media access control
identifier of a network
48 numbers grouping in hexadecimals or octet (8bit)

1. OUI
	manufacture identifier
2. the last three octets
	freely determined by manufacture
	
# Cast
Unicast
	one recieving address
Multicast
	determined by the MAC numbers
Broadcast
	send data to all

# Ethernet frames
data packet: single set of binary data being sent across a network link
1. Preamble
2. SFD, start frame delimiter
3. Destination MAC address
4. Source MAC address
6. VLAN header, segregate
5. EtherType field
7. Payload
8. FCS, frame check sequence
	CRC : polinomial division on data (checksum number)
	data integrity
	
	