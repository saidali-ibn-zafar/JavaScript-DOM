# insertAdjacentHTML() method

```html
<!DOCTYPE html>
  <head>
    <title>Document</title>
  </head>
  <body>
    <h1>Element.insertAdjacentHTML() - JavaScript DOM</h1>

    <p id="myPara">I will write some <em>text</em></p>

    <script>

      // beforebegin - before element
      // afterbegin - first child
      // beforeend - list child
      // afterend - after element

      const myPara = document.getElementById("myPara");

      myPara.insertAdjacentHTML("beforebegin", "<strong>ALI</strong>")
      myPara.insertAdjacentHTML("afterbegin", "<strong>ALI</strong>")
      myPara.insertAdjacentHTML("beforeend", "<strong>ALI</strong>")
      myPara.insertAdjacentHTML("afterend", "<strong>ALI</strong>")
    </script>
  </body>
</html>
```
