# elementFromPoint() method in JavaScript

- The `elementFromPoint()` method in JavaScript is used to retrieve the topmost element at the specified coordinates relative to the viewport. It returns the element located at the specified coordinates, or `null` if no element is found at that position.

- syntax:

```javascript
document.elementFromPoint(x, y);
```

```html
<!DOCTYPE html>
<html>
  <head>
    <title>elementFromPoint Example</title>
    <style>
      #container {
        width: 300px;
        height: 200px;
        background-color: lightblue;
        position: relative;
      }
      #target {
        width: 100px;
        height: 100px;
        background-color: pink;
        position: absolute;
        left: 50px;
        top: 50px;
      }
    </style>
  </head>
  <body>
    <div id="container">
      <div id="target"></div>
    </div>

    <script>
      document.addEventListener("click", function (event) {
        var element = document.elementFromPoint(event.clientX, event.clientY);
        if (element) {
          console.log("Element at clicked position:", element);
        } else {
          console.log("No element found at clicked position.");
        }
      });
    </script>
  </body>
</html>
```
