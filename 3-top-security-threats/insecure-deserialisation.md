# Insecure Deserialisation

Notes from Vanessa:
Business logic tier (backend) do the Data Serialisation process before it can pass the verified data to the persistance tier (DB).
Therefore we need to implement securtiy on the backend.

In short, deserialisation is the transformation of data coming from a file or the network, typically from a JSON or XML format into an object that our app can read: the backend. So Serialisation is the opposit to this where the object is serialised into a readable JSON format: the frontend. Most frameworks have methods that do this automatically for us.

## Serialisation

Obeject is serialised into a readable JSON format on the UI tier.
<br /> Object -> JSON/XML.

## Deserialisation

The transformation of data coming from a file or the network.
<br /> JON or XML -> Object.

So **_Insecure Deserialisation_** is when cyber criminals exploit on trusted data to render the app resources 'useless' such as a Denial of Service Attack (DoS Attack) or even execute code (scripts payload) inside of our app. To remedy this there are several ways and packages that exist as long as we DON'T use the JS Method `eval()`. To find solutions do a search on NPM and look for the most updated and active packages.

### Summary

1. Cyber criminals exploit JSON or XML deserialisation.
2. Don't use serialise packages with `eval()` method as they execute arbitrary code which can lead to security vulnerabilities if not properly sanitised. It's crucial to ensure that the serialised data is trusted and validated to prevent code injection attacks.
3. Find many packages on 'npm' Node Package Manager.
