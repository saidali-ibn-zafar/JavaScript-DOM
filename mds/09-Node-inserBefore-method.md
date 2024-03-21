# Node: insertBefore() method

- In this example, we are talking about `Node: insertBefore() method`. Briefly, we that method helps us to insert where we want... In these codes below there is `myList.insertBefore(orangesItem, pearsItem);` and it is inserting oranges before pears. After that we created `function` that works with `insertBefore` method. Consider the following example to understand more about `insertBefore` method.

```html
// ...
<body>
  <h2 id="title">Node.insertBefore() - JavaScript DOM</h2>
  <ul id="myList">
    <li>Apples</li>
    <li id="pearsItem">Pears</li>
    <li>Bananas</li>
  </ul>

  <script type="text/javascript">
    const myList = document.getElementById("myList");
    const pearsItem = document.getElementById("pearsItem");

    const orangesItem = document.createElement("li");
    orangesItem.textContent = "Oranges";

    //   myList.insertBefore(orangesItem, pearsItem);

    //   Opposite to appendChild
    function addToBeginning(parent, toInsert) {
      const firstChild = parent.firstChild;
      parent.insertBefore(toInsert, firstChild);
    }

    addToBeginning(myList, orangesItem);
  </script>
</body>
```
