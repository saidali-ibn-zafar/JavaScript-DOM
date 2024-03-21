## document.createElement

In the codes below, we will talk about creating an element (in this case "div" as an example). And then appending it as a child of body.

```html
// ...
<body>
  // ...
</body>

<script type="text/javascript">
  let newElement = document.createElement("div");

  document.body.appentChild(newElement);
</script>
```
