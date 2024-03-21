# document fragment

- The DocumentFragment interface represents a minimal document object that has no parent.

```html
// ...
<body>
  <ul id="myList">
    <li>Apple</li>
  </ul>
</body>

<script type="text/javascript">
  const myList = document.getElementById("myList");
  const docFrag = document.createDocumentFragment();

  let item1 = document.creteElement("li");
  let item2 = document.createElement("li");

  item1.textContent = "Apple";
  item2.textContent = "Banana";

  docFrag.appendChild(item1);
  docFrag.appendChild(item2);

  console.log(docFrag);

  myList.appendChild(docFrag);
  // after appendChild docFrag we cannot expand docFrag, because we moved it ...
</script>
```

- If we log the `docFrag` into console then we would have:

![alt text](/src/image2.png)
