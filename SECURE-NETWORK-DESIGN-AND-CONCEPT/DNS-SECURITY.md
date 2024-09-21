# Domain name system
maps domain to ip addresses

A - ipv4
AAAA - ipv6
CNAME - used to create alias for another domain or subnet
MX - mail server
SRV - port to a service
SPF - txt files that DNS use to stop unwanted traffic
DMARC - txt files used by IPS to stop phishing

<img width="558" alt="image" src="https://github.com/user-attachments/assets/276139fc-72e9-43b2-a4a0-e6b8339eb48c">

### DNS attacks
DNS poisoning - fake website, injecting a record into the DNS server | most common ID poisoning DNS cache
DNS hijacking
DDos attacks
DNS amplification

DNSSEC - use of digital signatures based on public key cryptography
       - DNS records are signed = RRSIG providing integrity


DNS sinkhole:
- provide false information to attacker
- blocks certain conent types in network


### IP addresses
public: each device has one

private: inside network given by DHCP
class:
A - 10.0.0.0
B - 172.16.x.x
C - 192.168.0.0

subnet mask - 32 bit
ip - network = 255.0
host         = 0.0


ipv6: 64 bit hexadecimal
public: 2001,2002,2003 - used externally
linklocal: Fe80
unique local: Fc00, Fd00

![image](https://github.com/user-attachments/assets/ca9a7562-75b0-45a0-a4dd-4a465bc85251)




