# The CIA Triad
model for designing security
- Confidentiality
	keeping things hidden
	- data leak
- Integrity
	keeping data accurate and untampered with
	- corrupted files
- Availability
	the information we have is readily accessible to those people that should have it
	- data loss
	- security down

# Essential Security Terms
- Risk
	the possibilty of suffering a loss in the event of an attack on the system
- Vulnerability
	a flaw in a system that could be exploited to compromise the system
	- 0-day vulnerability (zero day): a vulnerability that is not known to the software developer or vendor, but is known to an attacker
	- exploit: software that is used to take advantage of a security bug or vulnerability
	- threat: the possibility of danger that could exploit a vulnerability
- Hacker: someone who attempts to break into or exploit a system
	- black hat hacker
	- white hat hacker
- Attack: actual act of giving harm to the system

# Malicious Software
Malware
	malicious software that can be used to obtain sensitive information or delete or modify files
- viruses: attach itself to a program
- worms: live on their own and spread through network
	- Love Bug
- adware: software that display advertisements and collect data
- spyware: meant to spy on you
	- keylogger
- ransomware
	wannacry
- trojans: malware that disguise itself as other thing
- Bots: control other system
	- rootkit: run malicious proccesses
	- backdoors
	- botnets
	- logic bomb


# Network attack
- DNS Cache Poisoning Attack
	inserting fake DNS record
- Man-in-the-middle-attack
	- Session hijacking
	- Rogue AP
	- Evil twin

Denial-of-Service (DoS): overwhelming a service
	- Ping of Death (PoD)
	- ping flood, CIMP
	- SYN flood, half-open attack
	- Distributed DoS (DDoS)
	
	
Client-side attack
- Injection attack
	- Cross-site scripting (XSS)
	- SQL injection
Password attack
- brute force attack
Social engineering attack
- Phishing: disguise in something legitimate
	- spear phising
	- spoofing
	- baiting
	- tailgating



# Cryptography
- hiding info from unwanted recipients


security through obscurity

## symmetric cryptography

## asymmetric cryptogtaphy

## hashing
> a type of function or operation that takes in an aribitrary data input and maps it to an output of fixed size, called a hash or digest

N-data (variable length) --> hash function --> hash value (fixed length)

> you feed in any amount of data into a hash function and the resulting output will always be the same size, but the output should be unique to the input, such that two different inputs should never yield the same output.

- for uniquely identify data
- much faster search
- one directional
- ideally should be deterministic, the same input value should always return the same hash value
- should not contain hash collisions: two different inputs mapping to the same output
- operate on blocks of data

### hashing algorithms
- MD5
	- 1992
	- 512 bit blocks, generates 128 bit hash digest
	- suspectible to hash collision
		- flame malware
- SHA1 (secure hash algorithm)
	- 1995
	- 512 bit blocks, generates 160 bit hash digest
	- used in VCS
	- 2000, 2015, 2017 - hash collision
		- proved have full hash collision
- MIC (message integrity check)
### authentication
attacks
- brute force attacks
- rainbow table
protects
- password salt: additional randomized data

### public key infrastructure
- digital sertificate
- registration authority

[[Code - Encryption with MD5 and SHA]]