# querySelector method

- The Document method `querySelector()` returns the `first Element` within the document that `matches` the specified selector, or group of selectors. If no matches are found, `null` is returned.

```html
<!doctype html>
  <head>
    <title>Document</title>
  </head>

  <body>


    <h2 id="title">Element.querySelector - JS DOM</h2>



    <div class="box">Box 1</div>
    <div class="box">Box 2</div>
    <div class="box">Box 3</div>


    <script type="text/javascript">
        // const result = document.querySelector("#title");
        const result = document.querySelector(".box"); // we get Box 1


    </script>
  </body>
</html>
```

or

```html
<!doctype html>
  <head>
    <title>Document</title>
  </head>

  <body>


    <h2 id="title">Element.querySelector - JS DOM</h2>

    <div class="container1">
        <div class="box">Container 1 , Box 1</div>
    </div>


    <div class="container2">
        <div class="box">Container 2 , Box 2</div>
    </div>


    <script type="text/javascript">
        // const result = document.querySelector("#title");
        const result = document.querySelector(".box"); // we get Box 1

        const container2 = document.querySelector(".container2");

        const result = container2.querySelector(".box"); // and now we get Box 2

    </script>
  </body>
</html>
```
