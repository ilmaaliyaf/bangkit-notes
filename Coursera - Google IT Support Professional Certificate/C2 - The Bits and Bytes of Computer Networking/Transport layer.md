allows traffic to be directed to specific network applications

## multiplexing traffic
processes -> multiplexer -> IP
nodes on the network have the ability to direct traffic toweard many different reciving services

## demultiplexing traffic
IP -> multiplexer -> processes

## port
16-bit number to direct traffic
after a colon after IP address
example: 
	10.1.1.100:80

## FTP

## TCP
Encapsulation hierarcy: Ethernet -> IP diagram -> TCP segment

TCP heather The 20 bytes
1. Destination port (16)
2. Source port (16)
3. Sequence number (32)
4. Acknowledgment number
5. Header length (7)
6. Empty
7. Control flags
8. Windows (16)
9. Checksum (16)
10. Urgent pointer
11. Options
	complicated flows control
12. Padding
13. Data payload


### TCP Control Flags Handshake
1. URG (urgent)
2. ACK (acknowledges)
3. PSH (push), buffer
4. RST (reset)
5. SYN (synchronize)
6. FIN (finish)

(A) SYN -> (B) SYN/ACK -> (A) ACK -> repeat -> FIN -> ACK
Handshake: ensure two device talking in the same protocol

### TCP Socket States
Instantiation: actual implementation
- LISTEN, TCP ready to listen
- SYN_SENT
- SYN_RECIEVED
- ESTABLISHED, both sides free to send data
- FIN_WAIT, ACK hasn't been recieved yet
- CLOSE_WAIT
- CLOSED, no futher communication

## Connection
Connection-oriented protocol
	Established a connection, to ensure that all data has been properly transmitted
	ex: TCP
	- sequence number
Connectionless protocol
	just set a destinationed port, send the packet
	ex: UDP, streaming video

## Firewalls
a device that blocks traffic that meets certain criteria
- inspection of application layer traffect
- blocking ranges of IP address
