Before VPNS we had remote access servers - these can still be used although they are:
- slower
- server inside company network

VPNS are now widely used. it works over the internet and due to this must be secured

L2TP/IPsec - ensures both secure tunnel and authentication
L2TP - layer 2 tunnelling protocol - establishes a vpn connection tunnel but does not provide encryption by itself
IPSEC - internet protocol security layer 3 - provides ecryption and authentication of data passing through the tunnel
  * contains authentication header - SHA1 or MD5 hashing
  * Encapsulated security payload - DES, 3DES, AES

SSL socket layer - older systems using SSL certificates for authentication
HTML5 VPN - uses certificates for authentication


### IPSEC steps
so ipsec by itself can be used for tunneling and the encryption

the steps are:
SA negotiation - devices agree on authentication and encryption
IKE ( internet key exchange ) phase 1 - secure tunnel is established for negotiations
IKE phase 2 - actual ipsec tunnel is turned on
data transfer - data is encrypted and transferred
re-keying - keys are periodically refreshed
tunnel termination

the reason we use L2TP with ipsec eventhough ipsec can create the tunnel itself is:
- seperation of duties
- multiprotocol support
- double encapsulation
- higher security
- NAT traversal - nat allows multiple private ip addresses to use one public ip address, enhancing security by hiding internal network affairs


### Different types of remote

SSH - remote server, encrypts all data, public and private key, anternative to telnet and rlogin
powershell - microsofts version of remote access
remote desktop protocol - securely conects windows devices remotely
