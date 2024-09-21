# network segmentation 

software defined networking (SDN) - software controllers or API to communicate with underlying hardware infrastructure

LAN - home network/intranet - all important data should be here

a screened subnet is a DMZ between the LAN and external networks
for an organisation this is where they would put services that need to be accessed by external people - web servers, DNS
- seperates the network
- security increased
- sclabaility
- decreases the attack vector
- can have firewall at the endge of screened subnet facing out and then facing inward

how to protect a network:
- physical: swicthes, routers, policies enforced on these
- segmentation: seperate important data from day to day
- logical vlan: seperates LAN into segments, done with switches
- zero trust: flages every connection
- virtualisation: virtual network use and machines

### Traffic flow

East to west - within a network between servers or VMS for example, microsegmentation is often used here in order to have heightened security
North to south - from internal to external network such as the internet or an external cloud service, this type of traffic normally passes through a firewall and passess the screened subnet
