# Security Misconfiguration

Security Misconfigurations normally occurs when there is a lack of proper settings in our application or exposed info from the server side and they happen typically when a developer publishes the development version of the server. This could open all kinds of settings for cyber criminals to exploit and also hinder the perforance of our application. It is also happens when someone leaves the debugging on or even worse `console.log()` sensitive data in the client side. We should test our app in the UI often. Sometimes its easy to mannipuate the data with a few scripts in the console but be wary of this issue. Another one is 'users default username and password'. Example, admin login with an admin password. This happens on many sites from templates. Always use complex passwords. We can use a Password Manager for this. Also wide open folders and code access restrictions and access controls. Every section of our app should have roles and access controls to match those roles so the right data is shown to the right people.

## Common Errors

1. Development version used for production.
2. Debugging is on.
3. Default credentials.
4. Improper access controls.

In general, when setting up our server variables, which usually have some credentials for our hosts, always use files that are protected and not published to the host and NEVER commit those files to your repo. The DVLA Driver Lookup web app is a good example as that includes these measures to help keep the app safe.

✅ Always use proted files.

❌ Never commit those files with sever variables to your repos.
