# Sensitive Data

Must have a plan to hide sensitive data or application dat is crucial. Take a look at all the data available in our application.
What are the areas that would be safe for public consumption and the ones that are private or could be exploited? In general all user data should be considered to be sensitive and hidden from the public eye and take a look at the data users generate, can it be public or not? Once we have a plan, we need to implement some of the strategies mentioned in the 'Broken Authentication' lecture such as proper [crypto hashing](), HTTPS protocols and the use of advanced tools like [JS Crambler](https://jscrambler.com/) | [NPM - install JS Crambler](https://www.npmjs.com/package/jscrambler) - scrambles our code and data so it isn't easy to reverse engineer.

## The Big Question

We need to ask ourselves: "What are the areas that would be safe for public consumption and the ones that are private or could be exploited?".

In general all user data should be considered to be sensitive and hidden from the public eye and take a look at the data users generate, can it be public or not? Once we have a plan, we need to implement some of the strategies mentioned in the 'Broken Authentication' lecture such as proper [crypto hashing](), HTTPS protocols and the use of advanced tools like [JS Crambler](https://www.npmjs.com/package/jscrambler).

We need a plan to fully secure the sensitive data in our application before building the app. Then apply the appropriate strategy including the following:

### Private data

bcrypt/crypto - Proper crypto hashing.

### Code and functions

[JS Crambler](jscrambler.com)
Works at a deeper level with our code logic and scrambles our code and data making it difficult for cyber criminals to reverse engineer our minify code and figure out what functions does what.

### [Unsecured HTTP](https://owasp.org/www-community/vulnerabilities/Insecure_Transport)

HTTPS (Hypertext Transfer Protocol Secure)uses port 443 by default - used for secure communication btween a web brwoser and a web server, encrypting the data transmitted over the internet.
