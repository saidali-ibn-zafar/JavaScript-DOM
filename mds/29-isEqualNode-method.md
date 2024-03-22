# isEqualNode() method

- The `isEqualNode()` method in JavaScript is used to determine whether two nodes are equal in terms of their type, attributes, and content. It returns `true` if the two nodes are identical, and `false` otherwise.

- Syntax:

```javascript
node.isEqualNode(otherNode);
```

```html
<!DOCTYPE html>
<head>
  <title>Document</title>
</head>

<body>
  <h1>isEqualNode() - JS DOM</h1>

  <div class="test">
    <strong>TEST 1</strong>
  </div>
  <div class="test">
    <strong>TEST 1</strong>
  </div>

  <script>
    const div1 = document.querySelectorAll("div")[0];
    const div2 = document.querySelectorAll("div")[1];

    const isEqual = div1.isEqualNode(div2);

    console.log(isEqual);
  </script>
</body>
```
