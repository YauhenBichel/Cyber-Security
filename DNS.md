## Classification of threats:
- Intrusion: security breach
- Blocking: DoS and DDoS attacks
- Malware: trojans, botnets, worms, viruses

The common gateway interface (CGI) is a standard way for a Web server to pass a Web user's request to an application program and to receive data back to forward to the user.

## DNS
Client requests the A record which represents an IP address

- How does a name server know that any response packet is "expected"?
- response arrives on the same UDP port - otherwise it's dropped
- Question section in the reply, matches the Question in the pending query
- The Query ID matches the pending query
- Query ID = 16 bits
- The Authority and Additional sections represent names that are within the same domain as the question: this is known as "bailiwick checking"

## DNS Spoofing
redirect users to a compromised server
- redirect corporate e-mail through a hacker's server
- DNS DoS attacks - rendered large sites inaccessible (e.g., E-Bay, Yahoo, etc)

Zone transfers
- DNS query – port 53 using UDP
- queries DNS using TCP – called a zone transfer
- restrict to authorised servers only
- configure firewall to block unauthorised in-bound
connections to TCP port 53
- tools – nslookup and Dig

## DNSSEC
DNSSEC is a secure version of the DNS protocol
- DANE* leans on DNSSEC to add support for out-of-bound certificate validation
- It provides support for:
- Certificate Authority pinning
- Certificate pinning (has to be signed by valid CA)
- Self-signed certificates
- Problems to overcome:
- Not everyone uses DNSSEC in clients
- DNS registrar hack can hijack your domain name (*) DNS-based Authentication of Named Entities 



