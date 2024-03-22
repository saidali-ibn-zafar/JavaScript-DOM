# Element.insertAdjacentText() - JavaScript DOM

- It also works like the same as `insertAdjacentHTML()` and `insertAdjacentElement()` but it is for `text`. If you have not seen `insertAdjacentHTML()` and `insertAdjacentElement()` just take a look at them first...

```html
<!DOCTYPE html>
<head>
  <title>Document</title>
</head>

<body>
  <h1>Element.insertAdjacentText() - JavaScript DOM</h1>

  <p id="myPara">
    Lorem ipsum dolor sit amet, consectetur adipisicing elit. Reiciendis,
    quibusdam? Animi accusantium debitis harum itaque! Mollitia a quisquam ullam
    possimus reiciendis quibusdam atque sunt saepe natus. Repellat nam est
    adipisci.
  </p>

  <script>
    // beforebegin - before element
    // afterbegin - first child
    // beforeend - list child
    // afterend - after element

    const myPara = document.getElementById("myPara");
    myPara.insertAdjacentText("beforebegin", "Hello ");
  </script>
</body>
```
