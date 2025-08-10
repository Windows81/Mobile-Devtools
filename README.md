# Mobile DevTools

A mobile browser extension for debugging web apps. Based on the libre project [Eruda](https://eruda.liriliri.io/), Mobile DevTools allows you to view the console, DOM elements, network traffic, page source, resources, and more.

Click the extension's icon in the toolbar or menu to open the overlay.

- Console: View JavaScript logs, errors, warnings, and other debug info. Execute arbitrary JS to interact with the webpage.
- Elements: Drill down into the DOM tree to see attributes, inline styles, CSS rules, and computed styles.
- Network: Record in detail the network requests being made and inspect the responses.
- Resource: Show local storage, session storage, cookies, scripts, stylesheets, iframes, and image assets.
- Sources: Source code viewer for HTML, JS, and CSS.
- Info: View the current URL, User Agent, and device details.
- Snippets: Execute useful JavaScript snippets. If you're a developer and would like to add additional plugins, please visit Eruda's documentation at https://github.com/liriliri/eruda.

_Mobile DevTools may not work on all websites, depending on the page content's security policies._

## How to Build

```sh
curl https://cdn.jsdelivr.net/npm/eruda --output ./src/eruda.min.js
npm install -g crx
crx pack -p key.pem ./src mobile-devtools.crx
```
