# Class List (classList)

- The `Element.classList` is a read-only property that returns a live DOMTokenList collection of the class attributes of the element. This can then be used to manipulate the class list.

  - Adding - `Element.classList.add("nameOfClass")`;

  - Removing - `Element.classList.remove("nameOfClass")`;

  - Replacing - `Element.classList.replaceWith("nameOfClass", "newNameOfClass")`

  - Checking if it exists - `Element.classList.contains("nameOfClass")`

```javascript
// ...

<style>
    .bold{
        font-weight: bold;
    }

    .red-bg {
        background-color: red;
    }

    .white-text {
        color: #fff;
    }

    .big-font {
        font-size:36px
    }

</style>

<body>

   <h2 id="title">Class List</h2>
   <p id="myPara">
        Yeah mate
   </p>
</body>

<script type="text/javascript">

    const myPara = document.getElementById("myPara");

    // Adding
    myPara.classList.add("bold", "big-font");

    // Removing
    myPara.classList.remove("bold");

    // Replacing
    myPara.classList.resplace("big-font", "red-bg");

    myPara.classList.toggle("red-bg"); // removes red-bg, because toggle works if there is that class it removes, otherwise it adds...

    myPara.classList.toggle("red-bg"); // in this case it adds.

    console.log(myPara.classList.contains("bold")); // false

    console.log(myPara.classList);

</script>

```
