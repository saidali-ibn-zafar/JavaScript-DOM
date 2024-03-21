## textContent

- As it is clear we have `textContent` property and it means just a content (text content), consider these codes below:

```html
// ...
<body>
  <h2 id="title">Welcome to Programming!</h2>
</body>

<script type="text/javascript">
  let h2Title = document.getElementById("title");

  h2Title.textContent = "Programming is not easy...";
</script>
```

or

- We can use `innerHTML` as well, `<em></em>` makes the text italic.

```html
// ...
<body>
  <h2 id="title">Welcome to Programming!</h2>
</body>

<script type="text/javascript">
  let h2Title = document.getElementById("title");

  h2Title.innerHTML = "<em>Programming is not easy</em>";
</script>
```
