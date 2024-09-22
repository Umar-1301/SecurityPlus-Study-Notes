# DHCP - dynamic host config protocol

this is where the server allocates IP to clients
this is done through the DORA process

D - discover - client searches for server
O - offer - dhcp server responds to discover
R - request - client responds
A - acknowledgement/ACK - DHCP gives ip, subnet mask, DNS server

### commands
ipconfig /release - forces client to give up IP address
ipconfig /renew - used to get new ip address

169.254.x.x - issues getting private IP - due to exhausted resouces, incorrect network setup


assigning an ip address to a user is not bad, but controls should be in place
NAC - ensures ony authorised devices or users can access the network
segmentation - restrict new connections, uknown and guests can be isolated to VLAN
IDS/IPS - monitor network
MAC filtering and DHCP reservations - restrict based on the mac address


