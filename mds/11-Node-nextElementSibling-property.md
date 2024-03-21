# Element: nextElementSibling property

- `nextElementSibling` property gives us the next sibling element as it is clear but not node...

```javascript
// ...
<body>
  <h2 id="title">Element: nextElementSibling property - JavaScript DOM</h2>

  <ul id="myList">
    <li>Apples</li>
    Fruits
    <li>Bananas</li>
    <li>Oranges</li>
  </ul>

  <script type="text/javascript">
    const applesItem = document.querySelector("#myList > li:first-of-type");
    const bananasItem = applesItem.nextElementSibling; // <li>Bananas</li>
    const fruits = applesItem.nextSibling; // Fruits
  </script>
</body>
```
