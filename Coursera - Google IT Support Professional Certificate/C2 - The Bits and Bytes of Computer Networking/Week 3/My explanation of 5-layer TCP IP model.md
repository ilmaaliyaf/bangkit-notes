Let's say Node A on Network A wants to established a TCP connection with Node B on Network B with both of them are in the same router, that is Router Z. 
1. Node A declare that it wants to establish a TCP connection with Node B's IP address and TCP port. 
2. Node A will examine its own subnet, then finds that it lives on Network A. Node A also finds that Node B is on another network, that is Network B. Node A will need to use its gateway to send data to Node B. Node A communicate with it's network through cables that is on physical layer. 
3. Node A then make ARP request for an IP address to the local network to find it's MAC address. We are on data link layer now. 
4. Router A recieve the ARP request then send the MAC address of Node A to Node A. 
5. Node A recieve the hardware address of its gateway. 
6. Node A constructs outbound TCP packet which need an outbound TCP port. Node A finds available ephemeral port and open a socket which will connect Node A with this post.
7. Node A build a TCP segment with appropriate fields in the header. The segment includes choosen source port and destination port, sequence number. SYN flag is set and checksum is calculated.
8. The TCP segment is passed to the IP layer by constructs an IP header filled with the source IP, destination IP, and TTL number. Then the data payload is inserted. At last, a checksum is calculated again.
9. Inserted with IP datagram and MAC addresses, Node A is ready to send the Ethernet frame.
10. The ethernet frame sent as binary data through cable connected between Node A and Network A's switch.
11. Network A forwards the frame to another end of the link that is Router Z.
12. Router Z recognized the MAC address then calculates a checksum check with the frame header. If it match, then the data is recieved in complete form.
13. Router Z strips the ethernet frame, leaving it with just the IP datagram.
14. Checksum is calculated again. If all match, Router Z looks at the routing table to find the destination IP address. It finds that the destination, Node B, are on Network B, within a direct reach of Router Z.
15. Router Z decrements TTL number by 1, then costruct a ethernet frame to be sent to Network B. 
16. Netowrk B forwards the ethernet frame to Node B. 
17. Node B recieves the frame and identifies its own MAC address as the destination. The ethernet frame then stripped away.
18. Node B examines the destination IP address then recognizes that as its own. The IP datagram then stripped away too.
19. Checksum is performed again for the TCP segment. With all checks out, Node B examines the destination port.
20. Node B ensure the port has an open socket. If yes, then Node B will sees that the packet has the SYN flag set.
21. Node B then examines the sequence number and stor it to craft a response. Node B will repeat the same process to send SYN-ACT response to Node A. 
22. And so on!