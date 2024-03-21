## Element.setAttribute();

- In the codes below, we have input and it has "sample" as a value. And then using setAttribute() we are changing it into "modified sample"

```html
// ...
<body>
    <input type="text" id="myInput" value="sample"></input>
</body>

<script type="text/javascript">

    document.getElementById("myInput").setAttribute("value", "modified sample");

</script>
```

---

- We have learned `document.createElement`, so we will try to use it in the below example:

```html
// ...
<body></body>

<script type="text/javascript">
  const myElement = document.createElement("div");

  myElement.setAttribute("class", "container");
</script>
```

- As a result, we will have `<div class="container"></div>`

- And then we can append it as chilt of body:

```javascript
// ...
document.body.appendChild(myElement);
// ...
```
