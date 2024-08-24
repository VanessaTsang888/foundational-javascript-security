# XML External Entities

One of the top 10 issues on OWASP for a good reason. This attack occurs when an EXML document or code file is malformed and could be exploited for 'denial of services attacks'. This is what a malformed XML document looks like and to detect one you have most editors will be able to detect them. But if it dosen't or one was added to your web application, this is what you need to be looking for:

1. Non-closed element.
2. Non-existing attributes.
3. Bad XML.

```xml
<!-- xml syntax: -->
<one>
  <two>
  </one>
 </two>
<nonClosedElement nonExistingAttribute="test">
```

In this senario the attacker exploits the XML malformed doc that takes a bit more time to process due to its structure and then leverage this bad XML doc to render the resource processing unit useless. Therefore, denying its users of the resource which is 'denial of service' or DoS Attack. If we are using XML documents, ensure we are using proper syntax as we could be subjecting our users to not only slower performance but also opening up an opportunity for a hacker attack our system with a DoS Attack.

## XML on the Attack

1. Exploits malformed document (code files).
2. Causing CPU (central processing unit) into over-drive.
3. Denial-of-service (DoS) attack.
