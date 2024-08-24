# Top Security Threats

OWASP Top 10 Security Threats:

- SQL Injectins and JavaScript Injections is one of the most comon security issues in this category and is referred to as Cross Site Scripting attacks or XSS.
- This attack is when malicious code is executed inside of a user input and sends code that executes once the form is submitted.

[XSS in sandbox domains](https://bughunters.google.com/learn/invalid-reports/web-platform/xss/6619189462433792/xss-in-sandbox-domains):

When looking for xss issues use `alert(document.domain)` rather than `alert(1)` as our default XSS payload as the former script returns the domain where the XSS is injected. This allows us to verify if we are injecting script on a snadbox domain which is not considered to be a security vulnerability.

Self-XSS:
to test this in browser:

1. open up DevTools -> Console tab: here type `alert(document.domain)` and hit the Enter key on your keyboard.
2. Now you will see a pop-up with msg of 'brave://newtab says undefined'.
3. This don't have high impact.

XSS Impact:

For an account take-over the payload would have to be much longer.

1. Elements tab, right-click to edit HTML element to add additional html.
2. Example, edit the url within `href` attribute to `"javascript:alert(document.domain")`.
3. This will trigger a pop-up msg on browser.
4. This is a lot of social engineering to get the victim to modify the code.

Self XSS Method 2 - Response Modification:

Similar to the DevTools edit the html once of the option is to use Response Manipulation in a proxy such as [Burp](https://portswigger.net/burp/documentation/desktop/getting-started). This can be in security testing such as third party authentication.

Many framework such as React.js and Angular has been to escape the bad code and it submits the input as a string.

## A basic example

The website that the instructor is using to test script no longer exists and the script examples don't work on Chrome browser.

In browser -> search input type this code `<u>test<u>` and hit Enter key or the Search btn on the right of input. The result returned is not as shown in the lecture as this lecture is outdated.

Now insert a script instead `<script>alert('hello')</script>`.
