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
```
## Project #5: Motivational Meme Project
```HTML
<!-- HTML Portion -->

<!-- 
  TODO: Create a motivational post website.
Style it how ever you like. 
Look at the goal image for inspiration.
But it must have the following features:
1. The main h1 text should be using the Regular Libre Baskerville Font from Google Fonts:
  https://fonts.google.com/specimen/Libre+Baskerville
2. The text should be white and background black.
3. Add your own image into the images folder inside assets. It should have a 5px white border.
4. The text should be center aligned.
5. Create a div to contain the h1, p and img elements. Adjust the margins so that the image and text are centered on the page. 
  Hint: You horizontally center a div by giving it a width of 50% and a margin-left of 25%.
  Hint: Set the image to have a width of 100% so it fills the div. 
6. Read about the text-transform property on MDN docs to make the h1 uppercase with CSS.
  https://developer.mozilla.org/en-US/docs/Web/CSS/text-transform 
-->
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8"/>
    <link rel="stylesheet" href="style.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Libre+Baskerville&display=swap" rel="stylesheet">
  </head>
  <body>
    <div>
      <img src="./assets/images/turn.png" alt="motivational quote">
      <h1>Show love</h1>
      <p>No matter how, no matter where.</p>
    </div>
  </body>
</html>
```
```CSS
/* CSS Portion */

html{
    background-color: black;
}

h1{
    color: white;
    text-transform: uppercase;
}

p{
    color: white;
}

img{

    height: 600px;
    width: 100%;
    border: 5px solid white;
}

div{
    margin-top: 5%;
    width: 50%;
    margin-left: 27%;
    text-align: center;
}
```
## Project #6: CSS Flag Project

```CSS
.flag{
    background-color: #ce1126;
    height: 600px;
    width: 900px;
}

.flag > div{
    position: relative;
    background-color: #002868;
    height: 300px;
    width: 900px;
    text-align: center;
    top: 140px;
    
}

.flag p{
    position: absolute;
    color: white;
    text-align: center;
    left: 320px;
    top: -80px;
    font-size: 80px;
}

.flag > div > div {
    position: absolute;
    background-color: white;
    height: 200px;
    width: 200px;
    border-radius: 50%;
    text-align: center;
    left: 350px;
    top: 45px;
}

.flag div > div > p{
    position: absolute;
    color: #000000;
    text-align: center;
    left: 10px;
    right: 10px;
    top: -60px;
    font-size: 70px;
}
```
```HTML
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <title>CSS Flag Project</title>
<link rel="stylesheet" href="./style.css">
</head>

<!-- 
  IMPORTANT! Do not change any HTML
Don't add any classes/ids/elements 
Use what you know about combining selectors 
and CSS specificity instead.
Hint 1: The flag is 900px by 600px and the circle is 200px by 200px.
Hint 2: You can use CSS inspection to get the colors from
https://appbrewery.github.io/flag-of-laos/
-->

<body>
  <div class="flag">
    <p>The Flag</p>
    <div>
      <div>
        <p>of Laos</p>
      </div>
    </div>
  </div>
</body>

</html>
```
## Project #7: Web Design Agency.

```CSS
/* style.css*/

body {
  font-family: "Poppins", sans-serif;
  margin: 50px 50px 0 50px;
  background-color: #faf9f6;
  display: flex;
  flex-direction: column;
  min-height: 95vh;
}
.main {
  flex: 1;
}

h1 {
  font-size: 5rem;
  margin-right: 800px;
}

span{
  color: midnightblue;
}

.left{
  float: left;
  
}

.right{
  float: right;
}

.tile-image{
  float: left;
  height: 200px;
  width: 300px;
  padding-right: 50px;
}

.card-text{
  text-align: justify;
  margin-left: -430px;
}

footer {
  clear: both;
  text-align: right;
  color: midnightblue;
}
```
```CSS
/* mobiles.css*/

@media (min-width: 319px) and (max-width: 480px) {
      body {
        font-family: "Poppins", sans-serif;
        margin: 13px 13px 0 13x;
        background-color: #faf9f6;
        display: flex;
        flex-direction: column;
        min-height: 95vh;
      }
      .main {
        flex: 1;
      }
    
      .logo{
         height: 18px;
      }
      
      h1 {
        font-size: 2rem;
        margin: 0px 24px;
        text-align: center;
      }
      
      span{
        color: midnightblue;
      }
      
      .tile-image{
        height: 200px;
        width: 300px;
        margin-left: -10px;
      }
      
      .card-text{
        height: 200px;
        width: 250px;
        margin-left: 50px;
      }
      
      footer {
        clear: both;
        text-align: right;
        color: midnightblue;
      }    
  }
```
```CSS
/* tablets.css*/

@media (min-width: 481px) and (max-width: 1200px) {
  body {
    font-family: "Poppins", sans-serif;
    margin: 26px 26px 0 26x;
    background-color: #faf9f6;
    display: flex;
    flex-direction: column;
    min-height: 95vh;
  }
  .main {
    flex: 2;
  }

  .logo{
     height: 36px;
  }
  
  h1 {
    font-size: 4rem;
    margin: 0px 95px;
    text-align: center;
  }
  
  span{
    color: midnightblue;
  }
  
  .tile-image{
    float: left;
    margin-top: 50px;
    height: 200px;
    width: 250px;
  }

  .card-title{
   margin-top: 210px;
  }
  
  .card-text{
    height: 200px;
    width: 250px;
    margin-left: 0px;
  }
  
  footer {
    clear: both;
    text-align: right;
    color: midnightblue;
  }  
}
```
```CSS
/* Laptops*/

@media (min-width: 481px) and (max-width: 1200px) {
  body {
    font-family: "Poppins", sans-serif;
    margin: 26px 26px 0 26x;
    background-color: #faf9f6;
    display: flex;
    flex-direction: column;
    min-height: 95vh;
  }
  .main {
    flex: 2;
  }

  .logo{
     height: 36px;
  }
  
  h1 {
    font-size: 4rem;
    margin: 0px 95px;
    text-align: center;
  }
  
  span{
    color: midnightblue;
  }
  
  .tile-image{
    float: left;
    margin-top: 50px;
    height: 200px;
    width: 250px;
  }

  .card-title{
   margin-top: 210px;
  }
  
  .card-text{
    height: 200px;
    width: 250px;
    margin-left: 0px;
  }
  
  footer {
    clear: both;
    text-align: right;
    color: midnightblue;
  }  
}
```
```HTML
<!-- HTML Portion-->

<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Agency</title>
  <link rel="stylesheet" href="./style.css">
  <link rel="stylesheet" href="./laptops.css">
  <link rel="stylesheet" href="./tablets.css">
  <link rel="stylesheet" href="./mobiles.css">
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;700&display=swap" rel="stylesheet">
</head>

<body>
  <div class="main">
    <img class="logo" src="./assets/images/logo.png" alt="logo">
    <h1>We are a <span>Creative</span> Design Agency</h1>
    <div class="left card"><img class="tile-image" src="./assets/images/beautiful.jpg" alt="hand and flower in water">
      <h2 class="card-title">Beauty</h2>
      <p class="card-text">We strive to create the most beautiful websites for all your needs. Working closely with you
        to
        design and
        develop an amazing website for your business.</p>
    </div>

    <div class="right card"><img class="tile-image" src="./assets/images/construction.jpg" alt="metal structure">
      <h2 class="card-title">Construction</h2>
      <p class="card-text">Built by our team of professional developers, we ensure the most rigourous and modern websites. Built from
        scratch using HTML and CSS. Only the best for you.</p>
    </div>

  </div>
  <footer>
    <p>Create. Develop. Design.</p>
  </footer>
</body>

</html>
```
