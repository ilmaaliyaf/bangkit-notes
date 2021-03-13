taking large network and splitting it into smaller ones

## Subnet masks

Subnet ID
32-bit number

|   IP addr   |         9 |       100 |       100 |       100 |
|:-----------:| ---------:| ---------:| ---------:| ---------:|
|   IP addr   |  000 1001 | 0110 0100 | 0110 0100 | 0110 0100 |
| Subnet mask | 1111 1111 | 1111 1111 | 1111 1111 | 0000 0000 |
| Subnet mask |       255 |       255 |       255 |       254 | 

also written as 9.100.100.100/27
27 ones on subnet mask

the number in IP addr corresponding to 1 in subnet mask is the subnet ID
the number in IP addr corresponding to 0 in subnet mask is the host ID

only 1-124 address available for host ID

## [[Binary math]]

## CIDR
classless inter-domain routing
the slash notation: 9.100.100.100/27 above
allows for networks itself to have different size

example
/24 network is 8 host bits: 2^8 = 256
	we have 256-2 = 254 hosts available
/23 network is 9 host bits: 2^9 = 512
	we have 512-2 = 510 hosts available
	