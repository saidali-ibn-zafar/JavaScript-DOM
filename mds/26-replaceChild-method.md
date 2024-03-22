# replaceChild method

- The `replaceChild()` method in JavaScript is used to replace one child node of a specified parent node with another node.

### syntax:

```javascript
parent.replaceChild(newChild, oldChild);
```

```html
<!DOCTYPE html>
<head>
  <title>Document</title>
</head>

<body>
  <h1>replaceChild() - JS DOM</h1>

  <ul id="myList">
    <li>HTML</li>
    <li>CSS</li>
    <li>JS</li>
  </ul>

  <script>
    const myList = document.getElementById("myList");
    const cssListItem = myList.children[1];

    const newListItem = document.createElement("li");
    newListItem.textContent = "jQuery";

    myList.replaceChild(newListItem, cssListItem);
  </script>
</body>
```
