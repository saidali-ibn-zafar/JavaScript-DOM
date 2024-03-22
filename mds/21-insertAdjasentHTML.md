# insertAdjacentHTML() method

```html
<!DOCTYPE html>
  <head>
    <title>Document</title>
  </head>
  <body>
    <h1>Element.insertAdjacentHTML() - JavaScript DOM</h1>

    <p id="myPara">I will write some <em>text</em></p>

    <script>

      // beforebegin - before element
      // afterbegin - first child
      // beforeend - list child
      // afterend - after element

      const myPara = document.getElementById("myPara");

      myPara.insertAdjacentHTML("beforebegin", "<strong>ALI</strong>")
      myPara.insertAdjacentHTML("afterbegin", "<strong>ALI</strong>")
      myPara.insertAdjacentHTML("beforeend", "<strong>ALI</strong>")
      myPara.insertAdjacentHTML("afterend", "<strong>ALI</strong>")
    </script>
  </body>
</html>
```

- beforebegin:

![image](https://github.com/saidali-ibn-zafar/JavaScript-DOM/assets/120341849/ab10cd7d-6aa0-4a11-a109-ececba9c3474)

---

- afterbegin:

![image](https://github.com/saidali-ibn-zafar/JavaScript-DOM/assets/120341849/d8255dea-1c20-4f5c-910d-734c4420e627)

---

- beforeend:

![image](https://github.com/saidali-ibn-zafar/JavaScript-DOM/assets/120341849/24657d04-513a-4531-861c-02ff11abc8d6)

---

afterend:

![image](https://github.com/saidali-ibn-zafar/JavaScript-DOM/assets/120341849/58e1d959-161b-48eb-8b4d-fe101bb335d0)
