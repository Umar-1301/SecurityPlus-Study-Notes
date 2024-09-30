### TCP

- connection oriented
- establishes connection before sending data
- three way handshake : syn, syn ack, ack
- reliable


### UDP

- conectionless
- Faster but less reliable

### unsafe protocols

HTTP : 80 - Unencrypted web traffic, vulnerable to eavesdropping and man-in-the-middle attacks.
FTP : 21 - Transfers files without encryption, exposing credentials and data to potential interception.
Telnet : 23 - Unencrypted terminal access, making it easy for attackers to intercept login credentials and session data.
POP3 : 110 - Unencrypted email retrieval, which can expose email credentials and content.
IMAP : 143 - Unencrypted email access protocol, vulnerable to interception.
SMTP : 25 - Unencrypted email sending, which allows attackers to capture messages and credentials in transit.
SNMPv1/v2 : 161/162 - Lacks encryption and authentication, exposing network management data to interception and manipulation.

