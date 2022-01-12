Cryptography, (or encryption) is the process of encoding a message or information in such a way that only authorized parties can access it and those who are not authorized cannot. Encryption does not itself prevent interference, but denies the intelligible content to a would-be interceptor.

Steganography is the technique of hiding secret data within an ordinary, non-secret, file or message in order to avoid detection; the secret data is then extracted at its destination.

Hashing is generating a value or values from a string of text using a mathematical function. Hashing enables alterations to a message to be detected.

## CONFIDENTIALITY
CONFIDENTIALITY: keeping messages CONFIDENTIAL 

## NON-ALTERATION
NON-ALTERATION: preventing unauthorised ALTERATIONS to messages 

## NON-REPLAYS
NON-REPLAYS: preventing REPLAYS of the same message 

## CONTROLLED ACCESS
CONTROLLED ACCESS: controlling unauthorised ACCESS to messaging systems 

## TEXT ciphers
TEXT ciphers (e.g. Caesar, Enigma, Vigenere etc)
Which mix up characters  of the message itself

## BINARY Symmetric ciphers
BINARY Symmetric ciphers (e.g. DES, AES, Triple-DES)
Which mix up binary (0’s and 1’s) of the message
And use SAME key for encryption and decryption

## BINARY Asymmetric ciphers
BINARY Asymmetric ciphers (e.g. RSA, Merkle-Hellman (Knapsack))
Which mix up binary (0’s and 1’s) of the message
And use DIFFERENT keys for encryption and decryption

## Ciphers
- SUBSTITUTION: substituting one character for another e.g. substitute B for A, C for B … 
- TRANSPOSITION: changing the position of a character e.g. 
    - ABCDEF becomes DEFABC 
    - or 01001101 becomes 11010100  
- BLOCKING : breaking the message into blocks and treating each block differently. Blocks can then be sent by sender through different routes and re-ordered on arrival at receiver. Also, this allows each block to be treated with a different key

SIMPLE SUBSTITUTION: Usually a character is replaced with another character.  Very famous: Caesar Cipher after Julius Caesar. 
Here a character in plain-text is encrypted using a character further forward in the alphabet eg. the word CAESAR is encrypted as ECGUCT. Normally, one alphabet is placed above another and then pushed for ward a certain number of places (the key) – the end of the top alphabet is wrapped round to fill up the front of the alphabet (this is called a ‘rotate’).


## DES
DES : Data Encryption Standard:SUBSTITUTION + TRANSPOSITION + BLOCKING

## DES Algorithm
DES contains elements of : 
- Substitution with XOR
- Transposition with changing position of bits in key each time round
- Blocking with 28bit blocks and then shuffling  blocks and treating differently each time round
But DES now easily cracked and replaced with Triple-DES which also crackable but still in use on some mobile phones.

- What is the word CAESAR with a key of 3? FDHVDU
- How many different kinds of cipher can we generate  using just the UpperCase English alphabet? 25 yes but not 26 because that would include a cipher where letters not changed
- 



