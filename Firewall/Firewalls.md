Firewall - system or group of systems that enforces an access control
policy between two networks

two mechanisms:
 one that blocks traffic
 one which permits traffic

 monitors and controls traffic into and out of secure
networks
 normally located at the gateway to a network

## Firewalls: Why do we need one?
Prevent denial of service attacks:
• SYN flooding: attacker establishes many bogus TCP
connections, no resources left for “real” connections
Prevent illegal modification/access of internal data.
• e.g., attacker replaces homepage with something else
allow only authorized access to inside network (set of
authenticated users/hosts)
Three main types of firewalls:
• stateless packet filters
• stateful packet filters (deep packet inspection)
• application (proxy) gateways

Firewalls have the following design goals:-
1. All traffic from inside to outside must pass through the firewall
2. and vice versa
3. Only authorised traffic will be allowed to pass (defined by the local
security policy)
4. The firewall itself is immune to penetration
Provides access control and enforcement of a site’s security policy


## Firewalls: General Techniques
 Service control - services that can be accessed inbound or
outbound
 Direction control
 User control - typically applied to users behind a firewall
 Behaviour control - how services are used – e.g., filter
emails 

## Application Layer Firewall
 examines the application
 needs proxy software for each application accessed
 allows access to only specified applications
 client application – e.g., Web browser
 server application
 creates two connections – one on each side
 enables individual user authentication
 Can be passive or active
 Active – inspects incoming requests
 Passive – works like an IDS

## Packet Filtering Firewalls
 Policy rules are enforced through the use of packet
inspection filters
 filters examine the packet headers
 filtering based on:-
     Source addresses - easily forged - limited benefit
     Destination addresses
     Protocol - use TCP port numbers to filter packets, e.g.
    allow FTP but block Telnet
     Connection - network layer filtering [stateful
    inspection]


## Stateless packet filtering – More examples
Policy | Firewall Setting
- No outside Web access. | Drop all outgoing packets to any IP address going to port 80
- No incoming TCP connections, except those for the institution’s public Web server only. | Drop all incoming TCP SYN packets to any IP except 130.207.244 203 and port 80
- Prevent Web-radios from eating up the available bandwidth. |  Drop all incoming UDP packets - except DNS and router broadcasts.
- Prevent your network from being used for a Smurf DoS attack. |  Drop all ICMP packets going to a “broadcast” address (eg 130.207.255.255).
- Prevent your network from being tracerouted | Drop all outgoing ICMP TTL expired traffic


 Firewalls are a powerful tool for network security
 A well designed, configured and maintained firewall is
nearly impenetrable
 but skilled hackers will work around it
 exploit trust relationships
 weakest link security vulnerabilities
 go through the VPN or dial-up account
 need to know the first few steps an attacker will
perform to bypass your firewall


## Key limitations of Firewall:
 IP spoofing: router can’t know if data “really” comes from
claimed source
 Poorly trained administrators
 New services and protocols
 Lack of patching
 Never checking the logs
 Tradeoff: degree of communication with outside world vs
level of security
 Many highly protected sites still suffer from attacks.

## There are things Firewalls cannot do:-
 protect against attacks that bypass the firewall
 disgruntled employees
 insider threat
 transfer of a virus-infected program
 social engineering attacks
 Code Red, Nimda worm and Storm all penetrated
firewalls 


## Improving security
A web application firewall (WAF) is also a suitable technology, but placing it at location C would only protect from attacks via the organization's VPN, which should only be used by trusted users.
 A firewall may not have the ability to identify and stop cross-site scripting attacks,
 IDS systems only monitor and don't stop attacks.
 An IPS can scan traffic and stop both known and unknown attacks


