# The Web Development Bootcamp2023 
## Dr. Angela Yu

### Notes 

| Internet Components        | Website Components |
| -------------------------  | ------------------ |
| + Servers                  | + HTML             |
| + Client                   | + CSS              |
| + ISP                      | + JS               |
| + DNS                      |                    |
| + IP address - nslookup.io |                    |

### Heading Elements 

```HTML
<h1>Book</h1>
  <h2>Chapter 1</h2>
    <h3>Section 1</h3>
    <h3>Section 2</h3>
  <h2>Chapter 2</h2>
       <h4>Diagram 1</h4>
  <h2>Chapter 3<h4>
    <h3>Section 1</h3>
    <h3>Section 2</h3>
```

## Paragraph Element

```HTML
<p>Third paragraph. Nisl purus in mollis nunc sed id semper risus. Ipsum a arcu cursus vitae congue mauris rhoncus aenean. Ridiculus mus
mauris vitae ultricies leo integer malesuada nunc. In tellus integer feugiat scelerisque. Lectus mauris ultrices eros in
cursus turpis massa. Sollicitudin ac orci phasellus egestas. Massa massa ultricies mi quis hendrerit dolor. Quam
elementum pulvinar etiam non quam lacus suspendisse faucibus interdum. Iaculis nunc sed augue lacus viverra. Id ornare
arcu odio ut sem nulla pharetra. Amet luctus venenatis lectus magna fringilla urna porttitor. Eu nisl nunc mi ipsum
faucibus vitae aliquet nec ullamcorper. Nunc mattis enim ut tellus elementum sagittis. Mauris augue neque gravida in
fermentum et sollicitudin. Pellentesque habitant morbi tristique senectus. Tristique senectus et netus et. Turpis
egestas sed tempus urna et pharetra pharetra. Feugiat vivamus at augue eget arcu dictum varius duis at. Lacus sed
viverra tellus in hac habitasse platea dictumst vestibulum. Nisl condimentum id venenatis a condimentum vitae sapien.</p>
```

## Void Elements
```HTML
<h1>William Blake</h1> 
<p>
17 south molton street<br/>
London<br/>
W1K 5QT<br/>
UK<br/>
</p> 

<hr/>
```
## List Elements
```HTML
<h1>Angela's Cinnamon Roll Recipe</h1>

<h2>Ingredients</h2>

<h3>For the dough:</h3>
<ul> 
    <li> cup warm milk</li>
    <li>2 ¼ teaspoons yeast</li>
    <li>¼ cup granulated sugar</li>
    <li>1 egg plus 1 egg yolk</li>
    <li>¼ cup butter</li>
    <li>3 cups bread flour</li>
</ul>

<h3>For the filling:</h3>
<ul>
    <li>2/3 cup dark brown sugar</li> 
    <li>1 ½ tablespoons ground cinnamonn</li>
    <li>¼ cup butter</li>
</ul>

<h3>Instructions</h3>
<ol>
    <li>Mix the milk with the yeast, sugar, eggs.</li>
    <li>Melt the butter and add to the mixture.</li>
    <li>Add in the flour and mix until combined into a dough.</li>
    <li>Knead the dough for 10 minuites.</li>
    <li>Transfer the dough into a large bowl and cover with plastic wrap. Leave<br/>
        it somewhere to rise for 2 hours.</li>
    <li>After the dough has doubled in size, roll it out into a large rectangle.</li>
    <li>Melt the butter for the filling and mix in the sugar and cinnamon.</li>
    <li>Spread the filling onto the dough then roll the dough into a swiss roll.</li> 
    <li>Cut the roll into 3cm sections and place flat into a baking tray.</li>
    <li>Pre-heat the oven to 350F or 180C, then bake the rolls for 20-25min until lightly brown.</li>
</ol> 
```
## Nesting and Indentation.
```HTML
<ul>
    <li>A</li>
    <li>B
        <ol>
            <li>B1</li>
            <li>B2</li>
            <ul>
                <li>
                    B2a
                    <ul>
                        <li>B2aa</li>
                        <li>B2ab</li>
                    </ul> 
                </li>
                <li>B2b</li>
                <li>B2c</li>
            </ul>
        <li>B3
            <ol>
                <li>B31</li>
                <li>B32</li>
            </ol>
        </li>
        </ol>
    </li>
    <li>C</li>
</ul>
```
## Anchor Elements
```HTML
<h1>My top 5 Favourite Websites</h1>
<!-- Write your code below -->
<ol start="5">
    <li><a href="https://www.udemy.com/">Udemy</a></li>
    <li><a href="https://www.netflix.com/browse">Netflix</a></li>
    <li><a href="https://www.youtube.com/">YouTube</a></li>
    <li><a href="https://www.tiktok.com/explore">TikTok</a></li>
    <li><a href="https://www.facebook.com/">Facebook</a></li>
</ol>
```
## Image Elements
```HTML
<h1>I am a Cat Person</h1>
<!-- Kitten image URL -->
<img src="https://raw.githubusercontent.com/appbrewery/webdev/main/kitten.jpeg" alt="kitten image"/>

<h1>I am a dog Person </h1>
<!-- Puppy image URL -->
<img src="https://raw.githubusercontent.com/appbrewery/webdev/main/puppy.gif" alt="puppy image"/>
```

## Absolute Vs Relative File Paths
```HTML
<h1>All the Animals</h1>
<h2>Rabbit:</h2>
    <img src="./rabbit.png" alt="rabbit image"/>
<h2>Cat:</h2>
    <img src="./Folder3/cat.png" alt="cat image"/>
<h2>Dog:</h2>
    <img src="../dog.png" alt="dog image"/>
<h2>Fish:</h2>
    <img src="../Folder1/fish.png" alt="fish image"/>
<h2>Bird:</h2>
    <img src="../Folder1/Folder2/bird.png" alt="bird image"/>
```

## What are Web Pages?
```HTML
<h1>Welcome to My Website!</h1>
<!-- Add an image of yourself that links to the about page -->
    <a href="./public/about.html"><img src="./assets/images/cat.png" alt="cat image"/></a>
<hr />
<!-- Add a link to your contact me page here -->
<a href="./public/contact.html">Contact Me</a>
```

## The HTML Boilerplate
```HTML
<!DOCTYPE html>    
    <html lang="en">
        <head>
            <meta charset="UTF-8"/>
            <title>My Website!</title>
        </head>
        <body>
            <h1>Hello World!</h1>
        </body>
    </html>
```
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
## CSS Colours
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
## Project #1: Movie Ranking Project.
```HTML
<!-- Write your code below -->
<h1>The Best Movies According to Jorge</h1>
<h2>My top 3 movies of all time.</h2>
<hr/>
<h3>The Matrix</h3>
<p>It opens your mind towards how the current status quo works.</p>
<h3>Don't look up</h3>
<p>It depicts the perils we're headed to</p>
<h3>Leave the workd behind</h3>
<p>I consider it a wake up call</p>
```
## Project #2: Birthday Invite Project.
```HTML
<h1>It's My Birday!</h1>
<h2>On the 23rd of December</h2>

<img src="https://raw.githubusercontent.com/appbrewery/webdev/main/birthday-cake3.4.jpeg" alt="birthday-cake3"/>
<h3>What to bring:</h3>
<ul>
    <li>Baloons(I love baloons)</li>
    <li>Cake (I'm really good at eating)</li>
    <li>An appetite(There will be lots of food)</li>
</ul>

<h3>This is where you needd to go:</h3>
<a href="https://www.google.com/maps/@35.7040744,139.5577317,3a,75y,289.6h,87.01t,0.72r/data=!3m6!1e1!3m4!1sgT28ssf0BB2LxZ63JNcL1w!2e0!7i13312!8i6656">Google map link</a>

```
## Project 3: Angela Yu's Portfolio
```HTML
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8"/>
        <title>My Website</title>
    </head>
    <body>
        <h1>Angela Yu's Portfolio</h1>
        <h2>I'm a Web Developer</h2>
        <hr/>
        <h3><a href="./public/movie-ranking.html">Movie Ranking Project</a></h3>
            <img src="./assets/images/movie-ranking.png" height="200px"/>
        <h3><a href="./public/birthday-invite.html">Birthday Invite Project</a></h3>
            <img src="./assets/images/birthday-invite.png" height="200px"/>
        <hr/>
        <a href="./public/about.html">About Me</a>
        <a href="./public/contact.html">Contact Me</a>
    </body>
</html>
```
## Project #4: Colour Vocab Website
```HTML
<!--HTML Portion-->
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <title>Spanish Vocabulary</title>
  <link rel="stylesheet" href="./style.css" />
</head>

<body>
  <h1>Colors</h1>
  <h2>Learn the colors in Spanish!</h2>
  <h2 class="color-title" id="red">Rojo</h2>
  <img class="color" src="./assets/images/red.png" alt="red" />

  <h2 class="color-title" id="blue">Azul</h2>
  <img src="./assets/images/blue.png" alt="blue" />

  <h2 class="color-title" id="orange">Anaranjado</h2>
  <img src="./assets/images/orange.png" alt="orange" />

  <h2 class="color-title" id="green">Verde</h2>
  <img src="./assets/images/green.png" alt="green" />

  <h2 class="color-title" id="yellow">Amarillo</h2>
  <img src="./assets/images/yellow.png" alt="yellow" />
</body>

</html>
```
```CSS
/*CSS Portion*/
img{
    height: 200px;
    width: 200px;
}
.color-title{
    font-weight: normal;
}

#red{
    color:red;
}

#blue{
    color: blue;
}

#orange{
    color: orange;
}

#green{
    color: green;
}

#yellow{
    color: yellow;
}