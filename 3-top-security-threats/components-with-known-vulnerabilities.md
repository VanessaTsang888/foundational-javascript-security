# Components with know vulnerabilities

When we are developing an app we often use packages that offer us extensibility and leverage other components from these libraries. This extra help is great but can sometimes lead us into an insecure path with our app. An example is using a navigation or routing library with our React app where we would be their components to build out our routing or navigating areas with their component. The best way to identify these issue is when we test with Snyk or [Retire.js](https://retirejs.github.io/retire.js/) - check out the [Retire JS GitHub](https://github.com/RetireJS/retire.js) for more info - Scans websites for vulnerabilites. This tool will give us a good idea of which packages or libraries are outdated and insecure.

I have installed Retire.js as an [browser extension](https://chromewebstore.google.com/detail/retirejs/moibopkbhjceeedibkbkbchbjnkadmom) and used it to scan my portfolio website and found that it is clean which is expected since I've built my own components and not installed any packages/libraries.

## To keep our website secure

1. Test with Snyk or Retire.js
2. Retire or replace bad components.
3. Write your own components.

Otherwise validate that we are using secure components in our applications.
When we find outdated packages then we need to figure out if it is not just a simple update of the package and the syntax used. If not, then plan to replace these packages or write our own components.
