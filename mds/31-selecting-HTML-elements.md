# Selecting Elements

- single element by ID : `getElementById()`

- single element by CSS selector : `querySelector()`

- multiple elements by CSS selector : `querySelectorAll()`

- multiple elements by class (live) : `getElementByClassName()`

- multiple elements by tag (live) : `getElementByTagName()`

---

`querySelector()` and `querySelectorAll()` are more versatile as they can select elements using CSS selectors, whereas `getElementById()`, `getElementsByClassName()`, and `getElementsByTagName()` are more limited in their selection capabilities.
`querySelector()` returns the first element matching the selector, while `querySelectorAll()` returns a NodeList containing all matching elements.
`getElementsByClassName()`and`getElementsByTagName()`return HTMLCollections, which are live collections that automatically update when the DOM changes.`querySelectorAll()`also returns a NodeList, but it is not live.
It's worth noting that while`getElementById()`and`querySelector()`return only one element (or null if no element matches),`querySelectorAll()`, `getElementsByClassName()`, and `getElementsByTagName()` return collections of elements, even if only one element matches the criteria.

or watch this to understand more :

[Selecting HTML elements](https://www.youtube.com/watch?v=qnWqecp4QsY&list=PLVvjrrRCBy2JS8__NYlhPeaoNz2p1aPEN&index=32)
