 Network security
 Passwords
 Firewalls
 IDSs and IPSs
 …


## Confidentiality
Confidentiality: protects data content; only sender and intended receiver should “understand” message contents
- sender encrypts message
- receiver decrypts message

## Integrity
Integrity: sender and receiver want to ensure message not altered (in transit, or afterwards) without detection

## Authentication
Authentication: sender and receiver want to confirm identity of each other

## Access and availability
Access and availability: services must be accessible and available to users

## First line of defence – IDs and Passwords
 Weakest link
 front line defence against intruders ID provides security in the following ways:-
 determines if a user is authorised
 determines the user’s privileges
 discretionary access control e.g. a user may grant permission to read their files

Two main threats
 Attacker gains access – brute force attack
 Worse - grab the password file

## Encrypting user password
Encrypt passwords using one-way techniques – digest
 digest algorithms (also cryptographic hash functions) are
public
 Need to make it difficult for a hacker to brute force
passwords
 Use a Salt
 creates stronger password but you need to store this
 defend against a pre-computed hash attack, e.g., rainbow
tables
 Salt reuse – not good
 Short salt – attacker can try every combination of the salt
 Randomise the Salt – add it to the password before hashing






