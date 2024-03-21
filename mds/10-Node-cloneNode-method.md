# Node: cloneNode() method

- cloneNode method helps us to clone or copy the node, and it takes only one argument:

  - e.g: `bananasItem.cloneNode()` - in this case it just copies `<li></li>` without text.

  - e.g: `bananasItem.cloneNode(true)` - in that case, it copies deeply, which means with children. So we would have `<li>Bananas</li>`.

```html
// ...
<body>
  <h2 id="title">Node.cloneNode() - JavaScript DOM</h2>
  <ul id="myList">
    <li>Apples</li>
    <li>Bananas</li>
    <li>Oranges</li>
  </ul>

  <script type="text/javascript">
    const myList = document.getElementById("myList");
    const listChildren = myList.children;
    const bananasItem = listChildren[1];
    const bananasCopy = bananasItem.cloneNode(true);
    myList.appendChild(bananasCopy);
  </script>
</body>
```
