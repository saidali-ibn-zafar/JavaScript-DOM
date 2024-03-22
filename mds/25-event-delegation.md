# Event Delegation

- Event delegation in JavaScript means listening for events on many items at once by putting one listener on their shared parent, making it easier to manage events, especially for items added later.

```html
<!DOCTYPE html>
<head>
  <title>Document</title>
</head>

<body>
  <h1>What is Event Delegation?</h1>

  <p>
    Lorem ipsum dolor sit amet, consectetur adipisicing elit. Reiciendis,
    quibusdam? Animi accusantium debitis harum itaque! Mollitia a quisquam ullam
    possimus reiciendis quibusdam atque sunt saepe natus. Repellat nam est
    adipisci.
  </p>

  <ul id="myList">
    <li>Apple</li>
    <li>Banana</li>
    <li>Tomato</li>
  </ul>

  <script>
    const myList = document.getElementById("myList");

    myList.addEventListener("click", function (e) {
      // console.log(e);
      const target = e.target;

      if (target.matches("li")) {
        // do something
        target.style.backgroundColor = "red";
      }
    });

    const newLi = document.createElement("li");
    newLi.textContent = "Orange";
    myList.appendChild(newLi);
  </script>
</body>
```
