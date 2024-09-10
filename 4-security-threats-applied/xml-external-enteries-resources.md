# XML External Enteries Resources

Now known as [XML External Entity (XXE) Processing](<https://owasp.org/www-community/vulnerabilities/XML_External_Entity_(XXE)_Processing>) on the OWASP Top 10: 2021.

A way to exploit our XML code to extract data or execute malicious code. Therefore, if we have any XML-based web services, this document is a must read. The best way to prevent attacks is to use the [SAST Tool](https://owasp.org/www-community/Source_Code_Analysis_Tools). Use this tool to scan for any XXE in our code and resolve the issues ASAP.

## Description

An XML External Entity attack is a type of attack against an application that parses XML input. This attack occurs when XML input containing a reference to an external entity is processed by a weakly configured XML parser. This attack may lead to the disclosure of confidential data, denial of service, server side request forgery, port scanning from the perspective of the machine where the parser is located, and other system impacts.

### XML External Entity Prevention Cheat Sheet

The safest way to prevent XXE is always to disable DTDs (External Entities) completely. Depending on the parser, the method should be similar to the following:

```xml
factory.setFeature("http://apache.org/xml/features/disallow-doctype-decl", true);
```

Disabling DTDs also makes the parser secure against denial of services (DOS) attacks such as Billion Laughs. If it is not possible to disable DTDs completely, then external entities and external document type declarations must be disabled in the way that's specific to each parser.
