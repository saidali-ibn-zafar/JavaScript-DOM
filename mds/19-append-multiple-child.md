# Append Multiple Child

-

```html
<!DOCTYPE html>
  <head>
    <title>Document</title>
  </head>
  <body>
    <ul id="my-list"></ul>

    <script>
      // Creates this: <li>[text]</li>
      function createListItem(text) {
        var li = document.createElement("li");
        li.textContent = text;
        return li;
      }

      function appendChildren(parent, children) {
        children.forEach(function (child) {
          parent.appendChild(child);
        });
      }

      var myList = document.getElementById("my-list");
      var items = [
        createListItem("Item 1"),
        createListItem("Item 2"),
        createListItem("Item 3"),
        createListItem("Item 4"),
        createListItem("Item 5"),
        createListItem("Item 6"),
      ];

      //   appendChildren(myList, items);

      //   or

      items.forEach(function (item) {
        myList.appendChild(item);
      });
    </script>
  </body>
</html>

```
