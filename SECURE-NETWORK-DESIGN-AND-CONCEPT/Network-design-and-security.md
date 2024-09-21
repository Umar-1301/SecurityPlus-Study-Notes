# Components of a network

* routers
* switches
* firewalls
* dhcp servers
* access points
* dns servers
* servers
* NICs


how to boost security?

honeypots - attracting attackers to a server or a site
honey file - purposely weak file

fake telementary - gives false information
proxy server - a fake server, serves as a gateway for end users and websites
  forward proxy - a server between two endpoints, for example a user, server, website - the server keeps logs
  jump server - used mainly for admins, they go to a jump server to jump to the desired location, jumpservers require credentials

load balancers - distributes traffic across servers to avoid overloading
  active/active - all nodes and servers are active
  active/passive - one node active, once overloaded, next node opens

load balancing methods:
- least utilised - directs load to least utilised node at the time
- affinity - linkes user to a server once session starts, allowing only that server to be in use so long as the sessione remains active
- DNS round robin - a list of servers. the list is used in order of the list not taking into account usage or load


types of proxy servers
forwarding
application - between client and specific app
reverse proxy - web to network, opposite of forwarding


the purposes of a forwarding proxy = filtering, caching for speed, 

