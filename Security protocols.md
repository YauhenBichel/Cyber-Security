 Security protocols
     IPSec
     SSL
     TLS
 VPNs

## Security Protocols
 SET (Secure Electronic Transaction)
 SSL (Secure Sockets Layer ) protocol
 TLS (Transport Layer Security ) protocol
 SSH (Secure Shell)

 SSL used to secure HTTP
 HTTPS - port 443

 Problems with SSL
     Heartbleed – allowed anyone read the memory of vulnerable
    versions of the OpenSSL software
     Poodle and Drown


## Basic Security Requirements
 Confidentiality
 Repudiation
 Integrity
 Authentication
 Authorisation

## Virtual Private Network
Organisations need
• privacy for intra-organisation data exchange
• access to the Internet
 Private networks - using leased lines
 point-to-point links - problem is the cost

 VPN - appears to be a dedicated and secure link
between two sites
 advantages - lower cost

## Protocols to deliver VPN
 Key protocols used to implement VPNs
     PPTP (Point-to-Point Tunnelling protocol) – obsolete
     L2TP (Layer Two Tunnelling Protocol) – widely used and
    paired with IPSec
     OpenVPN – open source (uses AES_256 encryption with
    2048 bit RSA authentication and 160 bit SHA1 hash)
     SSTP (secure sockets tunnelling protocol) - 2048-bit TLS
    certificates for authentication and 256-bit SSL keys for
    encryption (MS developed)
     IKEv2 - Internet Key Exchange vs 2 (similar to L2TP) –
    uses IPsec for encryption and authentication


## VPN Characteristics
VPN’s have several characteristics:-
 Traffic is encrypted
 Remote site is authenticated
 Multiple protocols are supported
 Connection is point-to-point
 an end point may have several VPNs open with different starting points
 built to handle different application-level protocols 

## IPSec
• introduced to protect IP datagrams
• encrypts data between various devices
• transparent to the end user
• two encryption modes:
    – tunnel and transport
• Uses
    – data origin authentication
    – connectionless data integrity authentication
    – limited traffic flow confidentiality
    – also handles key exchanges
    – negotiation of algorithms

## IPSec Security Protocols
 Authentication Header (AH) provides:
- Connectionless integrity
- Data origin authentication
- Protection against replay attacks
 Encapsulating Security Payload (ESP)
provides:
- Confidentiality (encryption)
- Connectionless integrity
- Data origin authentication
- Protection against reply attacks
 Both protocols may be used alone or applied in
combination with each other.

## VPN
Benefits
 mainly cost
 user access to network and services
Dangers
 weak security at the remote site
 security policies at either end are critical
 authentication of each site is also important
 could allow an unauthorised user access to the network
 need to guard against viruses, worms and Trojan horses
 Heavy VPN traffic could overload VPN server
 need coherent addressing - alleviate addressing conflicts



