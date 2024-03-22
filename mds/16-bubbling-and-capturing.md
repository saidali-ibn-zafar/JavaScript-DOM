# Bubbling and Capturing in JavaScript

- Bubbling means start from bottom up to the top.

- Capturing means start from top and then sort of like capture the bottom elements.

```html
<!doctype html>
  <head>
    <title>Document</title>
  </head>

  <body>


    <h2 id="title">Bubbling and capturing - JS DOM</h2>

    <p id="parent">
      Lorem <strong id="child">ipsum</strong> dolor sit amet, consectetur
      adipisicing elit. Adipisci, impedit, et sed odit quisquam porro vero quo
      quaerat reiciendis nisi asperiores, numquam corporis. Nam laborum adipisci
      nemo eum. Et, vitae.
    </p>

<!-- Bubbling:  -->
    <script type="text/javascript">
      const parent = document.getElementById("parent");
      const child = document.getElementById("child");

      parent.addEventListener("click", function () {
        console.log("I am the PARENT");
      });

      child.addEventListener("click", function () {
        console.log("I am the CHILD");
      });

      //   this is bubbling because we go child up to parent. It means when we click child it works for child first and then for parent as well
    </script>
  </body>
</html>
```

---

- Capturing:

```javascript
const parent = document.getElementById("parent");
const child = document.getElementById("child");

parent.addEventListener(
  "click",
  function () {
    console.log("I am the PARENT");
  },
  true
);

child.addEventListener("click", function () {
  console.log("I am the CHILD");
});
```
