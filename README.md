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


