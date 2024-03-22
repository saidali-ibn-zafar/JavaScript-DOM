# append()

- The `append()` method in JavaScript is used to append one or more elements or text nodes to the end of a parent element.

```javascript
parentElement.append(node1, node2, ...);
```

```html
<!DOCTYPE html>
<head>
  <title>Document</title>
</head>

<body>
  <h1>append() - JS DOM</h1>

  <div id="myDiv"></div>

  <script>
    const myDiv = document.getElementById("myDiv");

    const strong = document.createElement("strong");
    const em = document.createElement("em");
    const myTextNode = document.createTextNode("Simple Text");

    strong.textContent = "Strong";
    em.textContent = "Emphasis";

    myDiv.append(strong, em, myTextNode, "some more text");
  </script>
</body>
```
