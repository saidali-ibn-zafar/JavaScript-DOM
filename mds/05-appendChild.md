## textContent

- In this time we are working on `appendChild()` and there we had `ul` with a list item of APPLE. After that we are creating an element with using `createElement()` property. Finally we are appending as child of `myList`...

```html
// ...
<body>
  <ul id="myList">
    <li>Apple</li>
  </ul>
</body>

<script type="text/javascript">
  // Parent Element:
  const myList = document.getElementById("myList");

  // New List Item
  const newListItem = document.createElement("li");

  newListItem.textContent = "Banana";

  myList.appendChild(newListItem);
</script>
```

---

- Creating and appending element with using `for of` loop:

```html
// ...
<body>
  <ul id="myList">
    <li>Apple</li>
  </ul>
</body>

<script type="text/javascript">
  // Parent Element:
  const myList = document.getElementById("myList");
  const fruitList = ["Orange", "Banana", "Mango", "Lemon"];

  for (const fruit of fruitList) {
    let newListItem = document.createElement("li");
    newListItem.textContent = fruit;

    myList.appendChild(newListItem);
  }
</script>
```
