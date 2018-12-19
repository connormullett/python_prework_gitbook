# Borders

Objectives:

* Work with basic CSS borders.

## File Location <a id="file-location"></a>

You should be located in the following files:

```text
    Python_Projects
        └── prework
            └── HTMLPrework
            └── CSSPrework
                07-borders.css
                07-borders.html
```

To get started, let's stub out our `html` and `css` files.

```text
<!DOCTYPE html>
<html>
  <head>
    <title>Borders</title>
    <link rel="stylesheet" type="text/css" href="07-borders.css">
  </head>
  <body>
    <div class="wrapper">
      <h1>Borders</h1>
      <p id="title-p">The border property allows you to specify the style, width, and color of an element's border. </p>
    </div>
    <div class="border-style"></div>
    <div class="border-width"></div>
    <div class="border-color"></div>
  </body>
</html>
```

Then in the css file, set it up to look like this:

```text
/*
Border shorthand looks like this:    
p{
    border: 5px solid red;
}
The order is: border-width border-style(required) 
    border-color
*/
​
body{
    background-color: lightblue;
}
​
.wrapper{
    margin: 5px;
}
​
h1{
    text-align: center;
}
​
#title-p{
    text-align: center;
}
```

Notice, the comment about border css, that's the structure we'll be working with in the future.

## Border Styles <a id="border-styles"></a>

Let's start with our `border-style` `<div>`. Add the following `html` to our border-style divs.

```text
<h3><u>Border Style</u></h3>
<p>The border-style property can take up to four values (top border, right border, bottom border, and left border). The following border-style values are allowed:</p>
<ul>
  <li><b>dotted:</b> dotted border</li>
  <li><b>dashed:</b>  dashed border</li>
  <li><b>solid:</b>  solid border</li>
  <li><b>double:</b>  double border</li>
  <li><b>groove:</b>  3D grooved border, depends on border-color value</li>
  <li><b>ridge:</b>  3D ridged border, depends on the border-color value</li>
  <li><b>inset:</b>  3D inset border, depends on the border-color value</li>
  <li><b>none:</b>  no border</li>
  <li><b>hidden:</b> hidden border</li>
  <li><b>mixed:</b> you can set a different border style for the top, bottom, right, and left</li>
</ul>
```

Let's look through these properties. Most of these are fairly self-explanatory here, so let's see this in action.

```text
.border-style li{
    margin: 5px;
}
​
.border-style li:nth-child(1){
    border-style: dotted;
}
​
.border-style li:nth-child(2){
    border-style: dashed;
}
​
.border-style li:nth-child(3){
    border-style: solid;
}
​
.border-style li:nth-child(4){
    border-style: double;
}
​
.border-style li:nth-child(5){
    border-style: groove;
}
​
.border-style li:nth-child(6){
    border-style: ridge;
}
​
.border-style li:nth-child(7){
    border-style: inset;
}
​
.border-style li:nth-child(8){
    border-style: none;
}
​
.border-style li:nth-child(9){
    border-style: hidden;
}
​
.border-style li:nth-child(10){
    border-style: dotted dashed solid double;
}
```

Let's talk about this css, notice how they say:

```css
.border-style li:nth-child(10)
```

This is what we call a psuedo-class.

```text
selector:pseudo-class {
    property:value;
}
```

`Psuedo classes` allow us to more easily style things. A pseudo-class is used to define a special state of an element. Pseudo-classes let you apply a style to an element not only in relation to the content of the document tree, but also in relation to external factors like the history of the navigator \(:visited, for example\), the status of its content \(like :checked on certain form elements\), or the position of the mouse \(like :hover, which lets you know if the mouse is over an element or not\).

`Nth-child` is a psuedo-class that matches one or more elements based on their position among a group of siblings.

So here we're using the nth-child psuedo class to identify each list item and style them independently. Check out all of the cool border styles, and how using psuedo-classes we can style them all specifically without needing to assign an id to each one.

## Border Widths <a id="border-widths"></a>

In the `border-width` div, let's fill in the following html:

```text
<div class="border-width">
  <h3><u>Border Width</u></h3>
  <h4>VERY IMPORTANT: border-width will not work unless you have border-style set!!</h4>
  <p>Border-width can be set to a specific size (px, em, etc) or you can use one of the following pre-set settings: thin, medium, thick. The border-width property can also take up to four values (top, right, bottom, left)</p>
​
  <p id="four-widths">Here's an example of border-width being set to more than one value.</p>
</div>
```

Important to note here, is that border-width will not work unless you have border-style set. Let's add some style to this, add the following to your css file.

```text
.border-width p{
    border-style: solid;
    border-width: 5px;
}
​
#four-widths{
    border-style: solid;
    border-width: 2px 10px 4px 20px;
}
```

Hopefully you can see the differences in the two border widths after we apply our css. Notice the order of the widths described. This order, as always goes: top-right-bottom-left. Try drastically changing the widths of each side to see the changes.

## Border Colors <a id="border-colors"></a>

Let's talk about border color next, as you may expect it allows us to assign a color to our border. Let's add the following html to our `border-color` div.

```text
<div class="border-color">
    <h3><u>Border Color</u></h3>
    <h4>VERY IMPORTANT: border-color will not work unless you have border-style set!!</h4>
    <p>Border-color can be set by the following ways:</p>
    <ul>
        <li><b>name:</b> specify a color such as "blue"</li>
        <li><b>Hex:</b> specify a hex value, like "#eee"</li>
        <li><b>RGB:</b> specify a RGB value, like "rgb(100,100,100)"</li>
        <li><b>transparent</b></li>
    </ul>
</div>
```

Again, note that you need border-style to use border-color. Let's add some CSS to it, so that we can see it in action.

```text
/* 7 */
.border-color li:nth-child(1){
    margin: 5px;
    border-style: solid;
    border-color: blue;
}
​
.border-color li:nth-child(2){
    margin: 5px;
    border-style: solid;
    border-color: #eee;
}
​
.border-color li:nth-child(3){
    margin: 5px;
    border-style: solid;
    border-color: rgb(100,0,100);
}
​
.border-color li:nth-child(4){
    margin: 5px;
    border-style: solid;
    border-color: transparent;
}
```

Notice here, we're using the psuedo class nth-child again! This time you should be able to see the color differences between borders.

## Border Shorthands <a id="border-shorthands"></a>

As you see if we use all three properties, we're using three lines of css. Fortunately there is a shorthand way of using border and its properties. Let's look at the comment at the top of our css again. Notice how we can just do `border: 5px solid red` instead of `border-width: 5px`, `border-style: solid` and `border-color: red`.

```text
/*Border shorthand looks like this:​p{    border: 5px solid red;}​The order is: border-width border-style(required)     border-color*/
```

Make sure your HTML and CSS files look like below.

HTML:

```text
<!DOCTYPE html>
<html>
  <head>
    <title>Borders</title>
    <link rel="stylesheet" type="text/css" href="07-borders.css">
  </head>
  <body>
    <div class="wrapper">
      <h1>Borders</h1>
      <p id="title-p">The border property allows you to specify the style, width, and color of an element's border. </p>
​
      <!--2-->
      <div class="border-style">
        <h3><u>Border Style</u></h3>
        <p>The border-style property can take up to four values (top border, right border, bottom border, and left border). The following border-style values are allowed:</p>
        <ul>
          <li><b>dotted:</b> dotted border</li>
          <li><b>dashed:</b>  dashed border</li>
          <li><b>solid:</b>  solid border</li>
          <li><b>double:</b>  double border</li>
          <li><b>groove:</b>  3D grooved border, depends on border-color value</li>
          <li><b>ridge:</b>  3D ridged border, depends on the border-color value</li>
          <li><b>inset:</b>  3D inset border, depends on the border-color value</li>
          <li><b>none:</b>  no border</li>
          <li><b>hidden:</b> hidden border</li>
          <li><b>mixed:</b> you can set a different border style for the top, bottom, right, and left</li>
        </ul>
      </div>
​
      <hr>
​
      <!--4-->
​
      <div class="border-width">
        <h3><u>Border Width</u></h3>
        <h4>VERY IMPORTANT: border-width will not work unless you have border-style set!!</h4>
        <p>Border-width can be set to a specific size (px, em, etc) or you can use one of the following pre-set settings: thin, medium, thick. The border-width property can also take up to four values (top, right, bottom, left)</p>
​
        <p id="four-widths">Here's an example of border-width being set to more than one value.</p>
      </div>
​
      <hr>
​
      <!--6-->
      <div class="border-color">
        <h3><u>Border Color</u></h3>
        <h4>VERY IMPORTANT: border-color will not work unless you have border-style set!!</h4>
        <p>Border-color can be set by the following ways:</p>
        <ul>
          <li><b>name:</b> specify a color such as "blue"</li>
          <li><b>Hex:</b> specify a hex value, like "#eee"</li>
          <li><b>RGB:</b> specify a RGB value, like "rgb(100,100,100)"</li>
          <li><b>transparent</b></li>
        </ul>
      </div>
    </div>
  </body>
</html>
```

CSS:

```text
/*
Border shorthand looks like this:
​
p{
    border: 5px solid red;
}
​
The order is: border-width border-style(required) 
    border-color
*/
​
body{
    background-color: lightblue;
}
.wrapper{
    margin: 5px;
}
​
h1{
    text-align: center;
}
​
#title-p{
    text-align: center;
}
​
/* 3 */
.border-style li{
    margin: 5px;
}
​
.border-style li:nth-child(1){
    border-style: dotted;
}
​
.border-style li:nth-child(2){
    border-style: dashed;
}
​
.border-style li:nth-child(3){
    border-style: solid;
}
​
.border-style li:nth-child(4){
    border-style: double;
}
​
.border-style li:nth-child(5){
    border-style: groove;
}
​
.border-style li:nth-child(6){
    border-style: ridge;
}
​
.border-style li:nth-child(7){
    border-style: inset;
}
​
.border-style li:nth-child(8){
    border-style: none;
}
​
.border-style li:nth-child(9){
    border-style: hidden;
}
​
.border-style li:nth-child(10){
    border-style: dotted dashed solid double;
}
​
/* 5 */
.border-width p{
    border-style: solid;
    border-width: 5px;
}
​
#four-widths{
    border-style: solid;
    border-width: 2px 10px 4px 20px;
}
​
/* 7 */
.border-color li:nth-child(1){
    margin: 5px;
    border-style: solid;
    border-color: blue;
}
​
.border-color li:nth-child(2){
    margin: 5px;
    border-style: solid;
    border-color: #eee;
}
​
.border-color li:nth-child(3){
    margin: 5px;
    border-style: solid;
    border-color: rgb(100,0,100);
}
​
.border-color li:nth-child(4){
    margin: 5px;
    border-style: solid;
    border-color: transparent;
}
```

Next, we'll talk about position.

