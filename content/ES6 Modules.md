---
draft: true
tags:
  - note
---
# Modules in JavaScript
Consider a simple web application in HTML, Javascript, and CSS. For example, let's say we're making a little grocery list app.

There are a few ways you might implement this app.
## Multiple Script Tags
- Multiple Files
- Maybe even some third party libraries like JQuery. 
- There were issues with this approach because it's separate HTTP requests for each file
	- Separate http requests greatly impacts the load time
	- If script2 depends on script1, but the HTTP for script2 finishes first, you get a bad load.
## Script Concatenation
- One solution is to concatenate them all.
- Back in the day, this would be done by hand
## Bundlers and Transpilers
- Software for doing this bundling automatically came about. 
- Enabled the potential for Transpiling, such as making Typescript
# CommonJS Modules
- The module.exports syntax that was used by node for a while.

# ES6 Modules
- Native support for modules finally came around in 2015.


> [!NOTE] Sources and References
> **ES6 Modules**
> https://www.sitepoint.com/understanding-es6-modules/
> **Bundlers**
> https://snipcart.com/blog/javascript-module-bundler