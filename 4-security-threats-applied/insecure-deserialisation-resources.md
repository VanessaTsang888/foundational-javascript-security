# Insecure Deserialisation Resources

[A8:2017-Insecure Deserialization](https://owasp.org/www-project-top-ten/2017/A8_2017-Insecure_Deserialization)
This is not currently within the OWASP Top 10: 2021.

## What?

Deserialization is the reverse of Serialization, taking data structured in some format, and rebuilding it into an object. Today, the most popular data format for serializing data is JSON. Before that, it was XML.

Unfortunately, the features of these native deserialization mechanisms can sometimes be repurposed for malicious effect when operating on untrusted data. Attacks against deserializers have been found to allow denial-of-service, access control, or remote code execution (RCE) attacks.

This type of attack is hard to exploit but when a cyber criminal succeeds, access to sensitive data can occur. Therefore, we need to consistanly test our APIs and validate our objects aren't tampered by cyber criminals. In my latest previous employment I used Postman API tool to test the GET and POST calls so that I can analyse the responses by comparing them to find issues and to workout which of the code I need to refactor to meet the new requirements. There are a number of ways to prevent attacks such as enforcing `strict` types i.e. use TypeScript.js and ensuring the code files are error free when deserialization (opposite of serialization) occurs.

## Solution

We should take the time to go through 'Is the Application Vulnerable?' and 'How to Prevent' which is within the above official docs. Also, read the cheatsheets so we don't miss opportunity enforce alerts and monitor deserialization.
