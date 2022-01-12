Digital Signature : definition
• A message digest encrypted with the originator’s private key is called a DIGITAL SIGNATURE

Does digital signature meet 4 legal requirements?
1. uniquely linked to the signatory
YES- the signer encrypts with their PRIVATE key which uniquely
links to them
2. capable of identifying the signatory
YES – the signer can be identified as the owner of the PUBLIC key
that goes with that PRIVATE key (see later: digital certificates)
3. created by means that signatory has under control
YES- the signer is in control of their own PRIVATE key – well,
nobody else should have it!!
4. linked to the data such that data alterations are revealed
YES – the digital signature is the message digest encrypted with the
signer’s PRIVATE key – the message digest technology detects
alterations, that’s what it is for.
