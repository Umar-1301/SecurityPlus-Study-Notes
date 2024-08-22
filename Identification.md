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
* public key along with details like org name, user name etc will be compiled into a CSR ( certificate signing request )
* this will be sent to CA
* CA will issue a certificate, signing it with the public key
* The other components such as CRL, Certificate storage are also utilised in a PKI

Think of PKI as the word fastfood - it is not the be all end all of certificates, rather the encompassing name which fastfood branches contribute to.

The private key will be stored in a secure location, but where end-point clinets ( websites, routers, email client ) have access to it to verify data being sent on the the network
