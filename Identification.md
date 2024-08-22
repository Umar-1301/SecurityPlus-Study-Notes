### Identification
ID comes in many shapes, but the purpose is for secure access management, accounting for the user and esuring they have the correct authorisation
ID types:

* Name
* Card
* Certificate
* Digital Signature
* Keys
* Tokens

Lets talk about certificates and keys. Keys are generate for a new user. These are created in pairs for what is called asymetric enryption.
It is composed of a public key and a private key. The keys are like a block of text. 
Within Microsoft Azure, they offer symetric key generation as a service. These are encrypted with AES. Else, this can also be done through OpenSSL, PowerShell etc

Within an organisation, they handle this through the use of PKI framework ( public key infrastructure ) - think of a pki as a all-encompassing framework when it comes to keys.
It is comprised of:
* CA ( certificate authority )
* RA ( registration authority )
* Digital Certificates
* CRL ( certificate revocation list )
* OSCP ( online certificate status protocol )
* Certificate Stores


The process will go something like:
* key pair is generate, one for encryption ( public ) one for decrepytion ( private )
* public key along with details like org name, user name etc will be compiled into a CSR ( certificate signing request ). This will be hashed before sent and encrypt all data but public key - this is the signature
  * Optional Registartion authority can check the details as correct before sending on - either be a person or automated
* This will be checked by the intermediary ca, decrypt through public key, then encrypt again using its own private key - it will then send to root
* then the root ca will digitally sign using its own private key after using intermediate public key to verify it

This is used to establish a secure and authentic connection between to points in a network ( client to client, server to server, database to printer )
The recipient of this connection will send certificate to inter and then root, verifying the authenticity of the connection.
The data itself will be encrypted using the recipients public key, found on their certificate. On the other end, the sender will go through the same process of authenticity verification of the recipients certificate
The data can then be decrypted using the recipients private key, which within a PKI, can be stored in a KMS, HSM, local encrypted database etc

PKI framework is used only for asymetric keys - outlining guidlines, procedures, controls, management solutions etc. For example RA, CRL
The storing of private keys:
* HSM ( hardware security model )
* Encrypted files
* KMS

So we've established what assymetric keys are, what they verify, how this is done through PKI framework, and how certificates are created. But how do these endpoints communcate and carry these certificates and data to eachother?
= TCP/IP for network, HTTP for web

Think of it like a road that is created in seconds, from the sender to the recipient. The problem with this road is that the road itself is not encrypted, think of a thin road along a mountain.
The packet itself is encrypted, through the use of assymetric keys, as it uses the recipients public key to encrypt the packet. Think of the packet as a armoured car
However this armoured car can only carry a small amount of information that is encrypted such as a symmetric key - the reasons are because it takes too long if large data is present, and it is best practice to use a sym key



# Symetric Keys

Instead of 2 keys, there is a single used for both encrypting and decrypting. 
Instead of following PKI framework, the use of symetric keys implores different frameworks such as:
* NIST
* KMIP
* Cloud KMS

symetric keys do not use certificates, the key itself is encrypted with a master key, stored in a similiar fashion to assym keys, faster, TCP/IP communciation channels if used by themselves.
If TCP/IP is used that means only sym keys are in play - this is not secure enough for many reasons
Sym keys encrypt large amounts of data - armoured car becomes armoured bus - because it is quicker to decrypt by the recipient

The best practice is using TLS channel and the process of TLS handshake
this uses both sym and asym - the asym will be used to establish the correct connection and the TLS channel/road is encrypted giving us a safe road with gunmen situated on buildings - then the sym will encrypt the data which can be decrypted once it reached the recipient

## important note - the encryption of data is only when the data is in transit - once the date has reached the destination then it is no longer encrypted

















