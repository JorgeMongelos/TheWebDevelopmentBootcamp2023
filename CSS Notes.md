# CSS Notes

## How to add css?
```HTML
<!--External-->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>External</title>
  <link rel="stylesheet" href="./style.css"/> <!--right here-->
</head>
<body>
  <h1>Style Me in Green</h1>
</body>
</html>

<!--Internal-->
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <title>Internal</title>
  <style> <!--right here-->       
    h1{
      color: red ;
    }
  </style>
</head>

<body>
<h1>Style Me in Red!</h1>
</body>

</html>

<!--Inline-->
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <title>Inline</title>
</head>

<body>
<h1 style="color: Blue;">Style Me in Blue!</h1> <!--right here-->
</body>

</html>
```
## CSS Selectors
```HTML
<!--HTML Portion-->
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <title>CSS Selectors</title>
  <link rel="stylesheet" href="./style.css" />
</head>

<body>
  <h1>CSS Selectors</h1>
  <h2>Applying CSS to Different Parts of HTML</h2>
  <!-- TODO 1: Set the CSS for all paragraph tags to "color: red" -->
  <p class="note">1. The element selector targets elements based on their HTML tag name.</p>

  <ol>
    <!-- TODO 2: Set the CSS for all elements with a class of "note" to "font-size: 20px" -->
    <li class="note" value="2">Class selectors target elements based on the value of the class attribute.</li>

    <!-- TODO 3: Set the CSS for the element with an id of "id-selector-demo" to "color: green" -->
    <li class="note" id="id-selector-demo" value="3">ID selectors target elements based on the value of the id
      attribute.</li>

    <!-- TODO 4: Set the CSS for the li elements that have the "value" attribute set to "4" to have "color: blue" -->
    <li class="note" value="4">Attribute selectors target elements based on their attributes and values.</li>

    <!-- TODO 5: Set all elements to have "text-align: center" -->
    <li class="note" value="5">The universal selector targets all elements.</li>
  </ol>
</body>

</html>
```
```CSS
/*CSS Portion*/
ol {
  margin-left: -40px;
  margin-top: -20px;
  list-style-position: inside;
}

/* Write your CSS below, don't change the rules above. */
p{
  color: red;
}

.note{
  font-size: 40px;
}

#id-selector-demo{
  color: green;
}

li[value="4"]{
  color: blue;
}

*{
  text-align: center;
}
```
## CSS Color Properties
+ [Docs - Named Colours](https://developer.mozilla.org/en-US/docs/Web/CSS/named-color)
+ [RGB Colour Sliders](https://www.csfieldguide.org.nz/en/interactives/rgb-mixer/)
```HTML
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <title>Colors</title>
  <style>
  /* Write your CSS code here. */
    /* 1. Make the background of the webpage "antiquewhite"
    2. Make the h1 "whitesmoke"
    3. Make the background of the h1 "darkseagreen"
    4. Make the h2 #FAF8F1
    5. Make the background of the h2 "#C58940" */
    body{ 
      background-color: antiquewhite; /* #1 */
    }
    h1{ 
      color: whitesmoke; /* #2 */
      background-color: darkseagreen; /* #3 */
    }
    h2{ 
      color:#FAF8F1; /* #4 */
      background-color: #C58940; /* #5 */
    }
  </style>
</head>

<body>
  <h1>Hello</h1>
  <h2>World</h2>
</body>

</html>
```
## CSS Font Properties
+ [Google Fonts: Caveat Regular 400](https://fonts.google.com/specimen/Caveat)
+ [Font Properties Documentation](https://developer.mozilla.org/en-US/docs/Web/CSS/font)
```CSS
/* Embedded CSS Portion */

  <style>
    html{
      font-size: 30px;
    }
    
    body {
      background-color: cornflowerblue;
      color: white;
      font-size: 18px;
    }

    /* Don't change the CSS above, add Your CSS below */
    #color{
      color: coral;
    }

    #fontSize{
      font-size: 2rem;
    }

    #fontWeight{
      font-size: 900;
    }

    #fontFamily{
      font-family: 'Caveat', cursive;
    }

    #textAlign{
      text-align: right;
    }

    
  </style>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Caveat&display=swap" rel="stylesheet">
```
```HTML
<!--HTML Portion-->

<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <title>CSS Properties</title>

</head>

<body>
  <h1>Important CSS Properties</h1>
  <p id="color">Color</p>
  <p id="fontSize">Font Size</p>
  <p id="fontWeight">Font Weight</p>
  <p id="fontFamily">Font Family</p>
  <p id="textAlign">Text Align</p>

  <!-- TODOs
  1. Change the color of <p>Color</p> to "coral" color.
  2. Change the font size of <p>Font Size</p> to 2X the size of the root font size.
  3. Change the font weight of <p>Font Weight</p> to 900.
  4. Change the font family of <p>Font Family</p> to the Google font Caveat with regular (400) font weight.
  Link: https://fonts.google.com/specimen/Caveat
  5. Change the <p>Text Align</p> to right align.
  6. Change the the root (html element) font size to 30px -->
</body>

</html>
```
## The Cascade - Specificity and Inheritance.

```HTML
<!-- HTML Portion-->

<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <title>CSS Cascade</title>
  <link rel="stylesheet" href="./style.css">
</head>

<body>
  <div id="outer-box" class="box">
    <div class="box">
      <p>Yellow Text</p>
      <div class="box inner-box">
        <p class="white-text">White Text</p>
      </div>
    </div>
    <div class="box">
      <p>Yellow Text</p>
      <div class="box inner-box">
        <p class="white-text">White Text</p>
      </div>
    </div>
  </div>
</body>

</html>

```
```CSS
/* CSS Portion  */

#outer-box{
  background-color: purple;
  padding: 10px;
}
.box {
  background-color: blue;
  padding: 10px;
}

.inner-box{
  background-color: red
}

p {
  color: yellow;
  margin: 0;
  padding: 0;
}

.white-text{
  color: white;
}
```
## Combining CSS Selectors.

```CSS
/* Write your code here: */
h1, h2{ /* Grouping example */
    color: blueviolet;
}

.box > p{ /* Parent-child inheritance example */
    color: firebrick;
}

.box li{ /* Descendant inheritance example */
    color: blue;
}

li.done{ /* Chaining example */
    color: seagreen;
}

ul p.done{ /* Combining Combiners example */
    font-size: 0.5rem;
}
```
```HTML
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <title>Combining CSS Selectors</title>
  <link rel="stylesheet" href="./style.css">
</head>

<!-- Don't change any of the HTML code! -->

<body>
  <h1>To Do List</h1>
  <h2>Monday</h2>
  <div class="box">
    <p class="done">Do these things today!</p>
    <ul class="list">
      <li>Wash Clothes</li>
      <li class="done">Read</li>
      <li class="done">Maths Questions</li>
    </ul>
  </div>

  <ul>
    <p class="done">Other items</p>
  </ul>
  <p>The best preparation for tomorrow is doing your best today.</p>

</body>

</html>
```
## CSS Positioning.

```CSS
.blue-box{
    position: relative;
    height: 300px;
    width: 500px;
    background-color: blue;
    margin-top: 200px;
    margin-left: 200px;
}

.red-circle{
    position: absolute;
    width: 200px;
    height: 200px;
    background-color: red;
    border-radius: 50%;
    z-index: 1;
    left: 250px;
    top: 150px;
}
```
```HTML
<!DOCTYPE html>
<html>

<head>
  <title>CSS Positioning Exercise</title>
  <link rel="stylesheet" href="./style.css">
</head>

<body>
  <div class="blue-box">
    <div class="red-circle">
    </div>
  </div>

</body>

</html>
```
## CSS Display.

```CSS
/* style.css */

p {
    color: white;
  }

  .red {
    display: inline-block;
    width: 200px;
    height: 200px;
    background-color: red;
  }

  .green {
    display: inline-block;
    width: 200px;
    height: 200px;
    background-color: green;
  }

  .blue {
    display: inline-block;
    width: 200px;
    height: 200px;
    background-color: blue;
  }
```
```CSS
/* style2.css */

p {
    color: white;
  }

  .red {
    display: block;
    width: 200px;
    height: 200px;
    background-color: red;
  }

  .green {
    display: block;
    width: 200px;
    height: 200px;
    background-color: green;
  }

  .blue {
    display: block;
    width: 200px;
    height: 200px;
    background-color: blue;
  }
```
```HTML
<!-- HTML Portion -->

<!DOCTYPE html>
<html>

<!-- 
  TODO
1. By changing only the display property of the CSS make all 3 squares line up horizontally like in goal1 image.
2. Change only the display property to make all 3 squares line up vertically like in goal2 image. 
-->

<head>
  <meta charset="UTF-8"/>
  <title>CSS Display Property Example</title>
      <link rel="stylesheet" href="./style.css">
  <!-- <link rel="stylesheet" href="./style2.css"> -->
</head>


<body>
  <h1>CSS Display Property</h1>
  <p class="red">Red Paragraph </p>
  <p class="green">Green Paragraph</p>
  <p class="blue">Blue Paragraph</p>
</body>

</html>
```
## CSS Float.

```CSS
div {
    display: inline-block;
    width: 40%;
  }
  img{
    float: left;
    padding: 10px;
  }

  p {
    font-size: 2em;
   
  }

  .cat {
    background-color: aquamarine;
    float: left;
  }

  .dog {
    background-color: coral;
    float: right;
  }

  footer {
    text-align: center;
    background-color: blueviolet;
    clear: both;
  }
```
```HTML
<!DOCTYPE html>
<html lang="en">

<!-- TODO
1. Make both paragraph elements wrap around the image.
2. Use Float to move the cat div to the left and the dog div to the right.
3. Use clear to make the footer go below both the cat and dog div. -->

<head>
  <meta charset="UTF-8">
  <title>CSS Float</title>
  <link rel="stylesheet" href="./style.css">
</head>

<body>
  <div class="cat">
    <h2>CatCSS</h2>

    <img src="cat.jpeg" alt="cat in a box" />
    <p class="first-paragraph">Nap all day cat dog hate mouse eat string barf pillow no baths hate everything but kitty
      poochy. Sleep on keyboard
      toy
      mouse squeak roll over. Mesmerizing birds. Poop on grasses licks paws destroy couch intently sniff hand. The dog
      smells
      bad gnaw.</p>
  </div>
  <div class="dog">
    <h2>DogCSS</h2>
    <img src="dog.jpeg" alt="dogs in a box" />
    <p class="second-paragraph">Heckin good boys and girls long woofer big ol wow very biscit long woofer heck what a
      nice
      floof, long doggo noodle
      horse vvv very taste wow. Very taste wow many pats aqua doggo he made many woofs pupperino, puggo doing me a
      frighten.</p>
  </div>

  <footer>Copyright. This is the footer</footer>
</body>

</html>
```
## CSS Media Query
+ [Media Query Docs](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_media_queries/Using_media_queries)

```CSS
body {
    background-color: aquamarine;
  }

  /*max-width: screen less than.
   *min-width: screen bigger than.
   */

   /* Mobile devices */
   @media (min-width: 319px) and (max-width: 480px) {
    body {
      background-color: lightsalmon;
    }
  }

  /* iPads and tablets */
  @media (min-width: 481px) and (max-width: 1200px) {
    body {
      background-color: powderblue;
    }
  }

  /* laptops */
  @media (min-width: 1201px) and (max-width: 1600px) {
    body {
      background-color: limegreen;
    }
  }

 /* Desktops */
    @media (min-width: 1601px) {
      body {
        background-color: seagreen;
      }
    }
  
```
```HTML
<!DOCTYPE html>
<html lang="en">

<!-- 
TODO: Change the background color for each device
[lightsalmon] Mobile Devices: 319px — 480px
[powderblue] iPads and Tablets: 481px — 1200px
[limegreen] Laptops: 1201px — 1600px
[seagreen] Desktops: 1601px and more
-->

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1, minimum-scale=1" />
  <title>Media Query</title>
  <link rel="stylesheet" href="./style.css">
</head>

<body>
</body>

</html>
```
## Placeholder

```CSS

```
```HTML

```





## Placeholder

```CSS

```
```HTML

```