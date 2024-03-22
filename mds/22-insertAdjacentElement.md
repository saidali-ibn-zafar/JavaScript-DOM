# Element.insertAdjacentElement()

- The `insertAdjacentElement()` method in JavaScript is a useful function that allows you to insert an HTML element at a specified position relative to the element it is invoked upon. This method provides a way to directly manipulate the DOM and can be a powerful tool for dynamic content manipulation in web pages.

- 'beforebegin': Before the targetElement itself.

- 'afterbegin': Just inside the targetElement, before its first child.

- 'beforeend': Just inside the targetElement, after its last child.

- 'afterend': After the targetElement itself.

```html
<!DOCTYPE html>
  <head>
    <title>Document</title>
  </head>

  <style>

    #area{
      background-color: black;
      color: white;
      padding: 25px;
    }

    #box {
      background-color: red;
      padding: 25px;
      margin-bottom: 10px;
    }

  </style>

  <body>
    <h1>Element.insertAdjacentElement() - JavaScript DOM</h1>

    <div id="area">
      <h2>Put some text inside there</h2>
    </div>

    <script>

      const area = document.getElementById("area");
      const box = document.createElement("div");

      box.id = "box";

      // beforebegin - before element
      // afterbegin - first child
      // beforeend - list child
      // afterend - after element


      area.insertAdjacentElement("afterbegin", box);
    </script>
  </body>
</html>


```
