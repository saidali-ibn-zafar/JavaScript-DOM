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

---

- Simple exercise for `nextElementSibling`:

```javascript

<!doctype html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>

  <style>
    body {
      margin: 0;
    }

    nav {
      position: fixed;
      z-index: 99;
      top: 0;
      left: 0;
      width: 100%;
      padding: 15px;
      font-weight: bold;
      background: red;
    }
  </style>

  <body>
    <nav>Navigation bar</nav>
    <h2 id="title">Node.cloneNode() - JavaScript DOM</h2>
    <ul id="myList">
      <li>Apples</li>
      <li>Bananas</li>
      <li>Oranges</li>
    </ul>

    <ul id="myList">
      <li>Apples</li>
      <li>Bananas</li>
      <li>Oranges</li>
    </ul>

    <ul id="myList">
      <li>Apples</li>
      <li>Bananas</li>
      <li>Oranges</li>
    </ul>

    <ul id="myList">
      <li>Apples</li>
      <li>Bananas</li>
      <li>Oranges</li>
    </ul>

    <ul id="myList">
      <li>Apples</li>
      <li>Bananas</li>
      <li>Oranges</li>
    </ul>

    <ul id="myList">
      <li>Apples</li>
      <li>Bananas</li>
      <li>Oranges</li>
    </ul>

    <script type="text/javascript">
      const nav = document.querySelector("nav");
      const belowNav = nav.nextElementSibling;

      belowNav.style.marginTop = nav.clientHeight + "px";
      //   console.log(nav.clientHeight);
    </script>
  </body>
</html>


```
