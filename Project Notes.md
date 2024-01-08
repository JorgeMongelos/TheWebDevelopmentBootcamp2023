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