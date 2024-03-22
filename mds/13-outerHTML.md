# outerHTML

- The outerHTML property sets or returns the HTML element, including attributes, start tag, and end tag.

```html
<!doctype html>
  <head>
    <title>Document</title>
  </head>

  <style>
    div{
        padding: 20px;
        font-weight: bold;
        color: white;
        background-color: red;

    }
  </style>

  <body>

    <h2 id="title">Element.outerHTML - JS DOM</h2>

    <script type="text/javascript">
        const h2Title = document.getElementById('title');

        console.log(h2Title.outerHTML);

        h2Title.innerHTML = "<div> I have been changedElement.outerHTML - JS DOM</div>"
    </script>
  </body>
</html>
```
