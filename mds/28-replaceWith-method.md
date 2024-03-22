# replaceWith()

- The `replaceWith()` method in JavaScript is used to replace one element with another. It replaces the specified element `(oldElement)` with the element(s) provided as argument(s) `(newNode)`.

- Syntax:

```javascript
oldElement.replaceWith(newNode);
```

```html
<!DOCTYPE html>
<head>
  <title>Document</title>
</head>

<body>
  <h1>replaceWith() - JS DOM</h1>

  <div id="example">
    <p>Sample Text</p>
  </div>

  <script>
    const pTag = document.querySelector("#example p");

    const newInput = document.createElement("input");
    newInput.value = "I am new!";

    const newBtn = document.createElement("button");
    newBtn.textContent = "Me too";

    // pTag.replaceWith(newInput, newBtn, "I am some text");

    const newStrong = document.createElement("strong");
    newStrong.textContent = "I am new and strong";
    pTag.childNodes[0].replaceWith(newStrong, "I am some text");
  </script>
</body>
```
