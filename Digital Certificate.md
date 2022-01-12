## Establishing Who Owns The Public Key
What is needed is a system for establishing the TRUE identity of
the owner of a public key. 

DIGITAL CERTIFICATE
  
In above situations we are not certain of the actual identity of the sender, only that the sender has a particular public key.
To purchase from a company over the web you would want to know that the company is who they say they are and that the  public key they send you really belongs to them. 
Authenticity of  a public key can be proved by a digital certificate. 
This gives the public key of a named party and verifies ownership. 

## WHY USE HEX? 
It is easier for humans to write and check. It is a form of shorthand with each Hex character representing the binary integer value of a 4 bit binary string except for integer values ten to fifteen which are shown as alphabetic characters. From now on we use Hex more often.

The digital certificate is to verify the owner of a PUBLIC key.
 Most certificates in the world are created to the X509 standard template. A typical certificate shows the following:
 ID: Certificate number – all certificates have an ID (in Hex)
OWNER: name and other details of PUBLIC key owner.
KEY: actual PUBLIC key that is being verified (in Hex)
PERIOD: validity period of the certificate.
TYPE: certificate type –usually three types.
CA: Certificating authority that issued the certificate to the owner.
CHECK DATE: when the certificate details were checked by the CA
ALGORITHM: the message digest algorithm that was used.
SIGNATURE: digital signature (in Hex) for whole certificate i.e the message digest for all the above details (using algorithm shown on certificate) encrypted with the CA’s PRIVATE key. The CA (who issued the certificate) are signing to say it is true and trustworthy.

DIGITAL CERTIFICATE 	Serial No: A2:EO:89:B1:E5 

Certified Details for : Sue Smith	 

Email: ss02@yahoo.com      
URL: http://www.cms.gre.ac.uk	
Public Key:9D:4F:16:3D:1A:87:F1:A2:EO:7D:B9:B1:D5:83:B3:62

Certificate Validity: 4/1/2022 – 3/1/2023 	
Certificate Type: Validated Persona Class 1 	
Checked: 20/12/2021

Certificating Authority: Verisign Class 1 CA: 62 Axford Street
Message Digest Type: MD6

Digital Signature for this Certificate: BD:44:15:3D:2A:57:F1:72:EO:…

## Q and A

Certificate above has digital signature at Part B.
Q: What is this signature composed of ? 
Answer: message digest of details in Part A encrypted with CA(PRIVATE key)
Q: Who encrypted the signature? 
Answer: the CA who created it (Verisgn Class 1 CA)
Q: How do we verify that certificate details have not been altered?
Answer: 
Calculate the message digest for Part A of the certificate
Decrypt signature with CA (PUBLIC key) to get original message digest
Compare the two digests: 
If digests DIFFERENT then certificate has been altered in some way and cannot be trusted

## Certificating Authority (CA): Classes of certificate 
Many Certificate Authorities (CA’s) e.g. Verisign, Thawte. 
Some do exhaustive checks - others do few eg Verisign: 

Verisign Class1: 
Personal certificate – usually individuals, first and last names, email

Verisign Class2 : 
Individual subscriber – persona validated:
 name, spouses name, email, dob ,employer, drivers lic. no., soc. sec. no.

Verisign Class 3: 
Secure Server: thorough identity checks

Q: But where does Joe get the C.A’s Public Key?

ANSWER
From the C.A’s Digital certificate !
Yes, the CA have their own certificate showing their PUBLIC key.
But how can Joe be sure the CA certficate is, He must do te same thing and check out the digital signature on this i.e decrypting the digital signature and checking the message digest.

Q: But who creates the digital signature for the C.A’s certificate?

ANSWER
The ROOT – and you have to get their PUBLIC Key by a very safe method probably by post, or personal visit to their offices.


# Hierarchy of Trust: Certificate Chaining
ROOT CA -> ROOT CA issues certificates to verify Public Keys of intermediate CA’s
e.g. Verisign ROOT 


Intermediate CA -> Intermediate CA issues certificates to verify public keys of Users.
e.g. Verisign Class 1 CA


End-users -> Users send certificate to anyone wanting to send them secret messages.
e.g. Sue, Joe, Fred, BP, etc


