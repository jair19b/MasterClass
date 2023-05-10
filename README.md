## CODIGO DE EJEMPLO

# HTML

```shell
<!DOCTYPE html>
<html lang="en">
   <head>
      <meta charset="UTF-8" />
      <meta http-equiv="X-UA-Compatible" content="IE=edge" />
      <meta name="viewport" content="width=device-width, initial-scale=1.0" />
      <title>My First Web Page</title>
      <link rel="stylesheet" href="css/main.css" />
   </head>
   <body class="center">
      <div class="card">
         <h1>Hi English Class</h1>

         <p class="texto-centrado">
            This is an example of how using HTML and CSS you can create the structure and presentation of a web page. Now we are going to see a
            test with JS to give dynamism to the page
         </p>

         <button type="button" id="boton">Take Away the Design</button>
      </div>
      <script src="js/main.js"></script>
   </body>
</html>

```

# CSS

```
*,
*::after,
*::before {
   padding: 0;
   margin: 0;
   box-sizing: border-box;
   font-family: Verdana, Geneva, Tahoma, sans-serif;
}

body {
   background-image: url("https://images6.alphacoders.com/373/373654.jpg");
   background-repeat: no-repeat;
   background-position: center;
   background-size: cover;
}

h1 {
   margin-bottom: 2rem;
}

p {
   text-align: justify;
   margin-bottom: 1rem;
}

button {
   display: inline-block;
   padding: 1rem 2.75rem;
   width: 100%;
   text-align: center;
   font-weight: bold;
   color: #fff;
   background-color: #d8419e;
   outline: none;
   border-radius: 0.25rem;
   border: 1px solid transparent;
   cursor: pointer;
   transition: all 0.3s ease-in-out;
}

button:hover {
   background-color: #b12d7e;
}

.center {
   display: flex;
   justify-content: center;
   align-items: center;
   width: 100%;
   height: 100vh;
   color: #000;
}

.card {
   width: 40%;
   border-radius: 1rem;
   background-color: #fff;
   text-align: center;
   padding: 2rem;
}

```

# JS

```
const boton = document.getElementById("boton");
let beautiful = true;

boton.addEventListener("click", () => {
   const styles = "css/main.css";
   if (beautiful) {
      document.getElementsByTagName("link")[0].href = "";
      boton.textContent = "Give me the styles";
      beautiful = false;
   } else {
      document.getElementsByTagName("link")[0].href = styles;
      boton.textContent = "Take Away the Desing";
      beautiful = true;
   }
});

```
