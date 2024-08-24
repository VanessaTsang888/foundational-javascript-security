# Broken Authentication

Where a black hat hacker is able to see or exploit user info such as username and password. Applications with poor Authentication practices, they are putting their application and users at **risk\*** and potential legal liabilities.

If our code provides clear text representation of our user's password wither publicly or when a user is logged in we are a victim of our own bad authentication practices.

## Examples of Broken Authentications:

1. Text passwords: bcrypt/crypto libraries:

If our code don't **_hash_** the password through the use of bcrypt/crypto or similar libraries we are exposing our user passwords for anyone to exploit.

2. Session IDs in browser: session libraries:

A session ID provides info about the user logged into the app. A hacker could use this Session ID to access user or application data. Use proper session libraries for this purpose.

3. Unsecured HTTP: HTTPS:

We should be using HTTPS protocols and user is connected to your site through an insecured network like a public wifi then a hacker can grab the session IDs and get any information from them and we could be providing access to users to areas they're not supposed to. Having a strong plan as to who should have access to which area is crucial.

4. Overall auth: Auth0:

### JavaScript Crypto Libraries

For JavaScript, evaluate libraries like Forge, crypto-js (discontinued), and elliptic based on your specific use case and requirements.

Creating roles within our app and providing the proper access rights to these roles should be in our planning when creating our app and authentication practices.

### Summary

Therefore use proper libraries to connect our users securly to our site or leverage Auth0 to help us to secure our authentication workflow.
