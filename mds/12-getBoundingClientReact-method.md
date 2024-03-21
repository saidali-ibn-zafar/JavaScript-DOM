# Element.getBouningClientRect()

- Just consider the codes below because it is kinda easy to understand...

```html
<!doctype html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>

  <style>
    .box {
      width: 100px;
      height: 100px;
      background-color: #009879;
      border: 2px solid black;
    }
  </style>

  <body>
    <h2 id="title">Element.getBouningClientRect() - JS DOM</h2>
    <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Vero adipisci
      dicta at libero molestias commodi iste. Sit vitae harum eius quos nulla
      quae ex id impedit. Adipisci magnam veniam delectus? Consectetur libero,
      est perspiciatis aperiam totam consequuntur praesentium eum deserunt ipsum
      ipsa voluptatibus molestias saepe! Dignissimos minima sunt rerum commodi
      nihil fugiat iure expedita, cupiditate accusantium error ea praesentium
      laboriosam. Dolor id ea debitis dolore laborum dolorum non dicta earum
      animi nemo quia, quis cum inventore magni suscipit! Minima illo modi rerum
      pariatur beatae nisi voluptatem praesentium non, optio fuga. Iure dolor
      velit quia in commodi hic distinctio nesciunt vero provident cum autem
      adipisci aspernatur fugiat ullam neque nobis doloremque iste aperiam quis
      illum porro, aliquam iusto optio? Maiores, quos. Reiciendis, commodi modi
      et quos aut officia error eveniet temporibus inventore corporis ipsa
      doloribus voluptatibus ad eos aliquid voluptatum! Distinctio adipisci
      ullam aperiam sequi ea praesentium obcaecati accusantium consectetur
      cumque. Labore nulla ad corrupti sequi, quibusdam soluta? Fuga, atque
      culpa eaque in numquam aliquid excepturi quisquam, ut cum est repellat
      iusto necessitatibus, cupiditate asperiores odit nam expedita molestias
      pariatur recusandae! Fuga voluptatem, exercitationem explicabo recusandae,
      magni praesentium necessitatibus voluptas iusto est distinctio animi.
      Neque tempore, harum iusto, tempora omnis atque, ullam error alias itaque
      beatae recusandae quos deleniti ratione autem. Quo ut tempore voluptate
      distinctio eligendi eaque ad explicabo ex labore unde, amet aperiam, fuga
    </p>
    <div class="box"></div>

    <script type="text/javascript">
      const box = document.querySelector("div.box");

      window.addEventListener("scroll", function () {
        // console.log(window.innerHeight);
        // console.log(box.getBoundingClientRect().top);

        if (box.getBoundingClientRect().top < window.innerHeight) {
          box.style.backgroundColor = "red";
        }
      });
    </script>
  </body>
</html>
```
