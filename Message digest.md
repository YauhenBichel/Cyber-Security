Message Digest: definition

• Such a method is the ‘Message Digest’ (a type of Hash – if
you don’t know this thing, don’t worry- explained later)
• Two common methods are:
• MD5 (message digest 5), SHA1 (Secure Hash Algorithm 1)
• But beware: these have been compromised and have now
been replaced with MD6 and SHA2 or SHA256

A message digest is usually a 128bit number (but nowadays 256 bits are being used) derived from a message contents and is unique to that message such that any alteration to the message would be noticeable from the digest.

Using A Digest To Detect Alterations
• CALCULATE DIGEST FOR MESSAGE TO SEND: Sender calculates message digest for message to be sent.
• SEND: Sender sends message + digest.
• CALCULATE DIGEST OF MESSAGE RECEIVED : Recipient applies same message digest algorithm to received message to calculate message digest.
• COMPARE DIGESTS: Original message digest and the received message digest should be the same. If not, then the message or the digest (or both) have, in some way, been altered/corrupted/tampered with. 

Message Digest: a simple 4bit digest
|---------D----------------|------------A-------------|
0 1 0 0 0 10 0 0 1 0 0 0 0 0 1
4bit start hash (seed) 1000
Block 1 0100
XOR 1100
Rotate(1 to left) 1001
Block2 0100
XOR 1101
Rotate(1 to left) 1011
Block 3 0100
XOR 1111
Roate(1 to left) 1111
Block 4 0001
XOR 1110
Rotate(1 to left) 1101
26
Most message digest algorithms use
RXOR – Rotate plus XOR (in this
algorithm here RXOR means XOR then
rotate 1 place to left (NOTE that different
algorithms have different types of
RXOR)).
Most algorithms create 128bit hash but
here we just use a 4bit hash (easier!).
Seeds can be any binary sequence not
just 1000 as shown. 


