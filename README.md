# JS-Multiple-color-squares

<p>Looping a grid of squares, next to a loop for changing the color specter.</p>
<p>You can see the live preview accesing: <a href="https://negrut112.github.io/JS-Multiple-color-squares/">https://negrut112.github.io/JS-Multiple-color-squares/</a></p>
<img src="https://i.imgur.com/8RJoTEG.jpg">

## HTML

<p>I have used the HTML to define the area where I’m working defining the height, width and the border style:</p>
<p>&lt;canvas id=“myCanvas” height=“310” width=“500” style=“border: 1px solid black”&gt;&lt;/canvas&gt;</p>

## JavaScript

<p>Here, we have two for loops, one inside the other. First loop is generating one row of squares then the 2nd loop is generating columns for each square of the row.</p>
<p>Regarding the colors I used the ‘rgb’ method to change each square color like this: decrementing RED with 42 and incrementing red by 15 from the intitial ‘rgb’(199, 79, 120);</p>

<pre><code>for(var i=0;i&lt;6;i++){<br>
for(var j=0;j&lt;6;j++){<br>
context.fillStyle=‘rgb(’+ Math.floor(199 - 42<em>j) + ‘, 79,’+ Math.floor(120+15</em>i)+’)’;<br>
context.fillRect(i<em>45+10,j</em>45+10,40,40);<br>
}<br>
}</pre></code>
