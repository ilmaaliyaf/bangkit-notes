#computerscience
Instructor: Victor Escobendo - Corporate Operation Engineer

# 1 Intro

Computer communicates with bit and bytes

Protocol
>a defined set of standards that computers must follow in order to communicate properly

Computer networking
>full scope of how computers communicate with each other

Two party:
- Server
- Client

How we model the network:
[[TCP IP five layer model]]

Other model: OSI
Read more: [SANS Institute: Reading Room - Standards](https://www.sans.org/reading-room/whitepapers/standards/paper/543)

# [[Networking devices]]

# [[Networking services]]

# [[Internet]]
## History
PSTN/POTS already global
1970s 
USENET created, soon to be dial-up

> baud rate: number of bits sent across a telephone line every second

## Dial-up Connection
- Use POTS (plain old telephone service) for data transfer.
- Connecting by actually dialing a phone number.
- Use device called modulator (modem) demodulator.
- Main way of how computer connects to each other for several decades

## [[Silos]]
## [[POTS and Dial-up]]
## [[Broadband Connection]]
## [[Wide Area Network vs PPVPN]]
## [[Wireless Networking]]


# Troubleshooting network problems
## ICMP
Internet Control Message Protocol
> a way of communicating why a transmission has failed, used by router or remote host

Fields:
1. Type (8)
2. Code (8)
3. Checksum (16)
4. Rest of the header (32)
5. Data section (payload, to know which transmission caused the error)

Ping
> send a special type of ICMP message called an **echo request**

if on, it will send back **echo reply**

## Traceroute
> utility to discover the path between two nodes, and give info about each hop along the way

## Public DNS Servers

# [[Cloud]]

# [[🍀 projects/2021-06-31 👩‍💻 bangkit - notes/IPv6]]