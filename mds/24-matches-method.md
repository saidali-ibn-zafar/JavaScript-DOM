# Element.matches - JS DOM

- In this example, we are exploring how to use the `element.matches()` method to determine whether a specific DOM element adheres to a set of CSS selector criteria. By evaluating both cases where an element does and does not match given selectors, we highlight the method's versatility in guiding conditional logic within JavaScript applications.

```html
<!DOCTYPE html>
<head>
  <title>Document</title>
</head>

<body>
  <h1>Element.matches - JavaScript DOM</h1>

  <p id="myPara" data-name="ali">
    Lorem ipsum dolor sit amet, consectetur adipisicing elit. Reiciendis,
    quibusdam? Animi accusantium debitis harum itaque! Mollitia a quisquam ullam
    possimus reiciendis quibusdam atque sunt saepe natus. Repellat nam est
    adipisci.
  </p>

  <script>
    const myPara = document.getElementById("myPara");

    const result = myPara.matches("#myPara");
    console.log(result); // true because it has id of myPara

    const result2 = myPara.matches("[data-names]");
    console.log(result2); // false because it has data-name but not data-names
  </script>
</body>
```
