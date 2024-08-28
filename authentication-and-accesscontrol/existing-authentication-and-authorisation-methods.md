We have discussed the typed of authentication and how authentication controls/aspects are managed. Now lets delve into the existing practical examples of authentication methods

### Active directory - management
Microsoft Active directory ( AD ) is a solution to identity management, authorisation, and authentication within an organisation. It is used by admins to issue controls over different devices on the network
such as printers or laptops. They can manage these by creating new users, gorups, domains and organisational units, whilst also enforcing security policies across the network

It utilises LDAP ( lightwieght directory access protocol ) - protocol used to query and modify the AD. This is used when admin manage and change the AD, but also by devices that need to fetch information from the AD.
For example, i try to connect to a printer. It is a certificate based authentication in place. The printer will query the information on the certificate such as name through LDAP to the AD. As admins can configure the
AD to possess information regarding the relationship of user and authoristion, this query acts as authorisation for the user.


### kerberos - authentication protocol

Uses USN ( updated sequence number )
The user sends their username and password, and the TGT grants them a one-time ticket session which allows the user full access to the network in relation to their authentication level.
This is a single sign-on protocol


### NTLM

Like ketberos, but the older version and is vulnerable to MITM, brute force, pass the hash

### Transitive Trust

Made up of a parent and children domain. The children domain belong to a parent. 
parent - www.domain.com
child - www.domain/bookings.com

The user is allowed access to the bookings domain as they are trusted by the adult.
As we can setup domains in AD, this concept extends to AD. Domains in AD act as they would on a website - they are bordered and a collection of users,groups etc. Like a country. If country A is trusted by B
and we have access to B, we can access A


### Federation Services

Federation services enable secure, cross-domain authentication and resource access, allowing users to log in once and access resources across different organizations or systems, typically through protocols like 
SAML - open standard used for authenticating and authorising data between parties

user attempts connection to SP ( service provider )
SP uses SAML request and redirects user to IdP
IdP generates a SAML response
Used for single sign on

Where AD uses LDAP, this uses SAML


### OAuth

Services like sign in with google - uses a third party for authentication and authorisation

### Biometrics

Fingerprints and Face ID for example

FAR - False acceptance rate - how many time authirastion is given but it is false
FRR - False rejection rate - legit users denied access
CER - Efficiacy rates - the combination of FAR and FRR - the lower this is the better the authorisation mechanism



