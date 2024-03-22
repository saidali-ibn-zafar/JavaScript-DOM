# window.parent property

- WORKING ON `window.parent` property

- index.html:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Main HTML Page</title>
  </head>
  <body>
    <h1 id="heading">This is the main HTML page!</h1>
    <iframe
      src="content.html"
      frameborder="1"
      style="width: 600px; height: 300px"
    ></iframe>
  </body>
</html>
```

---

- content.html:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Embedded HTML</title>
  </head>
  <body>
    <p id="para">
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Quod aliquid id
      cumque magnam, iure officiis numquam ea consequatur vero quisquam soluta
      facere sequi doloribus suscipit natus commodi. Laborum ratione
      voluptatibus maiores. Omnis exercitationem enim officiis amet officia
      placeat dolorem a?
    </p>

    <script>
      //   console.log(window.parent);

      const parentDocument = window.parent.document;
      const parentHeading = parentDocument.getElementById("heading");

      //   console.log(parentHeading);

      const para = document.getElementById("para");

      para.textContent = para.textContent + parentHeading.textContent;
    </script>
  </body>
</html>
```
