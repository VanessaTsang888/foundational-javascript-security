# Security Miscnfiguration Resources

The URL to the official docs is [A05:2021 – Security Misconfiguration](https://owasp.org/Top10/A05_2021-Security_Misconfiguration/).

## What?

This security vulnerability is when the developer don't take the time out to properly secure our application or leave breadcrumbs of our security access all over the code.

I am using the exercise files downloaded from the training course.
There Error or Bug is on line 15 of the News.js file. The API key for a News API that shouldn't be in this PROD (production) environment as this is a security vulnerability:

```jsx
const url = `https://newsapi.org/v2/top-headlines?country=us&category=entertainment&apiKey=bbd2af39b78f42c7ba70a93d1eca2565`;
```

### Environment Config Files

Environment Config files shouldn't be committed to repo whether the repo is privat or public, it is still an issue as a cyber criminal can use the elements inside of these files to give unauthorised access to our data. Pay attention on Headers used in our clients. Use the Cheat sheets from the above doc to prevent these attacks.
