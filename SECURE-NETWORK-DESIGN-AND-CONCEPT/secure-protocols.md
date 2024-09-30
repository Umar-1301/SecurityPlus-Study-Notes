# The different secure protocols

HTTPS : 443 - Secures web browsing by encrypting communication between a browser and a web server using SSL/TLS.
SSL/TLS : 443/465/993/995 - Provides encryption for data transmission across networks, commonly used in various secure protocols like HTTPS and SMTPS.
SSH : 22 - Enables secure remote login and command execution over an encrypted connection.
SFTP : 22 - Securely transfers files over SSH with encryption and authentication.
FTPS : 990 - An extension of FTP that encrypts file transfers using SSL/TLS.
IPsec : varies (typically 500 for IKE) - Secures IP communication by encrypting and authenticating data at the IP layer, often used in VPNs.
SMTPS : 465 - Sends emails securely by encrypting SMTP traffic using SSL/TLS.
POP3S : 995 - Encrypts the retrieval of emails from a mail server using SSL/TLS.
IMAPS : 993 - Provides secure access to emails stored on a server using SSL/TLS encryption.
LDAPS : 636 - Secures directory services communication by encrypting LDAP traffic with SSL/TLS.
DNSSEC : varies (53 for DNS) - Adds security to DNS by ensuring the authenticity and integrity of DNS data through digital signatures.
SNMPv3 : 161/162 - Secures network management communication with encryption and authentication features.
RDP : 3389 - Provides secure remote desktop access to computers, encrypting the session data.
Kerberos : 88 - Securely authenticates users and services within a network using secret-key cryptography.
OAuth : varies - Provides secure, token-based authorization to access resources without sharing credentials.

Think of port as a door way. Specific ports are used for specific services. When attempting SSH login, the port used to establish this is port 22
