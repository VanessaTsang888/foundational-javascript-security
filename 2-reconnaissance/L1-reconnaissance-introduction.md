# Lecture 1 - Reconnaissance Introduction

The goal of reconnaissance is to workout a set of common tools, if there are any issues or open doors for hackers to exploit and at this stage we valuate our code. The best way to do this is to do an `npm install` or `npm audit` - we'll explore this later. Start with `npm install`command.
Once installed, go through any msg console.log is telling us.

I have installed the node modules inside the Resources directory.

Act on any outdated dependancies immediately.
Make sure I have the latest dependancies.
To get more details on all the packages within the dependancies shown on package.json file run `npm audit`. Then fix myself mannual.
Use git versioning tool so I can go back in time in case I make an mistake.
Go through the report and decide what I need to do next.
Use the latest version of my own dependancies. From this i may need to update my syntax to the latest.

Linters are good to improve our writing style, clean our code but in most case they will not catch security issues. This is where Snyk, Retire.js andApp Sensor comes into play. Do some reconnaissance of our code and figure out any potential dangers/secrity threats.

## Vanessa's Notes

**_outdated dependancies_**
In my past commericial projects I have upgraded dependancies such as upgrading the Docusaurus framework from version 2.0.0 to version 2.4.0. This work was in regards to the Resolve Security Vulnabilities Issues ticket on the BAU board. To complete this ticket I had used [TortoiseGit](https://tortoisegit.org/) which is a Windows Shell Interface to Git

**_Linters - improve our writing style_**
In my commercial projects such as the Design System project I've used a Linter (to catch React.js syntax errors) by adding [Husky](https://www.npmjs.com/package/husky?activeTab=readme) the NPM package that makes it easy to add Git hooks (pre-commit hook) to our projects. I had installed Husky as a dependancy and that acts as a wrapper for ES Lint and Prettier. From my experience the Linter helped me ensure the way I write the React.js components is using the lastest syntax which I believe helps with my Defensive Programming work whcih is part of cyber security.
