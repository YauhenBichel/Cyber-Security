Symmetric Encryption: attributes

- Speed Very fast
- Secure Yes – if key is long. The longer thebetter – at least 128bits.
- Easy to distribute the key? No – how do you get a secret key to the receiving party?
Ok for banks and the military who are closed organisations but for ecommerce between strangers over the net – very difficult.

For Ecommerce we need Three Technologies
• To obtain a workable encryption method for internet/ecommerce/ebanking that enables anyone to send a confidential message , protected from alteration, protected from replay, and protected from impostors then we need 3 technologies:
• Symmetric encryption (same key for sender/receiver)
• Asymmetric encryption (different keys for sender/receiver)
• Message Digest (hash)

Which we can combine to make digital signatures, digital certificates and nonces

## Symmetric encryption
Symmetric encryption : one-key

## Asymmetric encryption
Asymmetric encryption: two-keys

A solution to symmetric key problems is asymmetric encryption
accredited to Diffie & Hellman and refined by Rivest, Shamir &
Adelman (RSA) in USA and to Clifford Cocks in UK. Clifford
worked for British secret service and was not permitted to go
public.

## The most common asymmetric system used in the world is RSA

The two keys are named:
• PRIVATE key (kept secret)
• PUBLIC key (distributed to others, anybody, anywhere)

The two keys are mathematically related such that:
Fundamentals of RSA Asymmetric Encryption
1. A message can be encrypted with either key but can only be
decrypted with the other key,
2. No key can be determined from knowledge of the other
3. The two keys are unique; no other key pairs are similar.


RSA (Rivest, Shamir and Adelman) Algorithm based on prime Numbers : C=M^e mod n
1. Select two prime numbers e.g. p=7, q=17
2. Calculate n: p*q = 7*17 = 119
3. Calculate (p-1)*(q-1) = 6*16 = 96
4. Choose e: prime number < 96 not a factor of 96 e.g. 5
5. Calculate d such that (d*e) mod 96 has remainder 1and d<96: so d=77
6. So, the two keys are public {5,119} and private {77,119}

ENCRYPT
PLAINTEXT : 00010011 Reading 00010011 as integer it is decimal 19
TO ENCRYPT using C=M^e mod n and key 5,199: 195
/119 = 20807 remainder 66 so
ciphertext is 66 

DECRYPT
using C=M^e mod n and key 77,199: 6677 /119 =1.06*10138 remainder 19 so result is
Integer 19 in binary is 00010011 which was original plaintext

Asymmetric Encryption
• The two keys are named:
• PRIVATE key (kept secret)
• PUBLIC key (available to others, anybody, anywhere and openly)

• The PRIVATE KEY must always be kept a secret by its owner. BUT
the corresponding PUBLIC KEY can be given to anybody.

• NB: It would take ENORMOUS computing power to derive the
private key from knowing the public key because the prime
numbers involved are so large, so difficult to find, and require so
much computing power to ensure they are prime that criminals
rarely have such resources available. Even governments can be
hard put to do this

## Comparison: Symmetric v Asymmetric
Criteria 
- Speed
    - Symmetric: Fast – mainly done in hardware XOR is built-in processor function
    - Asymmetric: Slow – mainly done in software - 100times slower than symmetric

- Key Distribution 
    - Symmetric: Difficult –how to keep key secret
    - Asymmetric: Easy –just send public key so easy to send to strangers

- Secure 
    - Symmetric: Yes – if key is long, at least 128bits
    - Asymmetric: Yes – big primes a good safeguard



