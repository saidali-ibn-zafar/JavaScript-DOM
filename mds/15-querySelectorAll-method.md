# querySelectorAll method

- `querySelector` is used to select a `single element` from the DOM tree, while document. `querySelectorAll` is used to select `multiple elements` from the DOM tree.

```html
<!doctype html>
  <head>
    <title>Document</title>
  </head>

  <body>


    <h2 id="title">Element.querySelectorAll - JS DOM</h2>

    <div class="box">Box 1</div>
    <div class="box">Box 2</div>
    <div class="box">Box 3</div>


    <script type="text/javascript">
        const boxes = document.querySelectorAll(".box")

        boxes.forEach((e) => {
            e.style.color = "red";
        });
    </script>
  </body>
</html>
```
