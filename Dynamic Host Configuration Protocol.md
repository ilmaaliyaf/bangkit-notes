Four things a computer needs to configure to operate a modern network:
- IP address
- Subnet mask
- Gateway
- Name server

MAC address are assigned and hardcoded.

IP address needs to be unique for each node, unlike others.


==DHCP==
> [[Application layer]] protocol that automates the configuration process of hosts on a network.

![[Pasted image 20210313121853.png]]

## Dynamic allocation
Using IP addresses. assign these IPs to these devices ==when they request one==.
## Automatic allocation
Like dynamic allocation, but a range of IP addresses is already set and keep track of the assignments, assign the same IP for certain device like in the past, if possible.
## Fixed allocation
Assign IP address using MAC address. If MAC address is not found, use protocols above.


NTP: Network Time Protocol


# DHCP discovery
> the process by which a client configured to use DHCP attempts to get network configuration information

Steps:
1. Server discovery. DHCPDISCOVER
2. DHCP examines the configuration: choose dynamic, automatic, fixed. DHCPOFFER
3. client reponse DHCPREQUEST
4. server response DHCPACK

DHCP lease: expiration date for a discovery process

