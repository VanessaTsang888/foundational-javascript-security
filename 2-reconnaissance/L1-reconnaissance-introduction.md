# Lecture 1 - Reconnaissance Introduction

The goal of reconnaissance is to workut a set of common tools, if there are any issues or open doors for hackers to exploit and at this stage we valuate our code. The best way to do this is to do an `npm install` or `npm audit` - we'll explore this later. Start with `npm install`command.
Once installed, go through any msg console.log is telling us.

- I need to update Node and NPM to the latest version:
  Node is a runtime environment that allows developers to execute JavaScript code outside the browser, on the server-side.

## How to update Node

1. Use NPM to Update Your Node Version
   To update Node with NPM, you will install the n package, which will be used to interactively manage node versions on your device.

Clear the NPM cache:
install dependencies, some modules are cached to improve the speed of installation in subsequent downloads. So first, you want to clear the NPM cache.

Install n
`npm install -g n`.

Install this package globally as it manages the Node versions at the root.
Install a new verion of Node:
`n lts`
`n latest`
