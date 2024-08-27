There are many types of authentication, each with uses in relation to business needs.

###Types of authentication

* Password-based Authentication - common authentication
* Multi-factor Authentication (MFA) - adds layered security, in case of, for example password, breach
* Biometric Authentication - face ID, fingerprint, voice
* Token-based Authentication - once a user gives password and has access, a token ( a long string of encrypted data ) is attatched to that user, authenticating them as they go about their business
* Certificate-based Authentication - a certificate is linked to the user containing their public key and digital signature. This allows recipients to validata the authenticity
* Single Sign-On (SSO) - signle sign on, so user can access different parts of the netwok without having to re-sign in
* Smart Card Authentication - having a physical card that only employees have
* OAuth/OpenID Connect - for example sign in with google
* Kerberos Authentication - widely used. contains authorisation server and tgt server ( ticket granting ). users are authenticated and then granted tickets. when trying to access network, the ticket is presented
* Challenge-Response Authentication - passwords and keys are never directly transmitted, instead a dynamic challenge is issued, and based on the response, access is granted. i want access, the client
                                      sends me a challenge containing a string of letters. then when i send my username of pw, this string is hashed. if the client gets the same hash i am granted access
* Location based - checks new device, travel time/impossible travel time, determined by IP


### Authentication management

Password keys - device that works in line with password
Password vaults - stores passwords, aes-256 encrypted
Trusted platform module - chip on motherboard, securely stores items such as keys, uses full disk encryption
HSM - portable, used to store keys, highly secure, if breach detected it will wipe all
