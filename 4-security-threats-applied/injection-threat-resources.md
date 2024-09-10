# Injection Threats Resources

[OWASP Top 10 - 2021](https://owasp.org/Top10/) - stay up-to-date with the Top 10 **_security vulnerabilities_** to be aware how issues appear in our applications and how we can prevent them. The most important **_security risks or threats_** are the Top 10 on this page. The order of these threats can change as the world wide web is a moving object and is constantly developing.

## [A03:2021 – Injection](https://owasp.org/Top10/A03_2021-Injection/)

The way cyber criminals leverage this security threat is when data or queries are NOT properly secured, validated, filtered or sanitised by the application. This is the job of the Business Logic Tier also known as the Backend. Then the criminals can leverage these openings to inject code/hostile data to corrupt or delete or pull data from our app. To prevent from this threat is to keep the data **_separate_** from the commands and queries. The DVLA Driver Lookup project that I worked on during my last employment do just this. This page contain multiple solutions in how to prevent Injection Threats.

### Use positive server-side input validation

1. Implement input validation on the server-side, as client-side validation can be easily bypassed by an attacker. This ensures that input validation code cannot be circumvented.

2. Validate input data against a set of predefined rules or patterns, which can include:

- Regular expressions for more complex patterns
- String matching for simpler patterns

3. Use a whitelist approach to validate email addresses, as described in the OWASP Cheat Sheet, by performing basic initial validation and then passing the address to the mail server to catch any exceptions.

### Example Attack Scenarios

We need to fully understand what Attack Scenarios look like this.

**_Scenario #1_**: An application uses untrusted data in the construction of the following vulnerable SQL call:

```sql
-- invalid sql syntax
String query = "SELECT \* FROM accounts WHERE custID='" + request.getParameter("id") + "'";

```

### References

This section contains cheat sheets we can use to prevent these attacks such as [Injection Prevention Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/Injection_Prevention_Cheat_Sheet.html)

Injection flaws occur when an application sends untrusted data to an interpreter. Injection flaws are very prevalent, particularly in legacy code, often found in SQL queries, LDAP queries, XPath queries, OS commands, program arguments, etc. Injection flaws are easy to discover when examining code, but more difficult via testing. Scanners and fuzzers can help attackers find them.
