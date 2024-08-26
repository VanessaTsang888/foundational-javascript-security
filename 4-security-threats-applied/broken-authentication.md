# Broken Authentication Resources

According to the [OWASP Top 10 - 2021](https://owasp.org/Top10/) this is now called **_[A07:2021 – Identification and Authentication Failures](https://owasp.org/Top10/A07_2021-Identification_and_Authentication_Failures/)_**.

This type of attack is when a cyber criminal is able to access our application through our authentication mechanism, either from weak password policies or weak authentication system. With access to our application a cyber criminal can do a lot of damage. Therefore, we need to use proper tools to authenication our app well such as two-factor-authentication or platforms like AuthO. We need to take the time to go through the content of this web page.

Within the **_References_** section there are alot of great cheat sheets such as [Implement Digital Identity](https://top10proactive.owasp.org/v3/en/c6-digital-identity) and the [Authentication Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/Authentication_Cheat_Sheet.html)

## How to Prevent

1. Where possible, implement multi-factor authentication to prevent automated credential stuffing, brute force, and stolen credential reuse attacks.
2. Do not ship or deploy with any default credentials, particularly for admin users.
3. Implement weak password checks, such as testing new or changed passwords against the top 10,000 worst passwords list.
4. Align password length, complexity, and rotation policies with National Institute of Standards and Technology (NIST) 800-63b's guidelines in section 5.1.1 for Memorized Secrets or other modern, evidence-based password policies.
5. Ensure registration, credential recovery, and API pathways are hardened against account enumeration attacks by using the same messages for all outcomes.
6. Limit or increasingly delay failed login attempts, but be careful not to create a denial of service scenario. Log all failures and alert administrators when credential stuffing, brute force, or other attacks are detected.
7. Use a server-side, secure, built-in session manager that generates a new random session ID with high entropy after login. Session identifier should not be in the URL, be securely stored, and invalidated after logout, idle, and absolute timeouts.
