# AAA servers - port 1812

First lets define a server - a server is a service. On a server specific tasks can be cnfigured such as databases, website hosting, running applications etc. 
Think of this as a huge plot of land, where the roads we established and the cars, can go to a from, and within these plots of land, they have their own roads and cars to travel to endpoints, which do an action to contribute to the purpose of that server/plot of land

A network will be made up of many servers, some servers containing an index of servers and so on.
Now the purpose of an AAA server is to authenticate, authorise and account for people trying to access the network through clients.

Acessing the network encompasses the initial connection to the network, and subsequent activity on the network requiring a road to the different components of the network
Physical connection - wired connection to a switch or router for example. when plugging in the ethernet to the client ( the end device trying to establish a connection ) the switch will forward the credentials to the AAA server. The AAA will be able to authorise if the user is authorised in its configuration if the shared  secret is correct.
The shared secret is pre configured between that specific client and the AAA server. So the username and pw of the user, paired with the shared secret, ensures integrity, authentication, and authorisation. The AAA server then sends a grant or deny

Accessing the network = network access points
Physical - switch, wire
Wireless - WAP ( wireless access points )
VPN/remote access - secure remote access over wifi

The AAA is configured to work whenever one of their clients is contacted or requested to be used. It's purpose is to add a layer of security
For example a VPN connection:
- i use my client ( laptop ) to connect to the network through VPN connection
- The AAA does its thing
- My client and a VPN gateway try to establish connection. The VPN gateway is a piece of software, server or endpoint device
- This connection is facilitated through TLS
- I am assigned a host ip address and when trying to connect to other clients on the network, it utilises layer 3 switchhing, my ip address and the clients ip address to facilitiate this.


### Extra security

my request is no longer sent directly to the AAA server. Instead the client is configured to filter traffic, rate-limit. This effectively keeps the request at the network edge and adds an extra layer of segmentation. Physical ( wired and wireless ) and VPN connections use different frameworks due to the protocols these frameworks have and cosiderations
that are made due to the difference in nature of the connection type

802.1x - Physical wired or wireless access points - l2 switches, l2 routers, WAPS, VOIP - EAP protocols
RAS - VPN connections - full encryption, l3 switches, l3 routers - PAP, CHAP, MCCHAPv2

## Radius

AAA server - Password encryption, username shown - UDP packets

## TACACS+

AAA server - Full packet encryption - TCP packets - more focused on admin access of network and client management - seperates authentication, authorisation and accounting to different servers

## Diamter

AAA server - TCP - successor to radius - end to end encryption

communication protocols:
EAP-TLS - certificate used by both client and AAA for authentication
PEAP - encapsulates in TLS tunnel and uses server side certificate similiar to RAS but only for the initial connection to the client
FAST - PEAP but faster, uses protected access credentials instead of certificates
TTLS - same as TLS but only required server to have certificate



### Application protocols

TLS - layer 4 transport protocol - protecting data in transit
IPsec - layer 3 network - securing ip based connections, specifically used with VPN's
