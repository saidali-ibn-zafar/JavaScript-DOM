# HTMLElement: dataset property

- The dataset read-only property of the HTMLElement interface provides read/write access to custom data attributes `(data-*)` on elements. It exposes a map of strings `(DOMStringMap)` with an entry for each `data-*`attribute.

```html
// ...

<body>
  <h2 id="title">Dataset</h2>
  <div id="myDiv" data-name="Ali" data-started-coding-at="18">Sample Text</div>
</body>

<script type="text/javascript">
  const myDiv = document.getElementById("myDiv");

  myDiv.dataset.name = "Saidali";
  myDiv.dataset.startedCodingAt = "16";

  myDiv.dataset.name = "";
  myDiv.dataset.removeAttribute("data-name");

  console.log(myDiv.dataset);
</script>
```
