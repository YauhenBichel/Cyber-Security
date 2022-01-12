Denial of Service (DoS) Attacks

- Requires very little skill
- cost businesses millions of dollars every year
- costs relate to
    - Downtime = lost revenue
    - labour involved in identifying and reacting
- motivation
    - personal or political vendettas
    - may need to crash a system
- easier to disrupt operation than to gain access

## How does this work?
- Volumetric - overloading the target system’s resources
(disk space, bandwidth, buffers etc)
- Making network devices crash (router or switch)
- Overwhelming a DNS server - it runs out of memory and is
unable to service requests from users
- TCP State-Exhaustion Attacks: overwhelm the connection
state tables (load-balancers, firewalls, application servers)
- Application Layer Attacks – HTTP flood - using GET and
POST requests

## SYN Flood
• original DoS attack – still popular
• single source attack
• Example of a TCP State-Exhaustion Attack
• attacking system sends a large number of TCP
SYN packets to the “victim”
• starts the three-way handshake
• connection is never completed
• target’s buffer will be overwhelmed
• legitimate users are blocked 

### Defences
• difficult to identify
• install network devices capable of identifying SYN
flood attacks
• e.g., network-based intrusion detection system
• many commercial firewalls can reduce the effects
of SYN floods
• stack tweaking – reducing timeout
• use netstat to view sockets (SYN_RECV state)

## Ping of Death
• simplest and most primitive DoS attack
• aim – to overload the target
• problem - design of the TCP/IP protocol stack
• oversized packet is sent to the target
• maximum size IP packet is 65,535 bytes
• too large for many networks to handle
• Yahoo – only allows very small pings
• ICMP flood (ping flood) – uses ping or traceroute

## Fragmentation attacks
- exploit the breakdown of datagrams in order to overwhelm
the target network
- UDP (Fraggle attack) and ICMP fragmentation attacks
- packets that are larger than the network’s MTU
- these packets are fake and can’t be reassembled
- TCP fragmentation attacks (a.k.a. Teardrop)
- prevents TCP/IP from putting back together fragmented data
packets
- data packets overlap and overwhelm the victim’s servers
- OS older vers vulnerability – fixed with patches
- but - resurfaced in Win 7 and Vista
- needed repatching in Win 10

 DoS attacks have been around for a long time;
 Still using TCP/IP protocols for the attack;
 Known about for many years;
 Often originating from Botnets;
 Still very effective;
 They can be devastating to Web sites

