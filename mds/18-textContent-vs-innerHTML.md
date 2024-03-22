# textContent vs innerHTML

- As we can see on the codes below, there we are using `textContent` and `innerHTML` but they result is not the same. e.g: with `innerHTML` we can use HTML tags, etc related to HTML but not with `textContent`. `textContent` just sets the content into the given value... I hope you got me. If not run the code to see the results...

```html
<!doctype html>
  <head>
    <title>Document</title>
  </head>

  <body>


    <h1 id="title">textContent vs innerHTML - JS DOM</h1>
    <div id="my-div"></div>

    <script>
      const myDiv = document.getElementById("my-div");

      myDiv.innerHTML = "Hey my name is <strong>Saidali</strong>";
      myDiv.textContent = "Hey my name is <strong>Saidali</strong>";
    </script>

  </body>
</html>
```
