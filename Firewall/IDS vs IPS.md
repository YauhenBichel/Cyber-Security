IDS vs IPS

IDS
 Some latency involved when malicious packet is
detected
 Needs real time detection
 Works on preconfigured rules
 Advantage - little impact on the network
 Disadvantage – will not stop an attack
     May be vulnerable to a hacker circumventing detection
     May give high false positive readings


IPS
 Sits inline and all packets must pass through it
 Advantage – can detect an attack
 Disadvantage
     Can slow the network traffic (bottleneck)
     May drop legitimate packets
     Needs to be up to date to block the latest attacks

 Host Intrusion Prevention System (HIPS)
     Can analyse encrypted traffic
     Detects abuse of privileges
     Place on DMZ servers