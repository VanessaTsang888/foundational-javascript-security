# Sensitive Data Exposure Resources

This is now [A02:2021-Cryptographic Failures](https://owasp.org/Top10/A02_2021-Cryptographic_Failures/).

## A02:2021 - Cryptographic Failures

Shifts up one position to #2 on the list of the 'Top 10 cybersecurity threats'. Previously known as 'A3:2017-Sensitive Data Exposure', which was broad symptom rather than a root cause. The renewed name focuses on failures related to cryptography (or lack thereof) as it has been implicitly before. This category often leads to sensitive data exposure or system compromise. Notable Common Weakness Enumerations (CWEs) included are CWE-259: Use of Hard-coded Password, CWE-327: Broken or Risky Crypto Algorithm, and CWE-331 Insufficient Entropy.

Most of the dangers around data is whilst in transit between the client side (user interface/Frontend) and the serverside (backend) and how encrypted the data is. Cyber criminals whom are able to access our private user data can do what they want with it and we need to ensure our application isn't vulnable to these attacks. Using strict transport security protocols like HSTS (strict transport security) and proper encryption.
