Cross-Site Request Forgery (CSRF)

 A user submits a state change request
 Does not include anything secret
http://example.com/app/transferFunds?amount=1500&destinationAccou
nt=4673243243
 Hacker constructs a request that transfers money
<img src=
"http://example.com/app/transferFunds?amount=1500&destinationAc
count=attackersAcct#" width="0" height="0" />
 This is embedded in an image request or iframe stored on sites under
the control of the hacker
 The authenticated user visits the site
 Forged requests automatically includes the user’s session info,
authorising the attacker’s request

## Delivering secure transactions?
 Change to HTTPs and you are using port 443
 You are also using the secure protocol SSL/TLS
 Uses encryption to protect sensitive data
 Using an SSL certificate and a “SSL handshake” to start a
secure session
 Secure?
 SSL generally prevents man-in-the-middle (MITM) attacks
 Hardware Vendor Mishandles Private Keys
 National Security Agency discovered a “critical vulnerability”
in Windows 10 - impacts HTTPS connections

## Conclusion
 Attackers look for unpatched systems, poor
design, unsanitised input, end-user carelessness
 Some of the most common attacks
• DoS attacks
• Certificate and Configuration issues – low hanging
fruit
• Request forgery – capture a cookie
• Failure to re-authenticate – known for over 2 yrs
• Server can not prove that there is no man-in-themiddle (Zeus)